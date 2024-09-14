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
```realloc``` realocira$^{[1]}$ blok ```memblock``` u blok veličine ```n``` i vraća adresu bloka (```void```-pokazivač) ili ```NULL``` ako alokacija nije uspela.
(Ne inicijalizuje nulama)

Ako ```memblock``` nije pokazivač na <u>početak bloka</u> — greška.

$[1]$:

___
Posle (re)alokacije uvek bitno proveravati da li je pokazivač ```NULL```.