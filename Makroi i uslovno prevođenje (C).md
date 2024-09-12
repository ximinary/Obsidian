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
#define max(A, B) ((A) > (B))
...

a = MAX;          // biće zamenjeno sa: a = 100;
int niz[MAX];     // biće zamenjeno sa: int niz[100];

printf("MAX");    // neće biti zamenjeno
b = MAX_LEN;      // neće biti zamenjeno
```