#fax #math #ds1 [deo poglavlja [[Prirodni brojevi|"prirodni brojevi"]] i [[Celi brojevi|"celi brojevi"]]]
$\:$

[[eukl alg t1.png|Teorema]]. Ako je $a = b\cdot q + r\:$, tada važi $\mathrm{NZD}(a,\,b) = \mathrm{NZD}(b,\,r)$
(Napomena: [[Euklidsko deljenje|euklidsko deljenje]], [[Deljivost#Zajednički delilac i zajednički sadržalac|NZD]]) ^4496b1

### Algoritam
$a, b \in \mathbb{N}, \ \ b \ne 0$
Primena teoreme odogo više puta dok ostatak neće postati 0:
$a = b\cdot q_{1} + r_{1}\quad\quad\quad\quad\quad\quad 0< r_{1}<b$
$b = r_{1}\cdot q_{2} + r_{2}\quad\quad\quad\quad\quad\ \ \, 0< r_{2}<r_{1}$
$r_{1} = r_{2}\cdot q_{3} + r_{3}\quad\quad\quad\quad\quad\ 0< r_{3}<r_{2}$
$\dots$
$r_{n-3} = r_{n-2}\cdot q_{n-1} +r_{n-1}\quad\ 0< r_{n-1}<r_{r-2}$
$r_{n-2} = r_{n-1}\cdot q_{n} +r_{n}\quad\quad\quad\!\ 0< r_{n}<r_{r-1}$
$r_{n-1} = r_{n}\cdot q_{n+1} \quad\quad\quad\quad\quad\ r_{n+1}=0$

Teorema. Poslednji nenula ostatak u Euklidovom algoritmu $r_{n}$ je jednak $\mathrm{NZD}(a,\,b)$.
> Dokaz:
> Iz teoreme:
> $\mathrm{NZD}(a,\,b) = \mathrm{NZD}(b,\,r_1) = \mathrm{NZD}(r_1,\,r_2) = \dots = \mathrm{NZD}(r_{n-2},\,r_{n-1}) = \mathrm{NZD}(r_{n-1},\,r_{n})$
> Poslednja jednčina: $r_{n-1} = r_{n}\cdot q_{n+1} \ \ \Rightarrow\ \ r_{n}\,|\,r_{n-1}\ \ \Rightarrow\ \ \mathrm{NZD}(r_{n-1},\,r_{n}) = r_{n}$

$\:$
[[eukl alg posl.png|Posledica]].$\ \forall a,\,b\in \mathbb{N}\ \ \ \exists p,\,q \in \mathbb{Z}\ \ : \ \ a\cdot p + b\cdot q = \mathrm{NZD}(a,\,b)$ ^e5f1a9

[[eukl alg primer.png|Primer]]

### Matrična metoda
$M_0=\left[\begin{array}{c|c c} 
	a & 1 & 0\\ 
	b & 0 & 1 
\end{array}\right]$

Operacije
- T1: zamena mesta vrsta
- T2: množenje vrsta sa -1
- T3: dodavanje jedne vrste pomnožene celim brojem drugoj vrsti.

Matrica $M_n=\left[\begin{array}{c|c c} 
	x & p & q\\ 
	y & r & s 
\end{array}\right]$ se dobija primenom T1, T2, T3

[[eukl alg matr 1.png|Teorema]]. Za $M_{n}$ važi $\begin{cases} x = a\cdot p + b \cdot q\\ y = a\cdot r + b \cdot s \end{cases}$

[[eukl alg matr 2.png|Teorema]]. Za $M_{n}$ važi $\mathrm{NZD}(a,\, b) = \mathrm{NZD}(x,\,y)$

$\:$
Primenom T1, T2, T3 iz matrice $\left[\begin{array}{c|c c} 
	a & 1 & 0\\ 
	b & 0 & 1 
\end{array}\right]$ treba dobiti matricu oblika $
\left[\begin{array}{c|c c} 
	d & p & q\\ 
	0 & p' & q' 
\end{array}\right]$, tada je $d=\mathrm{NZD}(a,\,b)$ i $d=a\cdot p + b\cdot q$
[[eukl alg matr primer.png|Primer]]