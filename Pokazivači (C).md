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
// greška: *pa = 15;
```

Pokazivač ni na šta:
```c
p = NULL;
```

```const```:
```c
int* const pb = &b;
//konstantni pokazivač; greška: pb = &c;

const int* pc;       
//pokazivač preko kojeg nije moguće menjati promenljivu na koju on pokazuje (greška: *pc = 5;), samo čitati
```
$\:$
Primer korišćenja pokazivača — swap:
```c
void swap(int *pa, int *pb) {
	int tmp = *pa;
	*pa = *pb;
	*pb = tmp;
}

int main() {
	int a = 5, b = 9;
	swap(&a, &b);
	printf("%d %d\n", a, b);
	return 0;
}
```

### Pokazivačka aritmetika
```c
tip *p, *q;
int i;
              //neformanlo,
              //u apsolutnim veličinama:
q = p + i     //p + i*sizeof(tip)
i = p - q;    //(p - q)/sizeof(tip)
```
- pokazivač ```p``` nekog <u>tipa</u> +/- ceo broj ```i``` je vrednost ```p``` (adresa) pomerena udesno/ulevo na ```i``` prostora veličine tog <u>tipa</u>.

- razlika dva pokazivača istog <u>tipa</u> je tipa ```int``` i jednaka je broju prostora veličine tog <u>tipa</u> između njihovih vrednosti.

```c
int main() {
	int a[] = {26, 54, 89};
	int *p = &(a[0]);
	int *q = &(a[2]);
	printf("%d ", q-p);
	p++;
	printf("%d\n", *p);
	return 0;
}
// ispis: 2 54
```
### Pokazivači i nizovi
```c
int a[10], *pa, i;
pa = a;      // isto što i pa = &a[0]
```
ime niza se konvertuje u pokazivač na 0-ti element niza osim u dva slučaja:
```c
sizeof(a)    // 40 - koliko prostora zauzima ceo niz
sizeof(pa)   // 8 - koliko prostora zauzima pokazivač
```
```c
&a           // pokazivač na ceo niz;
             // ima istu adresnu vrednost što i pa;
             // ali tip je int (*)[10]
             
             //zbog implicitne kovertacije tipova
             //(pa = a;) je isto što i (pa = &a;)
             
&pa          // pokazivač na pokazivač;
             // tip je int**
```

U ostalim slučajevima ime niza moguće koristi kao pokazivač i obratno pokazivač moguće koristiti kao ime niza pri pristupanju elemenata, na primer ```pa[3]```.

Sledeći izrazi su ekvivalentni (uz nastavak primera):
```c
  a + i  = &a[i] =   pa + i  = &pa[i]  //adresa
*(a + i) =  a[i] = *(pa + i) =  pa[i]  //element niza
```
---
```c
int niz[10];
int *a[10];     // niz od 10 pokazivača na int
int (*b)[10];   // pokazivač na niz od 10 int-ova
                // tip je int (*)[10]
b = &niz;

// b + 2 ima vrednost b + veličina 2 niza od 10 int-ova, tj u absolutnim vrednostima b + 80

// b[2] je niz od 10 elementa na absolutnoj adresi b + 80 (izvne deklarisanig, samo za primer), konvertuje se u nulti ele
(*b)[3]
```
---

### Pokazivači i niske

### Pokazivači na funkcije