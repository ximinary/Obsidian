#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$
Funkcija ```main``` je glavna funkcija sa koje počinje izvršavanje programa.
Iz ```main``` (i drugih funkcija) pozivaju se druge funkcije: [[Standardne biblioteke. Ulaz i izlaz (C)|bibliotečke]] ili korisnički.

U funkciju se obično izdvajaju neka izračunavanja, koja predstavljaju celinu i koristi se više puta u programu.

## Deklaracija, definicija i pozivanje.
```c
#include <stdio.h>

int kvadrat(int n);    // deklaracija
// kvadrat ima jedan parametar tipa int i vrača rezultat tipa int

int main() {
	printf("%d^2 = %d", 5, kvadrat(5)); 
	// poziv za vrednost 5 (fja vrača 25)
	
	printf("%d^2 = %d", 9, kvadrat(9)); 
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

##### Parametre funkcije ```main```
#todo
## Prenos argumenata
Argument u pozivu može biti promenljiva ili izraz, čija vrednost može da se konvertuje u tip parametra.

Vrednost argumenta se kopira u lokalnu promenljive funkcije; funkcija radi samo sa kopijom nemenjajući original.

Imena parametra i argumenta mogu da se poklapaju ali oni ostaju različite.

Prilikom pozivanja radi se implicitna konverzija tipova.

---
Kao argument moguće je proslediti pokazivač na neku promenljivu, time omogućujući promenu te promenljive u funkciji.

Niz ne može biti argumentom, samo ime niza, koje se konvertuje u pokazivač na njegov početak.
Niz se ne kopira, samo je moguće menjati originalan niz.
```c
tip ime_fje(tip ime_niza[]);
```
isto što i :
```c
tip ime_fje(tip* ime_niza);
```
Višedimenzioni niz (potrebno navesti sve dimenzije osim prve):
```c
tip ime_fje(tip ime_niza[][dim2][dim3]...);
```
## Povratna vrednost

## Funkcije sa promenljivim brojem argumenata
