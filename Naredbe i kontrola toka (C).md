#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$
Program je niz naredbi.
## Naredbi izraza i blokovi
Svaki izraz završeni sa ```;``` je naredba.
Naredba ima smisla samo ako ima sporedni efekat.
Postoji prazna naredba: ```;```

Više naredba grupisanih u blok tretiraju se kao jedna.
Unutra bloka mogu da se deklarišu promenljivi koji ne mogu se koristiti van bloka. 
**Blok**:
```c
{
	...;     // neke naredbe
	...;     // neke naredbe
}            // posle } ne treba ;
```


## Uslovi
##### ```if - else```
```c
if (izraz)
	naredba1;
else                                // opcioni deo
	naredba2;
```
Ako je ```izraz``` ne-nula izvršiće ```naredba1```;
ako je ```izraz``` nula izvršiće ```naredba2```;

Umesto ```naredba1``` i ```naredba2``` mogu se koristiti blokovi.

Konstrukcija ```else if```:
```c
if (izraz1)
	naredba1;
else if (izraz2)
	naredba2;
else if (izraz3)
	naredba3;
else
	naredba4;
```

U sledećem primeru ```else``` se odnosi na drugi ```if```:
```c
if (izraz1)
	if (izraz2)
		naredba1;
	else
		naredba2;
```

Da bi odnosio na prvi ```if```:
```c
if (izraz1) {
	if (izraz2)
		naredba1;
} else
	naredba2;
```
##### ```switch```
```c
switch (izraz) {
	case konst_izraz1 : naredbe1;
	case konst_izraz2 : naredbe2;
	...
	default : naredbeN;             // opcioni deo
}
```

Ako ```izraz``` je jednak nekom ```konst_inrazK```, onda će biti izvršene sve naredbe ```naredbeK```, ```naredbe(K+1)```, ..., ```naredbeN``` do kraja ```switch```, ili do prvog ```break```;
ako ```izraz``` nije jednak nijednom ```konst_inrazK```, biće izvršene samo ```naredbeN```;

Posle ```:``` moguće napisati koliko god naredbi bez ```{ }```.

Često se koristi ovako:
```c
switch (izraz) {
	case konst_izraz1 : naredbe1; break;
	case konst_izraz2 : naredbe2; break;
	...
	default : naredbeN;             // opcioni deo
}
```
U ovom slučaju ako ```izraz``` je jednak nekom ```konst_inrazK```, onda će biti izvršene samo ```naredbeK```;
ako ```izraz``` nije jednak nijednom ```konst_inrazK```, biće izvršene ```naredbeN```;

Primeri:
```c
switch (n % 4) {
	case 1 :
	case 2 :
	case 3 : printf("Nije deljiv sa 4\n"); break;
	default : printf("Deljiv je sa 4\n");
}
```
```c
switch (dan) {
	case 1 : printf("Ponedeljak\n"); break;
	case 2 : printf("Utorak\n"); break;
	case 3 : printf("Sreda\n"); break;
	case 4 : printf("Četvrtak\n"); break;
	case 5 : printf("Petak\n"); break;
	case 6 : printf("Subota\n"); break;
	case 7 : printf("Nedelja\n"); break;
	default : printf("greška\n");
}
```

## Petlje
##### ```while```
```c
while (izraz)
	naredba;
```
Dok ```izraz``` nije nula, izvršava se ```naredba```. Kad ```izraz``` postaje nula, izlazi iz petlji i nastavlja sa izvršavanjem programa.

Beskonačna petlja:
```c
while (1) 
	naredba;
```
##### ```for```
```c
for (izraz1; izraz2; izraz3) 
	naredba;
```
```izraz1``` — inicijalizacija: početni vrednosti promenljivih;
```izraz2``` — uslov;
```izraz3``` — korak;

Ekvivalentna je sa:
```c
izraz1;
while (izraz2) {
	naredba;
	izraz3;
}
```
$\:$
```for ( ; izraz2; )``` $\quad\Leftrightarrow\quad$ ```while (izraz2)```
```for ( ; ; )``` $\quad\quad\quad\quad\ \!\!\Leftrightarrow\quad$ ```while (1)```

Operator ```,``` može da se koristi u ```izra1``` i ```izraz3```

Primeri:
```c
for (i = 0; i < n; i++);
```
```c
for (i = 0, j = 10; i < j; i++, j--);
```
##### ```do - while```
```c
do { 
	naredbe;
} while (izraz);
```
Ekvivalentna je sa:
```c
naredbe;
while (izraz)
	naredbe;
```
##### Naredbe ```break``` i ```continue```


dejstvuju samo na unutrašnju petlju.
