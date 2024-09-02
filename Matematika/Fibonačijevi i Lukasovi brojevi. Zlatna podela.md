#fax #math #ds2 [deo [[Kombinatorika|kombinatorike]]]
$\:$
### Zlatna podela
![[zlatna podela.png]]
$\begin{align}\frac{a+b}{a}=\frac{a}{b}\end{align}$

>$b:=1$
>$\begin{align}\frac{a+1}{a}=a\end{align}$
>$a^{2}-a-1=0$
>$\begin{align}a_{1,2}=\frac{1\pm\sqrt{5}}{2}\end{align}$
>$\begin{align}a=\frac{1+\sqrt{ 5 }}{2}\approx1,681\end{align}$

$\begin{align}\frac{a+b}{a}=\frac{a}{b}=\frac{1+\sqrt{5}}{2}\end{align}$

### Fibonačijev [[Rekurentna jednačina|niz]]
$\begin{cases}F_{n+2}=F_{n+1}+F_{n}\\F_{0}=0,\ \ F_{1}=1\end{cases}$

$0,\,1,\,1,\,2,\,3,\,5,\,8,\,13,\,21,\,\dots$

[[Fib1.png|Teorema]]. Opšti član Fibonačijevog niza je
$\begin{align}F_{n}=\frac{\left(\frac{1+\sqrt{5}}{2}\right)^{n}-\left(\frac{1-\sqrt{5}}{2}\right)^{n}}{\sqrt{5}}=\left[\frac{\left(\frac{1+\sqrt{5}}{2}\right)^{n}}{\sqrt[]{5}}\right]\end{align}$, 
(gde je $[\ ]$ zaokruživanje na najbliži ceo broj)

[[Fib2.png|Teorema]]. Funkcija generatrisa Fibonačijevog niza je $\begin{align}F(x)=\frac{x}{1-x-x^{2}}\end{align}$

[[Fib3.png|Teorema]]. Važe jednakosti:
1. $\begin{align}\frac{F_{n+1}}{F_{n}}=\underset{(n-1\ \mathrm{pluseva})}{\underbrace{1+\frac{1}{1+\frac{1}{1+\frac{1}{1+\frac{1}{1+\dots_{\frac{1}{1+1}}}}}}}_{n}}\end{align}\:\:\:\:,$ $\quad\quad$ $n\geqslant1$
2. $\begin{align}\lim\limits_{ n \to \infty }\frac{F_{n+1}}{F_{n}}=\frac{1+\sqrt[]{5}}{2}\end{align}$
3. $\begin{align}\sum\limits_{i=0}^{n}F_{i}=F_{n+2}-1\end{align}$
4. $F_{n-1}\,F_{n+1}-F_{n}^{2}=(-1)^{n},\quad n  \geqslant1$

### Lukasov [[Rekurentna jednačina|niz]]
$\begin{cases}L_{n+2}=L_{n+1}+L_{n}\\L_{0}=2,\ \ L_{1}=1\end{cases}$

$2,\,1,\,3,\,4,\,7,\,11,\,18,\,29,\,\dots$

[[Luk1.png|Teorema]]. Opšti član Lukasovog niza je
$\begin{align}L_{n}=\left(\frac{1+\sqrt{5}}{2}\right)^{n}+\left(\frac{1-\sqrt{5}}{2}\right)^{n}\end{align}$

[[Luk2.png|Teorema]]. Funkcija generatrisa Lukasovog niza je $\begin{align}L(x)=\frac{2-x}{1-x-x^{2}}\end{align}$

[[FibLuk.png|Teorema]]. Važi $L_{n}=F_{n-1}+F_{n+1},\quad n\geqslant1$

### Tribonačijev [[Rekurentna jednačina|niz]]
$\begin{cases}T_{n+3}=T_{n+2}+T_{n+1}+T_{n}\\T_{0}=T_{1}=0,\ \ T_{2}=1\end{cases}$

### Katalanovi brojevi
$\begin{cases}C_{n+1}=\sum\limits_{i=0}^{n}C_{i}\,C_{n-i}\\C_{0}=1\end{cases}$

$1,\,1,\,2,\,5,\,14,\,42,\,132,\,\dots$

$\begin{align}C_{n}=\frac{1}{n+1}\binom{2n}{n}\end{align}$

[[Katalan.png|Teorema]].