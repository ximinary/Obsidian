#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$

Sve funkcije su u zaglavlju ```<stdio.h>```

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
int putchar(int c);  // ispisuje jedan karakter na standardni izlaz i vraća taj karakter ili EOF ako je došlo do grške 
```

##### Linijski ulaz i izlaz
```c
char* gets(char* s);  // !!! ne gledajući na dužinu niske !!! upisuje u s liniju sa ulaza do EOF ili '\n', umesto kojih stavi '\0', vraća s ili NULL ako nije uspelo (U slučaju greške ne menja s)
```

```c
int puts(const char* s);  // ispisuje nisku s na standardni izlaz, na kraju umesto '\0' ispisuje '\n'. Ako nije uspelo vraća EOF, inače drugu vrednost
```
##### Formatirani izlaz — ```printf```
```c
int printf(const char *format, ...);
```
— vraća broj odštampanih karaktera.

```format``` niska sadrži obične karaktere za štampanje kao i specifikacije konverzija za argumente ```...```; jednom argumentu odgovara zapis redom:
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
![[karakteri konverzije printf.png]]

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
```c
int scanf(const char *format, ...);
```
— vraća broj uspešnih dodeljivanja, ```EOF``` u slučaju kraja ulaza.

```format``` niska sadrži obične karaktere, koje se ignorišu, razmake za ignorisanje razmaka na ulazu pri korišćenju ```%c```,  kao i specifikacije konverzija za argumente ```...```, argumente su uvek pokazivači; jednom argumentu odgovara zapis redom:
- ```%``` $\ \ \ \:$ — $\:$  (obavezan)
- ```*``` $\ \ \ \:$  — $\:$ čitanje bez dodeljivanja; bez argumenta
- broj $\:$ — $\:$ dužina za čitanje
- modifikator
- karakter konverzije (obavezan)

Karakteri konverzije:
![[karakteri konverzije scanf.png]]
Modifikatori se podudaraju sa ```printf```.

## Ulaz iz niske i izlaz u nisku
```c
int sprintf(char* out_string, const char *format, ...);
```
— u nisku ```out_string``` upisuje isto što bi bilo ispisano ```printf```-om na standardni izlaz.

```c
int sscanf(char* in_string, const char *format, ...);
```
— iz niske ```in_string``` čita tako kako bi ```scanf``` pročitao sa standardnog ulaza.
## Ulaz iz datoteka i izlaz u datoteke
##### Pristupanje datoteci
```c
FILE* fopen(const char* filename, const char* mode);
```
— vraća pokazivač na strukturu ```FILE```, u koja sadrži informacije o fajlu, u slučaju greške vraća ```NULL```.

```filename``` — niska koja sadrži ime datoteke.
```mode``` — način otvaranja datoteke:
- ```"r"``` — čitanje
- ```"w"``` — pisanje (brišu se prethodne podatke)
- ```"a"``` — dopisivanje (pisanje posle već postojećih podataka)
- dodavanjem ```'+'``` u nisku omogućava se i čitanje i pisanje
- dodavanjem ```'b'``` u nisku datoteka se otvara kao binarna.

Treba uvek proveravati da li je dobro otvorio fajl, tj. da li pokazivač nije ```NULL```.

```c
int fclose(FILE* fp);
```
— zatvaranje fajla; treba uvek zatvarati fajl za obezbeđivanje podataka.

---
```c
FILE* stdin;  // datoteka standardnog ulaza
FILE* stdout; // datoteka standardnog izlaza
FILE* stderr; // datoteka standardnog izlaza za greške
```

##### Ulaz i izlaz pojedinačnih karaktera
```c
int getc(FILE* fp);  // vraća po 1 karakter iz fp, EOF (=-1) na kraju datoteke
```

```c
int putc(int c, FILE* fp);  // upisuje jedan karakter u datoteku i vraća taj karakter ili EOF ako je došlo do grške 
```

```c
int unget(int c, FILE* fp);  // "vraća" karakter c u datoteku (ne menja datoteku), sledeći getc će njega pročitati 
```

##### Provera grešaka i kraja datoteke
```c
int feof(FILE* fp);   // vraća ne-nulu ako je došlo do kraja datoteke 
```

```c
int ferror(FILE* fp); // vraća ne-nulu ako je došlo do greške sa datotekom
```
##### Linijski ulaz i izlaz
```c
char* fgets(char* s, int n, FILE* fp);  // upisuje u s liniju iz datoteke do EOF ili '\n' dužine najviše (n-1), na krraju stavi '\0', vraća s ili NULL ako nije uspelo (U slučaju greške ne menja s)
```

```c
int fputs(const char* s, FILE* fp);  // upisuje nisku s u datoteku, na kraju umesto '\0' ispisuje '\n'. Ako nije uspelo vraća EOF, inače drugu vrednost
```

##### [[Dinamička alokacija memorije (C)|Alokacija]] prostora za ulaznu liniju
```c
size_t getline(char** paloc_linija, int* n, FILE* fp);
```
```paloc_linija``` — pokazivač na pokazivač koji pokazuje na početak niske (alociranog bloka), u prvi poziv pokazuje na ```NULL```,
```n``` — pokazivač na broj — za koliko karaktera je alocirano memorije.

```getline``` čita liniju iz datoteke i upisuje u nisku ```*paloc_linija``` ako je moguće ili (re)alocira memoriju i upisuje.

Korišćenje:
```c
char *linija = NULL;
int n = 0;
getline(&linija, &n, file);    // čitanje prve linije
...
getline(&linija, &n, file);    // čitanje druge linije
...
free(linija);                  // !!!
```
##### Formatirani ulaz i izlaz
```c
int fprintf(FILE* fp, const char *format, ...);
```


```c
int fscanf(FILE* fp, const char *format, ...);
```
## [[Funkcije (C)#Argumenti funkcije ```main```|Argumente komandne linije]]