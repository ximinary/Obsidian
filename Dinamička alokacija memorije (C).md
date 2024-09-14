#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$

Sve funkcije su u zaglavlju ```<stdlib.h>```
Alokacija memorije se dešava u [[Organizacija memorije (C)#Hip segment|hipu]], funkcije vraćaju adresu ([[Pokazivači (C)|pokazivač]]), objekti nisu imenovani i nemaju doseg, imaju dinamički životni vek.

```c
void *malloc(size_t n);
```
```malloc``` alocira blok memorije veličine ```n``` bajtova i vraća adresu bloka (```void```-pokazivač) ili ```NULL``` ako alokacija nije uspela.

Primer alokacije niza od 100 ```int```-ova (sa implicitnom konverzijom tipa):
```c
int* niz = malloc(100 * sizeof(int));
```