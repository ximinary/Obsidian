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

## Povratna vrednost

## Funkcije sa promenljivim brojem argumenata
