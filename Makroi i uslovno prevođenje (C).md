#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$

Jednostavne operacije nad tekstualnim sadržajem programa, koje se vrše u fazi pretprocesiranja.

### Uključivanje datoteka zaglavlja — ```#include```

uključivanje u program prototipa funkcija:
```c
#include "ime_datoteke.h"  //iz direktorijuma programa
#include <ime_datoteke.h>  //iz direktorijuma standardnih biblioteka
```

### Makro zamene — ```#define```
```c
#define ORIGINALNI_TEXT novi_tekst
// zamena niza karaktera drugim nizom
```

Primer
```c
#define MAX 100
...

a = MAX;          // biće zamenjeno sa: a = 100;
int niz[MAX];     // biće zamenjeno sa: int niz[100];

printf("MAX");    // neće biti zamenjeno
b = MAX_LEN;      // neće biti zamenjeno
```

Zamene sa argumentima:
```c
#define max(A, B) ((A) > (B) ? (A) : (B))
...
//tekst programa  ->  posle prevođenja

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

složeni identifikator ```##```: