#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$

## Standardni tokovi
Fajlovi standardnog ulaza, izlaza i izlaza za greške pri pokretanju programa:
```
./prog < infile
./prog > outfile
./prog 2> errorfile
```
##### Ulaz i izlaz pojedinačnih karaktera
```c
int getchar(void);  // vraća po 1 karakter sa ulaza, EOF (=-1) na kraju ulaza
```

```c
int putchar(int);  // ispisuje jedan karakter na standardni izlaz i vraća taj karakter ili EOF ako je došlo da grške 
```

##### Linijski ulaz i izlaz
```c
char* gets(char* s);  // !!! ne gledajući na dužinu niske !!! upisuje u s liniju sa ulaza do EOF ili '\n', umesko kojih stavi '\0', vraća s ili NULL ako nije uspelo
```

```c
int puts(const char* s)  // ispisuje nisku s na standardni izlaz, na kraju umesto '\0' ispisuje '\n'. Ako nije uspelo vraća EOF, inače drugu vrednost
```
##### Formatirani izlaz — ```printf```
```c
int printf(const char *format, ...);
```
— vraća broj odštampanih karaktera.

```format``` niska sadrži obične karaktere za štampanje kao i specifikacije konverzija za argumente ```...```; jednom argumentu odgovara zapis:
- ```%``` $\ \ \ \:$ — $\:$  (obavezan)
- ```-``` $\ \ \ \:$ — $\:$ levo poravnanje
- broj $\:$ — $\:$ najmanja dužina polja za argument
- ```.```
- broj $\:$ — $\:$ niske: najmanji broj karaktera
  $\quad\quad\quad\quad$ pokretan zarez: broj decimala posle tačke
  $\quad\quad\quad\quad$ celi: najmanji broj cifara
  ili ```*``` $\,$  — $\:$ preciznost u odvojenom argumentu tipa ```int```
  $\quad\quad\quad\quad$  (primer dole)
- modifikator
- karakter konverzije (obavezan)

Karakteri konverzije:
![[karakteri konverzije (C).png]]

Modifikatori:
- ```h``` — ```short``` — ```%hd```
- ```l``` — ```long``` — ```%ld```
- ```L``` — ```long double``` i ```long long``` — ```Lf``` i ```Ld```

**!** ```float``` se implicitno konvertuje u ```double```

```*``` - argument:
```c
pritntf("%.*s", max, s); // odštampa najviše max karaktera niske s
```

##### Formatirani ulaz — ```scanf```