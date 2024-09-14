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
int *a[10];     // niz od 10 pokazivača na int
int (*b)[10];   // pokazivač na niz od 10 int-ova
                // tip je int (*)[10]

int niz[10];
b = &niz;

// b + 2 ima vrednost b + veličina 2 niza od 10 int-ova, tj u absolutnim vrednostima b + 80

// b[2] je niz od 10 elementa na absolutnoj adresi b + 80 (izvne deklarisanog, samo za primer), konvertuje se u pokazivač na nulti element tog niza.

// (*b)[3] je isto što i niz[3]
```
---
```c
int d[dim1][dim2][dim3]..;
```
```d``` se konvertuje u pokazivač na 0-ti element niza ```d``` - niz tipa ```int (*)[dim2][dim3]..```

Primer:
```c
int A[10][20];
```
Neka niz ```A``` počinje sa adrese ```0```, tada
```c
izraz         tip               vrednost

&A[0][2]      int*              8
&A[2][0]      int*              2*20*4 = 160
&A[2][6]      int*              (2*20 + 6)*4 = 184


A[2]          int[20]
              //konvertuje se:
              int*              160
A[2] + 6      int*              160 + 6*4 = 184


&A[2]         int (*)[20]       160
&A[2] + 6     int (*)[20]       160 + 6*20*4 = 640 


A             int[10][20]      
              //konvertuje se:
	          int (*)[20]       0
A + 6         int (*)[20]       0 + 6*20*4 = 480


&A            int (*)[10][20]   0
&A + 6        int (*)[10][20]   0 + 6*10*20*4 = 4800
```
### Pokazivači i niske
Konstantne niske se čuvaju u [[Organizacija memorije (C)#Segment podataka (.data i .BSS)|segmentu podataka]], niska navedena u tekstu programa u ```" "``` se konvertuje u pokazivač (tipa ```char*```) na njen početak u segmentu podataka.
Konstantne niske je nemoguće menjati.

```c
printf("%d", x);  // prvi argument je tipa char*

cahr* p = "informatika";
//greška: p[5] - 'k';
p++;
printf("%s", p);  //ispis: nformatika
```

```c
char a[] = "informatika"; // u stek okviru kreira se niz dužine 12 i popunjava se karakterima konstantne niske: a[0] = 'i', ..., a[11] = '\0'.
// nisku a već možemo da menjamo (karakrer po karakter)
```

implementacija ```strcpy```:
```c
void strcpy(char *a, const char* b) {
	while (*(a++) = *(b++));
}
...
//pozivi:
char s[20], t[20].
strcpy(s, "informatika");
strcpy(t, s)
```

Niz niski:
![[niz_niski.png]] #todo

### Pokazivači na funkcije
— omogućavaju slanje funkcije kao argument druge funkcije.

```c
//prototip funkcije koja vraća pokazivač na double:
double *a(int, float);

//deklaracija pokazivača na funkciju koja uzima int i float i vraća double:
double (*a)(int, float);
//a je tipa double (*)(int, float)

//deklaracija niza pokazivača na funkciju koja uzima int i float i vraća double:
double (*a[3])(int, float);
```

Isti operatori referenciranja ```&``` i dereferenciranja ```*```.

U praktici ```&``` se ne koristi jer ime funkcije, koje je napisano bez ```( )```, automatski se konvertuje u pokazivač na tu funkciju.

Primer korišćenja:
```c
#include <stdio.h>
#define N 5

void ucitaj_niz(int* a, int n) {
	for (i = 0; i < n; i++)
		scanf("%d", a + i);
}

void ispisi_niz(int* a, int n) {
	for (i = 0; i < n; i++)
		printf("%d ", a[i]);
	printf("\n");
}

void map(int* a, int n, int(*op)()) {

}

```