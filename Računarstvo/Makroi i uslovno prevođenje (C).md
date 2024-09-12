#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$

Jednostavne operacije nad tekstualnim sadržajem programa, koje se vrše u fazi [[Organizacija izvornog koda (C)#^14a8a4|pretprocesiranja]].

### Uključivanje datoteka zaglavlja — ```#include```

uključivanje u program prototipa funkcija:
```c
#include "ime_datoteke.h"  //iz direktorijuma programa
#include <ime_datoteke.h>  //iz direktorijuma standardnih biblioteka
```

### Makro zamene — ```#define```
Zamena:
```c
#define ORIGINALNI_TEXT novi_tekst
// zamena niza karaktera drugim nizom
```

Kraj primene zamene: 
```c
#undef ORIGINALNI_TEXT
```


Primer
```c
#define MAX 100
...
//tekst programa  ->  posle prevođenja

a = MAX           ->  a = 100 
int niz[MAX]      ->  int niz[100]

printf("MAX");    //  neće biti zamenjeno
b = MAX_LEN;      //  neće biti zamenjeno
```

Zamene sa argumentima:
```c
#define max(A, B) ((A) > (B) ? (A) : (B))
...
max(2, 3)         ->  ((2) > (3) ? (2) : (3))

max(x+2, 4*y)     ->  ((x+2) > (4*y) ? (x+2) : (4*y))

max(x++, ++y)     ->  ((x++) > (--y) ? (x++) : ++y))
// nije funkcija inkrementiraće dva puta!
```

treba paziti na zagrade:
```c
#define kvadrat(x) x*x
...
kvadrat(a + 2)    ->  a + 2*a + 2         // !
```
```c
#define kvadrat(x) (x)*(x)
...
kvadrat(a + 2)    ->  (a + 2)*(a + 2)
10/kvadrat(a)     ->  10/(a)*(a)          // !
```
```c
#define kvadrat(x) ((x)*(x))
...
10/kvadrat(a)     ->  10/((a)*(a))
```

zamena vrednosti promenljivih:
```c
#define swap(t, x, y) { t z; z = x; x = y; y = z; }
...
swap(int, a, b)   ->  { int z; z = a; a = b; b = z; }
```

zamena sa ```" "``` — identifikator ```#```:
```c
#define dprint(EXP) printf(#EXP " = %d", EXP)
...
dprint(x/y)       ->  printf("x/y" " = %d", x/y)
```

zamena unutra imena promenljive — identifikator ```##```: 
```c
#define dodaj_u_niz(ime, element) \
	niz_##ime[brojac_##ime++] = element
...
dodaj_u_niz(a, 2) ->  niz_a[brojac_a++] = 2
```


### Uslovno prevođenje

```c
#ifdef      // ako je definisano
#ifndef     // ako nije definisano
#else       // inače
#endif      // kraj uslova
```

Primer:
```c
#include <stdio.h>
#define SRB

int main() {
	#ifdef SRB
		printf("Zdravo\n");
	#else 
		printf("Hello\n");
	#endif
	return 0;
}
```

Definisanje preko komandne linije:
```
gcc -D SRB 1.c
```