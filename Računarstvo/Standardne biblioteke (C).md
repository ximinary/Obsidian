#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$

## Zaglavlje ```<string.h>>``` — rad sa niskama
```c
// dužina:
size_t strlen (const char* str);

// kopiranje:
char* strcpy (char* destination, const char* source);
char* strncpy (char* destination, const char* source,
size_t num);

// nadovezivanje:
char* strcat (char* destination, const char* source);
char* strncat (char* destination, const char* source,
size_t num);

// poredak: 
// -1 ako str1 leksikografski manje od str2 
// 0 ako su iste
// 1 ako str1 leksikografski veće od str2
int strcmp (const char* str1, const char* str2);
int strncmp (const char* str1, const char* str2,
size_t num);

// vraća pokazivač na prvo pojavljivane karaktera c u niski, NULL ako c nije u niski:
char* strchr (const char* str, int c);
// vraća pokazivač na poslednje pojavljivane karaktera c u niski, NULL ako c nije u niski:
char* strrchr (const char* str, int c);
// vraća pokazivač na na prvo pojavljivane nekog od karaktera niske str2 i niski str1, NULL ako nijedan karakter nije u niski:
char* strpbrk (char* str1, char* str2);
// vraća pokazivač na podnisku jednaku sa str2 u niski str1, NULL ako nije podniska:
char* strstr (const char* str1, const char* str2);

// dužina početnog dela str1 koji sadrži samo karaktere iz str2:
size_t strspn (const char* str1, const char* str2);
// dužina početnog dela str1 koji ne sadrži nijedan od karaktera iz str2:
size_t strcspn (const char* str1, const char* str2);

// deljenje niske str karakterima iz delimiters, korišćenje dole:
char* strtok (char* str, const char* delimiters);
```

```strtok```:
```c
char str[] ="- Ovo, je jedna niska.", delims[] = " ,.-";
char *s = strtok (str, delims);
while (s != NULL) {
	printf ("%s\n", s);
	s = strtok (NULL, delims);
}
```
ispis:
```
Ovo
je
jedna
niska
```

## Zaglavlje ```<stdlib.h>```
```c
// dinamička alokacija:
void *malloc(size_t n);
void *calloc(size_t n, size_t size);
void *realloc(void *memblock, size_t size);
void free(void* p);

int system(char* command);

// pseudo-slučajni brojevi:
int rand(void);
void srand(unsigned);

// zaustavljane programa:
void exit(int);

// konverzije:
double atof(const char *str); //str to double
int atoi(const char *str);    //str to int
long atol(const char *str);   //str to long

// konverzije:
// ako endptr nije NULL, stavlja *endptr na karakter posle pročitanog broja
double strtod(const char *str, char **endptr);
long strtol(const char *str, char **endptr, int base);
unsigned long strtoul(const char *str, char **endptr, int base);


// binarna pretraga:
void *bsearch(const void *key, const void *base, size_t nitems, size_t size, int (*compar)(const void *, const void *));

// sortiranje niza:
void qsort(void *base, size_t nitems, size_t size, int (*compar)(const void *, const void*));

// absolutna vrednost:
int abs(int x);
long labs(long x)
```

Funkcija ```int rand(void);``` generiše pseudo-slučajne cele brojeve u intervalu od ```0``` do ```RAND_MAX``` (definisana u zaglavlju)

Pseudo-slučajni brojevi u pokretnom zarezu iz intervala \[0, 1):
```c
((double)rand() / (RAND_MAX+1.0))
```
Pseudo-slučajni brojevi u  intervalu $[n,\,m]$:
```c
n + (m-n+1)*((double)rand() / (RAND_MAX + 1.0))
```

Funkcija ```rand``` niz pseudo-slučajnih brojeva generiše uvek počev od iste podrazumevane vrednosti (koja je jednaka 1). To znači da će se u svakom pokretanju programa dobiti isti niz pseudo-slučajnih brojeva. Funkcija ```void srand(unsigned);``` menja tu vrednost.
Za bilo koju vrednost funkcije ```srand```, niz brojeva koji vraća funkcija rand je uvek isti. 

Često se kao argument u pozivu funkcije ```srand``` navodi trenutno
vreme: ```srand(time(NULL))```, gde se koristi funkcija ```time``` iz zaglavlja ```<time.h>```, da bi se postiglo da se pri svakom pokretanju programa dobije različt niz vrednosti.

## Zaglavlje ```<assert.h>```
```c
void assert(int x);
```
Ako je ```x``` nula zaustavi program sa greškom:
```
Assertion failed: expression, file filename, line nnn
```
## Zaglavlje ```<ctype.h>```
```c
int isalpha(int c); // vraća ne-nulu ako je c slovo
int isdigit(int c); // cifra
int isalnum(int c); // cifra ili broj
int isspace(int c); // belina (razmak, tab, ...)
int isupper(int c); // veliko slovo
int islower(int c); // malo slovo
int toupper(int c); // vraća c, ako je c bio malo slovo, vraća veliko
int tolower(int c); // vraća c, ako je c bio veliko slovo, vraća malo
```

## Zaglavlje ```<math.h>```
```c
double sin(double); double asin(double);
double cos(double); double acos(double);
double tan(double); double atan(double);
double atan2(double, double);

double log(double);
double log10(double);
double log2(double);
double exp(double);
double pow(double, double);
double sqrt(double);
double fabs(double);
double floor(double);
double ceil(double);
double trunc(double);
double round(double).
```