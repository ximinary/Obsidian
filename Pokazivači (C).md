#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$
— vrednosti su memorijske adrese.
(4B — 32bit računar, 8B — 64bit računar)

```c
int *p1;
int* p2;
int* p3, p4;

// p1, p2, p3 su pokazivači na int
// p4 je tipa int
```

Operator referenciranja ```&```:
```c
int a = 10, *p;
p = &a;        // adresa a se zapisuje u p
```
Operator dereferenciranja ```*```:
```c
*p = 5;        // a će postati 5
```

Opšti (generički) pokazivač ```void*```:
— pokazivač bez tipa, koji ne možemo koristiti bez [[Predstavljanje podataka i operacije nad njima (C)#^fb3fd7|konvertiranja]] u potreban tip. 
```c
void* pa = &a;
*pa = 15;      // greška!!!
```

Pokazivač ni na šta:
```c
p = NULL;
```

```const```:
```c
int* const pb;  //konstantni pokazivač
const int* pc;  //

```