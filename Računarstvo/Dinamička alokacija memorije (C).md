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

```realoc(NULL, k);``` je isto što i ```malloc(k);```
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
	int n, i;
	scanf("%d", &n);     //unos broja elemenata
	
	//alokacija:
	int* a = malloc(n*sizeof(int));
	if (a == NULL) {     //provera pokazivača
		printf("Greska\n");
		return 1;
	}

	for (i = 0; i < n; i++)
		scanf("%d",&a[i]);
		
	for (i = n-1; i >= 0; i--)
		printf("%d ",a[i]);

	free(a);             //oslobađanje memorije
	return 0;
}
```
Primer alokacije "unos do ```-1```":
```c
#include <stdio.h>
#include <stdlib.h>
#define KORAK 100

int main() {
	int* a = NULL;     //niz je u pocetku prazan
	int duzina = 0;    //broj popunjenih elemenata niza
	int alocirano = 0;
	
	do {
		if (duzina == alocirano) {
			alocirano += KORAK;
			a = realloc(a, alocirano*sizeof(int));
			if (a == NULL) return 1;
		}
		scanf("%d", &a[duzina]);
	} while (a[duzina++] != -1);
	
	// ...
	
	free(a);
	return 0;
}

```

### Greške
- Curenje memorije — kada se izgubi pokazivač na alocirani blok:
  ```c
  p = malloc(1000);
  ...
  p = malloc(2000);
  ```
- Pristup oslobođenoj memoriji
- Pristup memorije van bloka
- Oslobađanje/realokacija pogrešnog pokazivača (koji ne pokazuje na početak već alociranog bloka)
### Fragmentacija memorije
Često alociranje i dealociranje može dovesti do fragmentacije.

Uprošćeni primer:
Neka je 1 - alocirana memorija, 0 - nealocirana.
```
0000 0000 0000 0000
____                    malloc
1111 0000 0000 0000
     ____ __            malloc
1111 1111 1100 0000
xxxx                    free
0000 1111 1100 0000
            __ ___      malloc
0000 1111 1111 1110
__                      calloc
1100 1111 1111 1110
     ___x xx            realloc
1100 1110 0011 1110
```
iako je ostalo 6 nula, nemoguće je alocirati blok od 4 jedinice.

Kako izbegavati:
- izbegavati dinamičku alokaciju
- alocirati odmah u većim blokovima
- memory pooling