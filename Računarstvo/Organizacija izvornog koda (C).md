#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$

### Od izvornog do izvršivog programa
- PRETPROCESIRANJE — jednostavne [[Makroi i uslovno prevođenje (C)|zamene]] u tekstu programa. Objedinjava kod iz različitih datoteka (```#include```) u **jedinici prevođenja**.
  ```
  gcc -E 1.c
  ```
  ^14a8a4
- KOMPILACIJA
  Jedinica prevođenja $\to$ **objektni modul** (ne može da se izvrši)
	- Predni sloj: 
		- <u>leksička analiza</u> (izdvajanje leksema)
		- <u>sintaksička analiza</u> (kreiranje sintaksičkog stabla)
		- <u>semantička analiza</u> (transformacija stabla)
		- <u>generisanje međukoda</u> ("asemblerski kod")
	- Srednji sloj:
		- <u>optimizacija međukoda</u>
	- Zadnji sloj:
		- <u>generisanje ciljnog (mašinskog) koda</u>
		- <u>optimizacija ciljnog koda</u>
	```
  gcc -c 1.c     //rezultat u 1.o
  ```
 
- POVEZIVANJE — kreiranje jedinstvene izvršive datoteke od jednog ili više objektnih modula (koje su dobiti kompilacijom ili već postoje) — poveziva adrese funkcija i nekih promenljivih.
  ```
  gcc program -o 1.o 2.c -m    //-m za <math.h>
  ```

[[Od izvornog do izvršivog.png|Primer]] #todo

### Organizacija koda u više datoteka. ```make```

Izdvajanje neke celine — grupe funkcija u odvojenu datoteku se vrši za:
- kompiliranje jednom i zatim korišćenje objektnog modula
- korišćenje u nekoliko različitih programa
$\:$

```.h``` datoteka sadrži deklaracije funkcija odgovarajuće ```.c``` datoteke, deklaracije globalnih promenljivih i definicije struktura.

```.c``` datoteka sadrži definicije funkcija, deklaracije globalnih promenljivih i konstanti, definicije struktura

Primer:

main.c:
```c
#include "liste.h"

int veci_od(cvor* lista, int broj) {
    int count = 0;
    while (lista != NULL) {
        if (lista->x > broj)
            count++;
        lista = lista->sl;
    }
    return count;
}

int main() {
    int n, k;
    scanf("%d %d", &n, &k);
    cvor* lista = NULL;
    ucitaj_listu(&lista, n, stdin);
    printf("%d\n", veci_od(lista, k));
    oslobodi_listu(&lista);
    return 0;
}
```
liste.h:
```c
#ifndef _LISTE_
#define _LISTE_

#include <stdio.h>
#include <stdlib.h>

typedef struct cvor {
    int x;
    struct cvor* sl;
} cvor;

void greska(); 

cvor* novi_cvor(int x);

void dodaj_na_pocetak(cvor** pPocetak, int x);
void dodaj_na_kraj(cvor** pPocetak, int x);
void ispisi_listu(cvor* tekuci, FILE* f);
void ucitaj_listu(cvor** pPocetak, int n, FILE* f);
void oslobodi_listu(cvor** pPocetak);

#endif
```
liste.c:
```c
#include "liste.h"

void greska() {
    fprintf(stderr, "-1\n");
    exit(EXIT_FAILURE);
}

cvor* novi_cvor(int x) {
    cvor* novi = malloc(sizeof(cvor));
    if (novi == NULL) greska();
    novi->x = x;
    return novi;
}

void dodaj_na_pocetak(cvor** pPocetak, int x) {
    cvor* novi = novi_cvor(x);
    novi->sl = *pPocetak;
    *pPocetak = novi;
}

void dodaj_na_kraj(cvor** pPocetak, int x) {
    cvor* novi = novi_cvor(x);
    novi->sl = NULL;
    if (*pPocetak == NULL)
        *pPocetak = novi;
    else{
        cvor* kraj;
        for (kraj = *pPocetak; kraj->sl != NULL; kraj = kraj->sl);
        kraj->sl = novi;
    }
}

void ispisi_listu(cvor* tekuci, FILE* f) {
    while (tekuci != NULL) {
        fprintf(f, "%d ", tekuci->x);
        tekuci = tekuci->sl;
    }
    printf("\n");
}

void ucitaj_listu(cvor** pPocetak, int n, FILE* f) {
    int tekuci, i;
    for (i = 0; i < n; i++) {
        fscanf(f, "%d", &tekuci);
        dodaj_na_kraj(pPocetak, tekuci);
    }
}

void oslobodi_listu(cvor** pPocetak) {
    cvor* tekuci;
    while(*pPocetak != NULL) {
        tekuci = *pPocetak;
        *pPocetak = (*pPocetak)->sl;
        free(tekuci);
    }
}
```
makefile:
```makefile
program : main.o liste.o
    gcc -o program main.o liste.o
liste.o : liste.c liste.h
    gcc -c liste.c
main.o : main.c liste.h
    gcc -c main.c
```
$\:$

```make``` određuje zavisnost datoteka, tako što
```makefile
fajl1 : fajle_od_kojih_zavisi_fajl1
	gcc kako se kreira fajl
```
Prvim treba navesti ciljni fajl.

Komandna linija:
```
make
```

```make``` će kreirati stablo zavisnosti i gledajući na vreme poslednjih promena datoteka će izvršavati samo potrebne komande u potrebnom redosledu.

U primeru ako se promenio ```main.c```, prvo će biti izvršeno ```gcc -c main.c``` da bi se dobio ```main.o``` pa će izvršiti ```gcc -o program main.o liste.o```.

