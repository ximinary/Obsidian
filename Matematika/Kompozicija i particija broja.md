#fax #math #ds2 [deo [[Kombinatorika|kombinatorike]]]


### Kompozicija broja
**Def**. Kompozicija broja $n\in\mathbb{N}$ na $k\in\mathbb{N}$ sabiraka je uređena $k$-torka $(a_{1},\,a_{2},\,\dots,\,a_{k})$ prirodnih brojeva takva da $n=a_{1}+a_{2}+\dots+a_{k}$

> Primer: $n=4$
> $k=1\ \:$ — $\:\ (4)$
> $k=2\ \:$ — $\:\ (1,\,3),\ (2,\,2),\ (3,\,1)$
> $k=3\ \:$ — $\:\ (1,\,1,\,2),\ (1,\,2,\,1),\ (2,\,1,\,1)$
> $k=4\ \:$ — $\:\ (1,\,1,\,1,\,1)$
> Ukupno: $\boxed{8}$

Teorema. Broj kompozicija broja $n$ na $k$ sabiraka iz $\mathbb{N}$ je $\begin{align}\binom{n-1}{k-1}\end{align}$
> Dokaz: $\underbrace{1\,\_\,1\,\_\,1\,\_\,\dots\,\_\,1\,\_\,1}_{n\ \mathrm{jedinica}}$
> Treba rasporediti $k-1$ pluseva na $n-1$ mesta. To moguće uraditi na $\begin{align}\binom{n-1}{k-1}\end{align}$ načina

Teorema. Broj kompozicija broja $n$ je $2^{n-1}$.
> Dokaz: $\begin{align}\sum\limits_{k=1}^{n}\binom{n-1}{k-1}=2^{n-1}\end{align}$


### Particija broja
**Def**. Particija broja $n\in\mathbb{N}$ na $k\in\mathbb{N}$ sabiraka je multiskup *(dozvoljeno ponavljanje, redosled nije bitan)* $[a_{1},\,a_{2},\,\dots,\,a_{k}]$ prirodnih brojeva takav da $n=a_{1}+a_{2}+\dots+a_{k}$

> Primer: $n=4$
> $k=1\ \:$ — $\:\ [4]$
> $k=2\ \:$ — $\:\ [1,\,3],\ [2,\,2]$
> $k=3\ \:$ — $\:\ [1,\,1,\,2]$
> $k=4\ \:$ — $\:\ [1,\,1,\,1,\,1]$
> Ukupno: $\boxed{5}$

Broj particija broja $n$ na $k$ sabiraka iz $\mathbb{N}$: $\ \ P_{k}(n)$
Broj particija broja $n$: $\ \ P(n)$

Niz particija brojeva:

$\begin{array}{c|c}
n &1&2&3&4&5&6&7&8&\dots\\
\hline
P(n) &1&2&3&5&7&11&15&22&\dots
\end{array}$

Teorema. $\begin{align}P_{k}(n+k)=\sum\limits_{i=1}^{k}P_{i}(n)\end{align}$

> Dokaz:
> $n+k=a_{1}+a_{2}+\dots+ a_{k}$
> $\quad \ \ \ n= \underbrace{(a_{1}-1)+(a_{2}-1)+\dots+(a_{k}-1)}_{=\,i\,\leqslant\, k \ \mathrm{sabiraka\ (od\ 0\ do\ k-1 \ postali\ nula)}}$
### Ferersov dijagram
**Def**. Ferersov dijagram neke particije broja $n$ na $k$ sabiraka sastoji od $n$ markera raspoređenih u vrste tako da svakoj vrsti odgovara jedan sabirak $a_{i}$ i ona sadrži $a_{i}$ markera. Vrste uređene opadajuće po broju markera.
> Primer: $10=5+2+2+1\quad\to\quad \begin{flalign}&\cdot\ \cdot\ \cdot\ \cdot\ \ \cdot&&\\&\cdot\ \ \cdot&&\\&\cdot\ \ \cdot&&\\&\ \cdot&&\end{flalign}$

**Def**. Dve particije su **konjugovane** (jedna u odnosu na drugu) ako jedna se dobija zamenom mesta vrsta i kolona drugoj.

> Primer:
> $10=5+2+2+1 \quad\quad\quad\quad\ \ \ 10=4+3+1+1+1$
> $\begin{flalign}
> &\cdot\ \cdot\ \cdot\ \cdot\ \cdot\ \quad\quad\quad\quad\quad\quad\quad\quad\cdot\ \cdot\ \cdot\ \ \cdot&&\\
> &\cdot\ \cdot\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\,\,\ \!\!\quad \cdot\  \cdot\ \ \cdot&&\\
> &\cdot\ \cdot\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\ \ \cdot&&\\
> &\cdot\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\ \ \cdot&&\\
> &\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\  \cdot&&
> \end{flalign}$

**Def**. Particija je **samokonjugovana** ako je konjugovana samoj sebi.

[[FerersoviDijagrami.png|Teorema]]. Važe identiteti: 
1. $P_{\leqslant k}(n)=P(n+k)$
2. $P_{\leqslant k}(n)=P(n,\ \mathrm{sabirci\ iz}\ \mathbb{N}_{k})$
3. $P(n,\ \mathrm{sabirci\ parni})=P(n,\ \mathrm{svaki\ sabirak\ pnavljuje\ parni\ broj\ puta})$
4. $P(n,\ \mathrm{samokonjugovana})=P(n,\ \mathrm{sabirci\ različiti\ i\ neparni})$