#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$

## Promenljive
- moraju biti deklarisane pre korišćenja.
- pridružen prostor u memoriji
- ime: prvi simbol \_ ili slovo, ostale \_, slova ili cifre

Deklaracija: 
```c
int a, b;
```
Deklaracija sa inicijalizacijom: 
```c
int a = 3;
```

Konstanta: 
```c
const double G = 9.81;
double const G = 9.81;
```

![[promenljive.png]]

## Tipovi podataka

**Celobrojne** tipovi u rastućem poretku prema dužine:
```c
short
int             # standardni tip
long         
long long
```
Dodatno pre tima moguće napisati:
```c
signed          # označeni - isto kao i ne pisati ništa
unsigned        # neoznačeni
```
$\:$

Tip za **karaktere**, ali u suštini <u>jednobitni</u> celobrojni tip:
```c
(signed/unsigned) char
```
$\:$

**Pokretan zarez** (IEEE754 standard - uklj. $+\infty,\ -\infty,\ \mathrm{sNaN},\ \mathrm{qNaN}$)
```c
float
double          # standardni tip
long double 
```
$\:$
Druge tipovi
```c
bool            # logički tip - true/false
void            # ništa
```

### Konstante i konstantne izrazi
Na primer: ```2, 207, 3.14, 1.4e6, '9', 034```

##### Celobrojne:
```c
12345   - int (-> long -> unsigned long) 
		  ## u zavisnosti od veličine broja
12345l  - long
12345L  - long long
12345u  - unsigned int
12345ul - unsigned long 
```
U oktalnom i heksadekadnom sistemu (moguće kombinovati sa ```l```, ```L```, ```u```, ... )
```c
056     - oktalni (int)
0x1f    - heksadekadni (int)
```

Negativne konstante ne postoje: koristi se unitarni operator ```-```.
Na primer ```-678```

##### U pokretnom zarezu:
```c
13.45   - double
1e-2    - double        # = 0.01
1.45e6  - double        # = 1450000.0
.3      - double        # = 0.3
2.      - double        # = 2.0

13.45f  - float         # (f ili F)
13.45l  - long double   # (l ili L)
```
Mogu biti i pozitivne i negativne .

##### Simboli (karakteri)
```c
'a'     - int           # = 97
'A'     - int           # = 65
'0'     - int           # = 48
```
Specijalni simboli:
```'\n'``` — new line
```'\t'``` — horizontal tab
```'\v'``` — vertical tab
```'\\'``` — ```\```
```'\?'``` — ```?```
```'\''``` — ```'```
```'\"'``` — ```"```
```'\012'``` — oktalni broj
```'\x12'``` — heksadekadni broj
```'\0'``` — vrednost $0$, kraj niske

##### Konstantne izrazi
Na primer: ```4 + 3 * 5```
Konstantne izrazi izračunavaju se tokom prevođenja programa.

## Operatori i izrazi
Arnost operatora — broj operanada na koje se pimenjuje.
- unarni
	- prefiksni (```-x```)
	- postfiksni (```x++```)
- binarni (```x + y```)
- ternarni (```x ? y : z```)
$\:$

Operatori nad brojevima:
- aritmetičke
- logičke
- relacijske

[[Prioritet operatora (C).png|Prioritet operatora]]
1. Unarni postfiksni pa unarni prefiksni pa binarni
2. Aritmetički pa relacijski pa logički
3. Kao u matematici: ```( )```, ```*``` i ```/``` i ```%```, ```+``` i ```-```
4. ```<``` i ```<=``` i ```>``` i ```>=``` pa ```==``` i ```!=```
5. Najmanji prioritet: ```? :``` pa dodele pa ```,```
$\:$

Asocijativnost operatora:
- leva: $x\ \overset{\mathrm{I}}/\ 10\ \overset{\mathrm{II}}/\ 20$
- desna: $x\ \overset{\mathrm{II}}=\ y\ \overset{\mathrm{I}}=\ 33$
- neasocijativan: zabranjeno uzastopnost ponavljanje.

##### Operator dodele ```=```
```c
x = ...;     # x je izmenjiva l-vrednost (promenljiva)
```
promena vrednosti objekata na levoj strani je sporedni efekat (side effect).

Ima desnu asocijativnost.

Dodela ima vrednost: 
```c
x = y = 3;  # y = 3 ima vrednost 3 koja se dodeljuje x-u
```

```c
int a;
double b = a = 3.5;
```
Prvo ```a```-u se dodeljuje vrednost ```3```;
```a = 3.5``` ima vrednost ```3```;
Posle ```b```-u se dodeljuje vrednost ```a = 3.5``` tj. ```3```;
Rezultat: ```a = 3; b = 3.0```

##### Aritmetičke operatori
```+``` — binarni operator sabiranja;
```-``` — binarni operator oduzimanja;
```*``` — binarni operator množenja;
```%``` — binarni operator ostatka pri deljenju (oba operanda celi);
```/``` — binarni operator:
- celobrojnog deljenja, ako su oba operanda celi;
- deljena, ako je bar jedan operand broj u pokretnom zarezu;


```+``` — unarni operator;
```-``` — unarni operator promene znaka;

*Svi  aritmetički operatori gore imaju levu asocijativnost, dole — desnu.*

```++``` — prefiksno ili postfiksno inkrementiranje;
```--``` — prefiksno ili postfiksno dekrementiranje;
```c
           i = 5;
I slučaj            II slučaj
x = i++;            x = ++i;
          Rezultat
i == 6              i == 6
x == 5              x == 6
```

```i++``` ima vrednost ```i``` do inkr.; $\ \ \ \ \ \ \ \quad$ ```i--``` ima vrednost ```i``` do dekr.;
```++i``` ima vrednost ```i``` posle inkr.; $\ \ \quad$ ```--i``` ima vrednost ```i``` posle dekr.

##### Relacijski operatori
```==``` — jednako;
```!=``` — različito;
```<``` — manje;
```<=``` — manje ili jednako;
```>``` — veće;
```>=``` — veće ili jednako;

Imaju levu asocijativnost.

Ako je tačno ima vrednost ```1``` (```int```).
Ako nije tačno ima vrednost ```0``` (```int```).

Na primer: $\underbrace{\underbrace{5 \ > \ 3}_{1}\ >\ 2}_{0}$

##### Logički operatori
```!``` — [[Logičke operacije#^b24d81|logičko ne]];
```&&``` — [[Logičke operacije#^96b28f|logičko i]];
```||``` — [[Logičke operacije#^66b381|logičko ili]];

Svaka ne-nula vrednost se računa kao```1```

Na primer:
- ```!0``` je ```1```; $\ \:$ ```!1``` je ```0```; $\ \:$ ```!9.2``` je ```0```;
- ```5 && 4.3``` je ```1```; $\ \:$ ```3.1 && 0``` je ```0```;
- ```10 || 0``` je ```1```; $\ \:$ ```0 || 0``` je ```0```.

> ##### Lenjo izračunavanja
> Sleva nadesno:
> U operatorima ```&&``` i ```||``` prvo se računa leva strana i ako rezultat ne zavisi od desne strane, desna strana i ne računa se.
> 
> Na primer:
> - $\underbrace{\underbrace{2\ <\ 1}_{0}\ \  \&\& \ \ a\!+\!+ }_{0}\quad\quad$ ($a\!+\!+$ neće biti uvršeno)
> - $a\!+\!+\ \ \&\&\ \ 2<1\ \ \quad\quad$ ($a\!+\!+$ sigurno će biti uvršeno)
> - $\underbrace{\underbrace{2\ >\ 1}_{1}\ \  || \ \ a\!+\!+ }_{1}\quad\quad\quad$ (slično $a\!+\!+$ neće biti uvršeno)
##### Bitovski operatori
```~``` — bitovska negacija;
```&``` — bitovsko i;
```|``` — bitovsko ili;
```^``` — bitovski **XOR**;
```<<``` — pomeranje bitova ulevo;
```>>``` — pomeranje bitova udesno;


```x << k``` — pomeranje bitova broja ```x``` sa ```k``` mesta ulevo.
```x >> k``` — pomeranje bitova broja ```x``` sa ```k``` mesta udesno:
- ako je ```x``` tipa ```int``` aritmetičko — na viši (oslobođeni) bitovi stavlja se bit znaka.
- ako je ```x``` tipa ```unsigned``` logičko — na viši (oslobođeni) bitovi stavlja se ```0```.

```x``` može biti konstanta ili promenljiva. ```<<``` i ```>>``` ne menjaju ```x```.
##### Složeni operatori dodele ```+=```, ```-=```, ```*=```, ```%=```, ```/=```, ```&=```, ```|=```, ```<<=```, ```>>=```

```izraz1 op= izraz2``` isto što i ```izraz1 = izraz1 op ipraz2```

##### Operator uslova ```izraz1 ? izraz2 : izraz3```

Prvo se izračunava ```izraz1```.
Ako je ne-nula, onda se izračunava ```izraz2``` i to je vrednost operatora.
Inače se izračunava ```izraz3``` i to je vrednost operatora.

##### Operator zarez ```,``` (u deklaraciji <u>nije</u> operator)
```c
for (i = 10, j = 0; i < j; i++, j--) { ...; }
```
ima najniži prioritet;
računaju se i leva i desna strana;
vrednost operatora je vrednost desne strane.

```x = 1, 2;``` je isto što i ```x = 2;```
```x = 3, y = 5;``` je isto što i ```x = 3; y = 5;```

##### Operator ```sizeof```
veličina tipa ili promenljive u bajtovima;
vrača vrednost tipa ```size_t``` (sličan sa ```unsigned```).
```c
double a;
size_t x = sizeof(a);
size_t y = sizeof(int);
```
## Konverzije tipova
— menja se tip izraza, ne menja se tip promenljivih.

- <u>Eksplicitna konverzija</u> (na zahtev programera)
  Operator kastovanja: ```(tip) izraz```
  — prefiksni unarni operator 
  $\:$
- <u>Implicitna konverzija</u> (izvršava se automatski po potrebi)
	
1. konverzija u tip leve strane:
```c
int a = 46;
double b;
b = a;          
## pre upisivanja vrednost a se konvertuje u double.
```

2. aritmetičke operatori se ne primenjuju na ```char``` i ```short```
```c
char a = 2, b = 3, c;
c = a + b; 
## vrednost a se konvertuje u int, vrednost b se konvertuje u int, računa se zbir, vrednost zbira se konvertuje u char i upisuje se u c.
```
3. aritmetički i logički operatori zahtevaju operandi u istom tipu, tako jedan od operanada se konvertuje u tip drugog, koji ima "bogatiji" tip.
```c
char a = 2; double b = 7.9; 
b = (a + 5.6f) / b;
## vrednost a se konvertuje u float, računa se zbir, vrednost zbira se konvertuje u double, računa se količnik i rezultat se upisuje u b.
```
$\:$

Promocija — konverzija u "bogatiji" tip — obično ne dolazi do gubitka.
*Na primer može doći do gubitka pri konverziji velikog broja tipa* ```long``` *u tip* ```double```*;*

Democija — konverzija u "siromašniji" tip — često dolazi do gubitka.
*Na primer pri konverziji broja tipa* ```double``` *ili* ```float``` *u tip* ```int``` *odsecaju se decimale*: ```int a = 8.31f``` — ```a``` *će dobiti vrednost* ```8```.

## Nizovi i niske
Deklaracija niza:
```c
tip ime_niza[dimenzija];
```
dimenzija mora da bude konstantan ceo broj;
na primer: ``````
ili 

## Korisnički definisane tipovi