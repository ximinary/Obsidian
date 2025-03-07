#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$

Funkcija ```main``` je glavna funkcija sa koje počinje izvršavanje programa.
Iz ```main``` (i drugih funkcija) pozivaju se druge funkcije: [[Standardne biblioteke (C)|bibliotečke]] ili korisnički.

U funkciju se obično izdvajaju neka izračunavanja, koja predstavljaju celinu i koristi se više puta u programu.

## Deklaracija, definicija i pozivanje.
```c
#include <stdio.h>

int kvadrat(int n);    // deklaracija
// kvadrat ima jedan parametar tipa int i vrača rezultat tipa int

int main() {
	printf("%d^2 = %d\n", 5, kvadrat(5)); 
	// poziv za vrednost 5 (fja vrača 25)
	
	printf("%d^2 = %d\n", 9, kvadrat(9)); 
	// poziv za vrednost 5 (fja vrača 81)
	
	return 0;
}

int kvadrat(int n) {    // definicija
	return n*n;
}
```

deklaracija (prototip):
```c
tip ime_fje(niz_deklaracija_parametara);
```
definicija:
```c
tip ime_fje(niz_deklaracija_parametara) {
	deklaracije_lokalnih_promenljivih;
	naredbe;
	return __;        // opcion
}
```

Ako nećemo deklarisati pre definicije, funkcija će biti deklarisana i definisana odjednom.

**!** Funkcija mora da bude deklarisana <u>pre</u> (iznad) poziva. 
## Parametri
Parametri — promenljivi koji čine deklaraciju funkcija.
Argumenti — izrazi koji su navedeni u pozivu funkcije.

Parametri su lokalne promenljivi funkcije.

Funkcija koja ne uzima parametre:  ```tip funkcija(void);```
— parametra sigurno nema, poziv samo ```funkcija();```

Funkciju ```tip funkcija();``` možemo pozvati: ```funkcija(šta_god);```

## Prenos argumenata
Argument u pozivu može biti promenljiva ili izraz, čija vrednost može da se konvertuje u tip parametra.

Vrednost argumenta se kopira u lokalnu promenljive funkcije; funkcija radi samo sa kopijom nemenjajući original.

Imena parametra i argumenta mogu da se poklapaju ali oni ostaju različite.

Prilikom pozivanja radi se implicitna konverzija tipova.

---
Kao argument moguće je proslediti [[Pokazivači (C)|pokazivač]] na neku promenljivu, time omogućujući promenu te promenljive u funkciji.

Niz ne može biti argumentom, samo ime niza, koje se konvertuje u pokazivač na njegov početak.
Niz se ne kopira, samo je moguće menjati originalan niz.
```c
tip ime_fje(tip ime_niza[]);
```
isto što i :
```c
tip ime_fje(tip *ime_niza);
```
Višedimenzioni niz (potrebno navesti sve dimenzije osim prve):
```c
tip ime_fje(tip ime_niza[][dim2][dim3]...);
```
isto što i :
```c
tip ime_fje(tip (*ime_niza)[dim2][dim3]...);
```
___
Promenljiva korisnički definisanog tipa se prenosi kao i obična promenljiva, tj kopiranjem vrednost.
___
##### Argumenti funkcije ```main```
```c
int main (int argc, char* argv[]) {...;}
```
```argc``` — broj argumenata;
```argv``` — pokazivač na niz pokazivača koji pokazuju na argumente (niske).

Primer:
poziv programa:
```
./a.out 12345 -u zdravo "16 KB"
```
onda ```argc``` će biti ```5```
```argv[0]``` je pokazivač na nisku ```"./a.out"```
```argv[1]``` je pokazivač na nisku ```"12345"```
```argv[2]``` je pokazivač na nisku ```"-u"```
```argv[3]``` je pokazivač na nisku ```"zdravo"```
```argv[4]``` je pokazivač na nisku ```"16 KB"```

![[argumenti_main.png]]
## Povratna vrednost
```c
tip funkcija(...) {
	...
	return __;
	// return konvertuje __ u tip vraća vrednost i prekida izvršavanje fje, program se vraća ka izvršavanju fje, iz koje je bila pozvana ova fja.
}
```
Funkcija ne vraća ništa:
```c
void funkcija(...) {
	...
	return; // opcion; samo prekida fju.
}
```

Povratna vrednost može biti korisnički definisanog tipa, ali ne može biti niz.

```main``` mora da ima povratni tip ```int```
Konvencija: ```main``` vraća ```0``` ako nema grešaka, i ne-nula kod greške, ako je došlo do greške.
## Funkcije sa promenljivim brojem argumenata

Koriste se uz pomoć uključivanja zaglavlja ```<stdarg.h>```.

Tip podataka: ```va_list``` — lista argumenata.
```va_start(lista, br_argumenata)``` — početak
```va_arg(lista, tip)``` — vrača naredni argument
```va_end(lista)``` — kraj

Primer:
```c
#include <stdio.h>
#include <stdarg.h>

int sumof(int n_args, ...) {
		// n_args - broj argumenata.
	int i, sum;
	va_list args;
	va_start(args, n_args);
	sum = 0;
	for (i = 0; i < n_args; i++) 
		sum += va_arg(args, int);
	va_end(args);
	return sum;
}

int main() {
	printf("%d\n", sumof(4, 4, 34, 9, 6));
	return 0;
}
```