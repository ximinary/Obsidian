#fax #math #ds2 [deo [[Kombinatorika|kombinatorike]]]
$\:$
[[binomnaFormula.png|Teorema]] (Binomna formula). $x,\,y \in \mathbb{R},\,n\in \mathbb{N}_{0}$. Tada 
$$
(x+y)^{n}=\sum_{k=0}^{n}\binom{n}{k}x^{k}\,y^{n-k}
$$

Posledice:
- $\begin{align}\sum\limits_{k=0}^{n}\binom{n}{k}(-1)^{k}=0\end{align}$
- $\begin{align}\sum\limits_{k=0}^{n}\binom{n}{k}=2^{n}\end{align}$

### Specijalni slučaj za celobrojne koeficijenti

- Za $|x|< 1$ važi
  $\begin{align}1+x+x^{2}+\dots+x^{k}+\dots=\frac{1}{1-x}\end{align}\quad$ ([[Aritmetička i geometrijska progresija#^adeab1|*]])

Lema. $n,\,k\in \mathbb{N}$. Koeficijent uz $x^{k}$ u $(1+x+x^{2}+\dots+x^{k}+\dots)^{n}$ je $\begin{align}\binom{n+k-1}{k}\end{align}$
> Dokaz:
> $\underbrace{(1+x+x^{2}+\dots)\,(1+x+x^{2}+\dots)\dots(1+x+x^{2}+\dots)}_{n}$
> Pitanje je na koliko načina možemo izabrati po jedan sabirak iz svakog faktora tako da proizvod bude $x^{k}$
> Neka je $a_{m}$ stepen sabirka izabranog iz $m$-toj faktora.
> Tada zadatak se svodi na pronalaženje svih rešenja jednačine $a_{1}+a_{2}+\dots+a_{n}=k$ u skupu $\mathbb{N}_{0}$.
> Rešiti jednačinu znači rastaviti $(n-1)$ granicu (*granica je znak +*) između $k$ markera.
> To moguće uraditi na $\begin{align}\binom{n+k-1}{k}\end{align}$ načina. ([[Izbor elemenata#(4) Neuređen izbor elta sa ponavljanima|**]])
> 


Lema. $|x|<1, \ \ n,\, k\in \mathbb{N}$. Koeficijent uz $x^{k}$ u $(1+x)^{-n}$ je $\begin{align}\binom{-n}{k}\end{align}$
> Dokaz: smena $x=-t$
> $(1+x)^{-n} = (1-t)^{-n}\overset{(*)}{=}(1+t+t^{2}+\dots+t^{k}+\dots)^{n}$
> Iz prethodne leme koef. uz $t^{n}$ je $\begin{align}\binom{n+k-1}{k}\end{align}$
> $x^{k}=(-1)^{k}t^{k}$, znači koef. uz $x^{k}$ je koef. uz $t^{k}$ pomnožen sa $(-1)^{k}$ 
> tj. koef. uz $x^{k}$ je $\begin{align}(-1)^{k}\binom{n+k-1}{k}=\binom{-n}{k}\end{align}\quad$ ([[Binomni koeficijenti#^37ae6b|***]])

Teorema (Specijalni slučaj binomne formule za celobrojne koeficijenti). 
$|x|<1,\ \ n \in \mathbb{Z}$. Tada $\begin{align}(1+x)^{n}=\sum\limits_{k=0}^{\infty}\binom{n}{k}x^{k}\end{align}$
>Dokaz:
>$n\in \mathbb{N}_{0}$ — binomna formula
>$n\in \mathbb{Z}\setminus\mathbb{N}_{0}$ — iz prethodne leme