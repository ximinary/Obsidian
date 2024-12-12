#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]


### Doseg identifikatora 
— određuje deo programa u kojem je identifikator vidljiv.

Globalni:
- doseg **datoteke** — ime važi od tačke uvođenja do kraja datoteke (globalne promenljive);

Lokalni:
- doseg **bloka** — ime važi od tačke uvođenja do kraja bloka (lokalne promenljive);
- doseg **funkcije** — ime važi u celoj funkciji (lokalne promenljive koje se koriste uz ```goto``` naredbu)
- doseg **prototipa funkcije** — ime važi u okviru prototipa funkcije.
$\:$

Konflikt identifikatora — smatraju se kao različite promenljive.
```c
int main() {
	int a = 3, i;
	for (i = 0; i < 4; i++) {
		int a = 5;
		printf("%d ", a);
	}
	printf("%d\n", a);
	return 0;
}
// ispis: 5 5 5 5 3
```

### Životni vek objekata. ```static``` i ```auto```
— deo vremena izvršavanja programa u kojem se promenljiva može koristiti i za nju je rezervisano mesto u memoriji.
- **statički** — objekt je dostupan tokom celog izvršavanja programa.
- **automatski** — promenljive koje se automatski stvaraju i uklanjaju prilikom pozivanja funkcija.
- **dinamički** — promenljive koje se alociraju i dealociraju na eksplicitan zahtev programera (kada količina memorije bude poznata samo tokom izvršavanja programa — [[Dinamička alokacija memorije (C)|dinamička alokacija memorije]]).

Globalni promenljivi su uvek statički.

Lokalne promenljive:
```c
void f() {
	int a;          // automatski ž.v.
	auto int b;     // automatski ž.v.
	       //(auto — u suštiti ne treba navoditi)
	       
	static int c;   // statički ž.v.
}
```

Lokalne statičke promenljive:
- kreiraju se na početku izvršavanja programa;
- mogu se koristiti samo u bloku, u kojem su deklarisani;
- vrednost se čuva posle izvršavanja funkcije i pri novom pozivu ostaje ista (iako je inicijalizovana);

primer:
```c
void f() {
	int a = 0;
	printf("f: %d\n", a);
	a++;
}

void g() {
	static int a = 0;
	printf("g: %d\n", a);
	a++;
}

int main() {
	f(); f(); f(); f();
	g(); g(); g(); g();
	return 0;
}
```


Globalne i statičke lokalne promenljive se inicijalizuju nulom.

### Povezanost identifikatora. ```static``` i ```extern```
— promenljive sa istim imenom u različitim objektnim modulima.

- BEZ POVEZANOSTI:
	- lokalne promenljivi
	- korisnički definisani tipovi
- SA SPOLJAŠNJOM POVEZANOŠĆU
  (promenljive/fje sa istim imenom u različitim fajlovima se računaju kao jedna promenljiva/fja)
	- globalne promenljive i funkcije
		- bez kvalifikatora
		- ```extern``` — promenljiva/fja je definisana u drugom fajlu (mora bar u jednom fajlu bez ```extern```!)
		  — moguće navesti u bloku da bi bila vidljiva samo tamo

Primer:
1.c:
```c 
#include <stdio.h>

int a;          // = 0
int b = 3;

void f() {
	printf("a = %d\n", a);
}
```
2.c:
```c 
#include <stdio.h>

extern int a;
void f();

void g() {
	extern int b;
	printf("b = %d\n", b);
	f();
}

int main() {
	a++;             // b nije vidljiva ovde
	g();
	return 0;
}
```
ispis: 
```
b = 3
a = 1
```

- SA UNUTRAŠNJOM POVEZANOŠĆU
	- globalna promenljiva/fja sa kvalifikatorom ```static``` 
	  (neće biti povezana sa promenjivoj/fjoj sa istim imenom u drugom fajlu)

Primer:
1.c:
```c 
#include <stdio.h>

static int a = 3;  // sa unutrašnjom
int b = 5;         // sa spoljašnjom

static void f() {
	printf("f: a = %d, b = %d\n", a, b);
}

int g() {
	f();
	return 1;
}
```
2.c:
```c 
#include <stdio.h>

int g();
int a, b;

double f() { ...; }
//nikako nije povezana sa f u drugom fajlu.

int main() {
	printf("main: a = %d, b = %d\n", a, b);
	
	if (g())
		return 0;
	return 1;
}
```
ispis: 
```
main: a = 0, b = 5
f: a = 3, b = 5
```