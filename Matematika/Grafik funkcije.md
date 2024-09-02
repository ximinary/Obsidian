#fax #math #a1 [deo [[Analiza|analize]]]
$\:$

# Ispitivanje toka i skiciranje grafika funkcije $f(x)$

### 1) Domen $D_{f}$
### 2) Znak i nule
$f$ je pozitivna na intervalu $A$, ako $\forall x\in A\quad f(x)>0$
$f$ je negativna na intervalu $A$, ako $\forall x\in A\quad f(x)<0$

Nule su rešenja jednačine $f(x)=0$

Ako nemoguće rešiti (ne)jednačine preskočiti.
### 3) Svojstva
- $f$ je periodična ako $\exists T\in\mathbb{R}\ :\ \forall x\in \mathbb{R}\quad f(x)=f(x+T)$
- $f$ je parna ako $\forall x\in D_{f}\quad f(-x)=f(x)$
- $f$ je neparna ako $\forall x\in D_{f}\quad f(-x)=-f(x)$

Može biti ni parna ni neparna, može biti periodična i parna, i td.

### 4) [[Neprekidnost]]

Sve osnovne funkcije su neprekidne, kao i njihov zbir, proizvod i kompozicija.

Treba proveriti granične tačke intervala u funkciji datoj sa vitičastom zagradom.
> Na primer:
> $f(x)=\begin{cases} |x|,\ \mathrm{ako}\ x\in[-1,\,1]\cup(2,\,5]\\ 4x^{2},\ \mathrm{ako}\ x\in(1,\,2]\\5,\ \mathrm{ako}\ x\in(5,\,+\infty)\end{cases}$
> Treba proveriti tačke: $-1,\,1,\,2,\,5$

Za svaku takvu tačku $a$ treba naći $\lim\limits_{ x \to a^{-} }f(x)=L$ i $\lim\limits_{ x \to a^{+} }f(x)=D$ ako to ima smisla. (U primeru fja nije zadata levo od $-1$, onda ne razmatramo $L$)
Ako $L=f(a)=D$ (ili samo $f(a)=D$, ako $L$ nema smisla ili samo $L=f(a)$, ako $D$ nema smisla), onda je $f$ neprekidna u $a$.

Ako  $L\ne f(a)$ ili $f(a)\ne D$ onda $f$ nije neprekidna u $a$


### 5) [[Izvod|Diferencijabilnost]]

Funkcija $f$ može biti diferencijabilna u $a$ samo ako je neprekidna u $a$.

Razdvojiti na slučajeve u $f$ kad je modul nenegativan i kad je negativan za svaki modul. 
>Nastavljamo primer:
>$f(x)=\begin{cases} -x,\ \mathrm{ako}\ x\in[-1,\,0)\\x,\ \mathrm{ako}\ x\in[0,\,1]\cup(2,\,5]\\ 4x^{2},\ \mathrm{ako}\ x\in(1,\,2]\\5,\ \mathrm{ako}\ x\in(5,\,+\infty)\end{cases}$


Naći izvod za svaki slučaj **na otvorenom delu svakog intervala**.
>Nastavljamo primer:
>$f'(x)=\begin{cases} -1,\ \mathrm{ako}\ x\in(-1,\,0)\\1,\ \mathrm{ako}\ x\in(0,\,1)\cup(2,\,5)\\ 8x,\ \mathrm{ako}\ x\in(1,\,2)\\0,\ \mathrm{ako}\ x\in(5,\,+\infty)\end{cases}$

Svaku graničnu tačku $a$ razmatramo odvojeno:
1. $f$ nije neprekidna u $a$ $\ \ \Rightarrow\ \:$ $f$ nije diferencijabilna u $a$ 
2. $f'_{-}(a)=f'_{+}(a)\ \ \Rightarrow\ \ f$ je diferencijabilna u $a$
3. Ako $\nexists f'_{-}(a)\:$ ili $\:\nexists f'_{+}(a)\:$ ili $\:f'_{-}(a)\ne f'_{+}(a)$
   treba tražiti izvod po definicije:
   Ako $\begin{align}\exists\lim\limits_{ h \to 0^{-} }\frac{f(a+h)-f(a)}{h}=L\in\mathbb{R}\end{align},$
   $\begin{align}\exists\lim\limits_{ h \to 0^{+} }\frac{f(a+h)-f(a)}{h}=D\in\mathbb{R} \quad \mathrm{i}\quad L=D\end{align}$, onda je $f$ diferencijabilna u $a$ inače nije diferencijabilna u $a$.

### 6) [[Teoreme o srednjoj vrednosti#^9f49d5|Intervale monotonosti]] i [[Ekstremum. Nužni i dovoljni uslov ekstremuma|ekstremumi]]

$f$ raste na  intervalu $A$, ako $\forall x\in A\quad f'(x)>0$
$f$ opada na  intervalu $A$, ako $\forall x\in A\quad f'(x)<0$

Razmatramo sve tačke $a$ u kojih važi $f'(a)=0$
Ako u levoj okolini tačke $a$ $f$ raste, u desnoj opada i $f(a)\in\mathbb{R}$, onda je $a$ maksimum.
Ako u levoj okolini tačke $a$ $f$ opada, u desnoj raste i $f(a)\in\mathbb{R}$, onda je $a$ minimum.

### -) Dodatno pronalaženje nula ako je bio preskočen deo 2):
Ako je $f$ neprekidna i monotona na intervalu $[a,\,b]$ i $f(a)\cdot f(b) <0$ onda postoji jedinstvena nula $c$ na intervalu $[a,\,b]$.
 
Razmatramo svaki interval monotonosti tako što gledamo da li su odgovarajući ekstremumi (ili uzimamo slučajne tačke na intervalu) različitog znaka, ako jesu postoji jedinstvena nula.

### 7) [[Konveksnost i konkavnost|Konveksnost/konkavnost i prevojne tačke]]

Tražimo $f''(x)$

$f$ je konveksna na  intervalu $A$, ako $\forall x\in A\quad f''(x)>0$
$f$ je konkavna na  intervalu $A$, ako $\forall x\in A\quad f''(x)<0$

Razmatramo sve tačke $a$ u kojih važi $f''(a)=0$
Ako je u levoj okolini tačke $a$ $f$ konveksna (konkavna), u desnoj okolini konkavna (konveksna) i $f(a)\in\mathbb{R}$, onda je $a$ prevojna tačka.

### 8) [[Asimptota|Asimptote]]
- Vertikalne: proveravamo sve $a\notin D_{f}$ — tačke nagomilavanja $D_{f}$.
Ako $\lim\limits_{ x \to a^{-} }f(x)=\pm\infty\ \:$ ili $\:\ \lim\limits_{ x \to a^{+} }f(x)=\pm\infty$ onda je $x=a$ vertikalna asimptota.
$\:$
- Kose kod $+\infty$ i $-\infty$ su oblika $y= k\,x+n$
(Ako $\nexists k$ ili $\nexists n$ onda $\nexists\:$ asimptota)
  - Tražimo $k$ i $n$ direktno:
$\begin{align}k =\lim\limits_{ x \to \pm\infty }\frac{f(x)}{x}\end{align}$
$n=\lim\limits_{ x \to \pm\infty}\big(f(x)-k\,x\big)$

  - Ili pomoću Tejlorovog polinoma (obično zamenom $t=\frac{1}{x}$):
$\begin{align}f(x)=k\,x+n+\frac{m}{x},\quad x\to\pm\infty\end{align}$,
gde ako $\begin{align}\frac{m}{x}>0\end{align}$ $\:$ $f$ prolazi iznad asimptote,
ako $\begin{align}\frac{m}{x}<0\end{align}$ $\:$ $f$ prolazi ispod asimptote
