#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$

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


### Povezanost identifikatora. ```ststic``` i ```extern```
— promenljive sa istim imenom u različitim objektnim modulima.

- BEZ POVEZANOSTI:
	- lokalne promenljivi
	- korisnički definisani tipovi
- SA SPOLJAŠNJOM POVEZANOŠĆU