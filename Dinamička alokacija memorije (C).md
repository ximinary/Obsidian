#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$

Sve funkcije su u zaglavlju ```<stdlib.h>```
Alokacija memorije se dešava u [[Organizacija memorije (C)#Hip segment|hipu]], funkcije vraćaju adresu ([[Pokazivači (C)|pokazivač]]), objekti nisu imenovani i nemaju doseg, imaju dinamički životni vek.
___
```c
void *malloc(size_t n);
```
```malloc``` alocira blok memorije veličine ```n``` bajtova i vraća adresu bloka (```void```-pokazivač) ili ```NULL``` ako alokacija nije uspela.

Primer alokacije niza od 100 ```int```-ova (sa implicitnom konverzijom tipa):
```c
int* niz = malloc(100 * sizeof(int));
```
Možemo koristiti ```niz``` isto kao obični pokazivač na 0-ti element niza (ili kao obični niz osim u [[Pokazivači (C)#Pokazivači i nizovi|dva slučaja]])
___
```c
void *calloc(size_t n, size_t size);
```
```calloc``` alocira blok memorije za ```n``` objekata veličine ```size``` i <u>inicijalizuje ih nulama</u>, vraća adresu bloka (```void```-pokazivač) ili ```NULL``` ako alokacija nije uspela.
```c
int* niz = malloc(100, sizeof(int));
```
___
```c
void *realloc(void* memblock, size_t n);
```
```realloc``` realocira$^{[*]}$ blok ```memblock``` u blok veličine ```n``` i vraća adresu bloka (```void```-pokazivač) ili ```NULL``` ako alokacija nije uspela.
(Ne inicijalizuje nulama)

Ako ```memblock``` nije pokazivač na <u>početak bloka</u> — greška.

$[*]$: ![[Realokacija.png]]

___
Posle (re)alokacije uvek bitno proveravati da li je pokazivač ```NULL```.
___
```c
void free(void* memblock);
```
```free```oslobađa (dealocira) memoriju kolja je bila alocirana ```maloc```, ```calloc```, ```realloc```.

Posle oslobođenja moramo da postavimo pokazivač na ```NULL``` da ne bismo slučajno iskoristili.

Greške pri oslobađanju:
- oslobađanje memorije koja nije alocirana.
- oslobođenje pomoću pokazivača koji pokazuje unutar bloka, umesto na početak
- ponovo oslobađanje
---
Primer alokacije po unesenom broju:
```c
#include <stdio.h>
#include <stdlib.h>

int main() {
	int n, i, *a;
	scanf("%d", &n);  // Unos broja elemenata
	/* Alocira se memorija */
	if ((a = malloc(n*sizeof(int))) == NULL) {
	printf("Greska prilikom alokacije memorije\n");
	return 1;
	}
	/* Unos elemenata */
	for (i = 0; i < n; i++) scanf("%d",&a[i]);
	/* Ispis elemenata u obratnom poretku */
	for (i = n-1; i >= 0; i--) printf("%d ",a[i]);
	/* Oslobadjanje memorije */
	free(a);
	return 0;
}
```
Primer alokacije "unos do ```-1```"
```c
#include <stdio.h>
#include <stdlib.h>
#define KORAK 100

int main() {
int* a = NULL; /* Niz je u pocetku prazan */
int duzina = 0; /* broj popunjenih elemenata niza */
int alocirano = 0; /* koliko elemenata moze biti smesteno */
int i;
do {
printf("Unesi ceo broj (-1 za poslednji broj): ");
scanf("%d", &i);
/* Ako nema vise slobodnih mesta, vrsi se prosirivanje */
if (duzina == alocirano) {
alocirano += KORAK;
a = realloc(a, alocirano*sizeof(int));
if (a == NULL) return 1;
}
a[duzina++] = i;
} while (i != -1);
/* Ispis elemenata */
printf("Uneto je %d brojeva. Alocirano je %d bajtova\n",
duzina, alocirano*sizeof(int));
printf("Brojevi su : ");
for (i = 0; i<duzina; i++)
printf("%d ", a[i]);
/* Oslobadjanje memorije */
free(a);
return 0;
}

```

### Greške

### Fragmentacija memorije