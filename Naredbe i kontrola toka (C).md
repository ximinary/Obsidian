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
else                   // opcioni deo
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

##### ```switch```

## Petlje
##### ```while```

##### ```for```

##### ```do - while```

##### Naredbe ```break``` i ```continue```