#fax #cs/prog [deo [[Računarstvo|računarstva]]]
$\:$

Efikasnost algoritma:
- vremenska složenost
- memorijska (prostorna) složenost
$\:$
- za neku konkretnu ulaznu veličinu
- asimptotsko ponašanje kado veličina ulaza raste

### Merenje i procenjivanje resursa
— Merenje vremena (na primer, u C-u pomoću biblioteke [```<time.h>```](Standardne%20biblioteke%20(C).md)).

— Procenjivanje vremena, ako znamo prosečno vreme za izvršavanje operacija.

— Profajliranje
- analiza performansa programa;
- koliko puta je bila pozvana i koliko vremena je utrošila funkcija.

Sa ovim znanjem možemo da razumemo koje (najčešće korišćene i koje  najviše troše) funkcije treba da optimizujemo
### [[Asimptotske klase. Asimptotska relacija ekvivalencije|Asimptotsko]] ponašanje
- vreme izvršavanja — funkcija od broja argumenata
- analiza najgoreg slučaja

$f(n)$ — broj instrukcija za $n$ argumenata.

$\log n \ \ll\ n\ \ll\ n\,\log n\ \ll\ n^{k}\ \ll\ a^{n}\ \ll\ n!$, $\quad$ $a>1,\ k>0$
___
**Def**.  $f(n)=O\big(g(n)\big)\quad\Leftrightarrow\quad\exists c>0\ \ \exists N\ \ \forall n\geqslant N\ \ f(n) \leqslant c\,g(n)$

$O\big(g(n)\big)$ — klasa funkcija koje raste sporije od $g(n)$
___
**Def**.  $f(n)=\Omega\big(g(n)\big)\quad\Leftrightarrow\quad\exists c>0\ \ \exists N\ \ \forall n\geqslant N\ \ f(n) \geqslant c\,g(n)$

$O\big(g(n)\big)$ — klasa funkcija koje raste brže od $g(n)$
___
**Def**.  $f(n)=\Theta\big(g(n)\big)\quad\Leftrightarrow\quad\exists c_{1},\,c_{2}>0\ \ \exists N\ \ \forall n\geqslant N\ \ c_{1}\,g(n)\leqslant f(n) \leqslant c_{2}\,g(n)$

$\Theta\big(g(n)\big)$ — klasa funkcija koje raste slično kao i $g(n)$
___
**Teorema**. važi za $O$, $\Omega$ i $\Theta$:
1. $a\,f(n)+b=O\big(f(n)\big),\quad\forall a>0,\,b\in\mathbb{R}$
2. $f_{1}(n)=O\big(g_{1}(n)\big),\ \ f_{2}(n)=O\big(g(n)\big).$ Tada:
   - $f_{1}(n)+f_{2}(n)=O\big(g_{1}(n)+g_{2}(n)\big)$
   - $f_{1}(n)\cdot f_{2}(n)=O\big(g_{1}(n)\cdot g_{2}(n)\big)$
3. $f(n)=O\big(g(n)\big)\ \ \mathrm{i} \ \ g(n)=O\big(h(n)\big)\quad\Rightarrow\quad f(n)=O\big(h(n)\big)$
$\:$

**Teorema**.
1. $f(n)=\Theta\big(g(n)\big)\quad\Leftrightarrow\quad f(n)=O\big(g(n)\big)\ \ \mathrm{i}\ \ f(n)=\Omega\big(g(n)\big)$
2. $f(n)=O\big(g(n)\big)\quad\Leftrightarrow\quad g(n)=\Omega\big(f(n)\big)$
   Odakle:  $f(n)=\Theta\big(g(n)\big)\quad\Leftrightarrow\quad g(n)=\Theta\big(f(n)\big)$

Primeri:
- $1242352135=O(1)$
- $n^{2}=O(n^{2})$
- $5n^{2}+10=O(n^{2})$
- $n^{2}=O(n^{3}),\quad n^{2}=O(2^{n})$
- $7\cdot2^{n}+n=O(2^{n})$
- $3^{n}+2^{n}+n=O(3^{n})$
- $n\cdot 2^{n}+2^{n}+n^{123}=O(n\cdot2^{n})$
---
**Def**. $T(n)$ — vreme izvršavanja algoritma $A$ za ulaz veličine $n$, $T(n)=O\big(g(n)\big)$. Tada je algoritam $A$ složenosti (reda) $O\big(g(n)\big)$.

Složenost algoritama obično se izražava u terminima $O\big(g(n)\big)$, pri tome što se traži funkcija $g$ koja raste što sporije.
> Na primer, $T(n)=5n\,\log n+n^{3}+32$.
> Iako važi  i $\ \:T(n)=O(n^{3})\ \:$ i $\: \ T(n)=O(n^{35})\ \:$ i $\ \:T(n)=O(3^{n})$,
> Kažemo da je taj algoritam složenosti $O(n^{3})$.

Procenjivane u terminima $\Theta\big(g(n)\big)$ je preciznije ali nije uvek moguće.
> Na primer:
> Za neke ulaze $T(n)=n$, a za neke $T(n)=n^{2}$, tada algoritam nije ni složenosti $\Theta(n)$ ni $\Theta(n^{2})$, ali jeste složenosti $O(n^{2}).$

___
Složenost:
$O(1)$ — konstantna 
$O(\log n)$ — logaritamska
$O(n)$ — linearna
$O(n\,\log n)$ — kvazilinearna 
$O(n^{2})$ — kvadratna
$O(n^{3})$ — kubna
$O(n^{k})$ — polinomna $(k>0)$
$O(a^{n})$ — eksponencijalna $(a>1)$
___
Izračunavanje složenosti:
- Vremenska:
	- Naredbe bez petlji i poziva funkcija — $O(1)$
	- Blok složenosti $O(f)$ a posle blok $O(g)$ — $O(f+g)$
	- if (...) $O(f)$ else $O(g)$ — $O(f+g)$
	- petlja sa $n$ iteracija i $O(1)$ u telu — $O(n)$
	- petlja sa $n$ iteracija unutra petlji sa $m$ iteracija — $O(n\cdot m)$
- Prostorna:
	- bez poziva fja i dinamička alokacija — $O(1)$
	- alokacija $n$ elemenata složenosti $O(1)$ — $O(n)$
	- alokacija niza od $n$ elemenata $O(1)$ — $O(n)$
	- $n$ poziva fje složenosti $O(g)$ iz fje složenosti $O(f)$ — $O(f+g)$

___
Klasa $P$.
**Def**. Algoritam sa $n$ ulaza je polinomske složenosti ako $T(n)=O(n^{k})$ za neko $k\in\mathbb{R}$. 
Klasa problema za koje postoji algoritam sa $O(n^{k})$ označava se sa $P$.

Problem zadovoljivosti:
Da li je [[Iskazna logika#^f1f8bc|zadovoljiva]] data logička formula od $n$ primenljivih?
$2^{n}$ kombinacija  $\ \ \to\ \ O(2^{n})$.
Pripada li problem klasi $P$? Nema dokaza ni da pripada ni da ne pripada. ^ebfaa0

### Popravljanje složenosti
Vremenske:
- Naći delove (funkcije) koje dominantno utiču na složenost
- Prvo naći algoritam sa najboljim asimptotskim ponašanjem
- Kada je asimptotsko ponašanje najbolje, smanjiti broj naredbi
- Koristiti optimizaciju kompilatora
- Izdvojiti ponavljajući izvršavanja (izdvojiti što više moguće izvan petlji)
- \[Prioritet vreme]: Čuvati neka ponavljajuća izračunavanja

Prostorne:
- Najmanji mogući tipovi
- \[Prioritet memorija]: Ne čuvati stvari koje se lako računaju.