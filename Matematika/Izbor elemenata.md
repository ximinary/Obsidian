#fax #math #ds2 [deo [[Kombinatorika|kombinatorike]]]
$\:$

$n$ elemenata, $k$ mesta

|                              | (bez ponavljanja)     | sa ponavljanima |
| ---------------------------- | --------------------- |:--------------- |
| Varijacije (uređen izbor)    | $\frac{n!}{(n-k)!}\quad$ [[Izbor elemenata#(1) Uređen izbor elta\|(1)]]  | $n^k\quad$ [[Izbor elemenata#(2) Uređen izbor elta sa ponavljanima\|(2)]]      |
| Kombinacije (neuređen izbor) | $\binom{n}{k}=\frac{n!}{k!(n-k)!}\quad$ [[Izbor elemenata#(3) Neuređen izbor elta\|(3)]] | $\binom{n+k-1}{n}=\frac{(n+k-1)!}{n!(k-1)!}\quad$ [[Izbor elemenata#(4) Neuređen izbor elta sa ponavljanima\|(4)]]             |
| Permutacije                  |   $n! \quad (n=k)\quad$ [[Izbor elemenata#(5) Permutacije\|(5)]]              |$\binom{n}{n_{1},\,n_{2},\,\dots,\,n_{k}}$, gde je $n_{1}$ broj ponavljanja prvog elta,  $n_{2}$ broj ponavljanja drugog elta i td.$\quad$ [[Izbor elemenata#(6) Permutacije sa ponavljanima\|(6)]]                |

### (1) Uređen izbor elta
$f:\mathbb{N}_{k}\overset{1-1}\to\mathbb{N}_{n}$
Svakom preslikavanju $f$ odgovara jedan izbor elta, tako da je $i$-ti izabrani element je $f(i)$.
Stav. Broj preslikavanja $f:\mathbb{N}_{k}\overset{1-1}\to\mathbb{N}_{n}$ je $\prod\limits_{i=0}^{k-1}(n-i)$

### (2) Uređen izbor elta sa ponavljanima
$f:\mathbb{N}_{k}\to\mathbb{N}_{n}$
Svakom preslikavanju $f$ odgovara jedan izbor elta, tako da je $i$-ti izabrani element je $f(i)$.
Stav. Broj preslikavanja $f:\mathbb{N}_{k}\to\mathbb{N}_{n}$ je $n^{k}$

### (3) Neuređen izbor elta
Stav. Broj ovakvih izbora je jednak $\begin{align}\binom{n}{k}=\frac{n!}{k!(n-k)!}\end{align}$
(* [[Binomni koeficijenti|binomni koef.]])
> Dokaz: ima $\frac{n!}{(n-k)!}$ uređenih izbora, pri tome uređenih izbora, koji imaju po $k$ istih elemenata, ima $k!$ ([[Izbor elemenata#(5) Permutacije|permutacije]]). Odakle neuređenih izbora ima $k!$ puta manje.

### (4) Neuređen izbor elta sa ponavljanima
Stav. Broj ovakvih izbora je jednak $\begin{align}\binom{n+k-1}{k}=\frac{(n+k-1)!}{k!(n-1)!}\end{align}$
> Dokaz: Na $k$ mesta treba izabrati po nekoliko (od 0 do $k$) svakog od $n$ elemenata. To moguće predstaviti u sledećem obliku:
> $n-1$ *granica* između elemenata
> $k$ *markera*, svaki od kojih označava izabrani element
> > Na primer: biramo 5 elta iz skupa $\mathbb{N_{7}}$
> > $\begin{array}{c|c|c|c|c|c|c}
> > 1&2&3&4&5&6&7 \\
> > \hline
> > &.&&.\!.&.&&.
> > \end{array}$
> > $n=7,\ k=5$
> > Izabrano je $[2,\,4,\,4,\,5,\,7]$
> 
> Problem se svodi na [[Izbor elemenata#(3) Neuređen izbor elta|neuređeni izbor]] $k$ *markera* iz skupa *granica* i *markera*, tj. neuređeni izbor $k$ elemenata na $(n+k-1)$ mesta.
### (5) Permutacije
Broj permutacija je jednak broju uređenih izbora kad $k=n$,
tada $\frac{n!}{(n-k)!}=\frac{n!}{0!}=n!$
### (6) Permutacije sa ponavljanima
Teorema. Broj permutacija sa ponavljanjima multiskupa od $n$ elemenata u kojem 1. element pojavljuje $n_{1}$ puta, 2. — $n_2$ puta, $\dots$, $k$-ti — $n_{k}$ puta, a $n=n_{1}+n_{2}+\dots+n_{k}$ je $\begin{align}\binom{n}{n_{1},\,n_{2},\,\dots,\,n_{k}}\end{align}$ 
(* [[Multinomna formula|multinomni koef.]])
>Dokaz:
>Raspoređujemo 1. elementi — biramo $n_1$ elemenata od $n$.
>Raspoređujemo 2. elementi — biramo $n_2$ elemenata od $n - n_1$.
>$\dots$
>Na kraju dobijamo:
>$\begin{align}\binom{n}{n_{1}}\binom{n-n_{1}}{n_{2}}\dots\binom{n-n_{1}-n_{2}-\dots - n_{k-1}}{n_{k}}=\end{align}$
>$\begin{align}=\frac{n!}{n_{1}!\,\cancel{(n-n_{1})!}}\cdot\frac{\cancel{(n-n_{1})!}}{n_{2}!\,\cancel{(n-n_{̌1}-n_{2})}}\dots\frac{\cancel{(n-n_{1}-n_{2}-\dots - n_{k-1})!}}{n_{k}!\,(n-n_{1}-n_{2}-\dots - n_{k})!}=\end{align}$
>$\begin{align}=\frac{n!}{n_{1}!\,n_{2}!\,\dots\,n_{k}!\,\cancel{0!}}=\binom{n}{n_{1},\,n_{2},\,\dots,\,n_{k}}\end{align}$