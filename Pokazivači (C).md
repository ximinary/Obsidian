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

### Pokazivači i niske

### Pokazivači na funkcije