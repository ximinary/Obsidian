#fax #cs/prog [deo [[Programski jezik C|jezika C]]]
$\:$

### Promenljive
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

### Tipovi podataka

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

Celobrojne:
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

Negativne konstante ne postoje:koristi se unitarni operator ```-```.
Na primer ```-678```