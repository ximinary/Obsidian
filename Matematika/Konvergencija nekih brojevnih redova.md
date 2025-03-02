
#fax #math #a2 [deo poglavlja [[Brojevni red|"brojevni red"]]]
$\:$

**Stav**. $\begin{align}\sum\limits_{n=1}^{\infty} q^{n}=\begin{cases}\frac{q}{1-q},&\text{za }-1<q<1\\\\\text{divergira},&\text{za ostale } q\end{cases}\end{align}$ ^20d439

> Dokaz:
> za $q=1$ divergira jer $\lim\limits_{ n \to \infty }1^{n}=1\ne0$
> 
> za $q\ne1$
> $\begin{align}\sum\limits_{n=1}^{\infty} q^{n}=\lim\limits_{ n \to \infty }\sum\limits_{k=1}^{n}q^{k}=\lim\limits_{ n \to \infty }\big(q+q^{2}+\dots+q^{n}\big)=\lim\limits_{ n \to \infty }q\frac{1-q^{n}}{1-q}=(*)\end{align}$
> 
> Koristimo [[Osnovni limesi#^ff0b5b|limes]], tada $(*)=\begin{cases}+\infty,&q>1\\\frac{q}{1-q},&-1<q<1\\\not\exists,&q<-1\end{cases}$

$\:$
**Stav**. $\begin{align}\sum\limits_{n=1}^{\infty}\frac{1}{n}\quad\text{divergira} \end{align}$.
> Dokaz:
> Pokazati da divergira koristeći [[Kriterijumi konvergencije brojevnih redova#^f4afac|Košijev kriterijum]],
> tj. treba naći $\varepsilon>0$ tako da $\forall N\in\mathbb{N}\quad\exists m,\,k\geqslant N\quad|s_{m}-s_{k}|\geqslant\varepsilon$
>
> uzmemo $k = N+1$ i $m=2N$, tada
> $\begin{align}|s_{m}-s_{k}|=\sum\limits_{n=N+1}^{2N}\frac{1}{n}\geqslant\sum\limits_{n=N+1}^{2N}\frac{1}{2N}=\frac{N}{2N}=\frac{1}{2} \end{align}$
> $\begin{align}\varepsilon:=\frac{1}{2}\end{align}$

$\:$
**Stav**. $\begin{align}\sum\limits_{n=1}^{\infty}\frac{(-1)^{n-1}}{n}\quad\text{konvergira}\end{align}$.
> Dokaz:
> $\begin{align}a_{n}=\frac{1}{n}\end{align}$ je strogo opadajući niz i važi $\lim\limits_{ n \to \infty }a_{n}=0$. 
> Dakle, na osnovu [[Kriterijumi konvergencije brojevnih redova#^94970b|Lajbnicovog kriterijuma]] $\begin{align}\sum\limits_{n=1}^{\infty}\frac{(-1)^{n-1}}{n}\ \ \end{align}$ konvergira.

$\:$
**Stav**. $\begin{align}\sum\limits_{n=1}^{\infty}\frac{1}{n^{2}}\quad\text{konvergira} \end{align}$.
> Dokaz: $\begin{align}\forall n\geqslant2\quad\frac{1}{n^{2}}\leqslant\frac{1}{n(n-1)}\quad\quad\ \ \ (1)\end{align}$
> 
> Razmotrimo konvergenciju reda $\begin{align}\sum\limits_{n=2}^{\infty} \frac{1}{n(n-1)} \end{align}$
> Njegova parcijalna suma: $\begin{align}\sigma_{n}=\sum\limits_{k=2}^{n}\frac{1}{k(k-1)}=\sum\limits_{k=2}^{n}\Big(\frac{1}{k-1}-\frac{1}{k}\Big)=1-\frac{1}{n}\end{align}$
> Odakle $\begin{align}\sum\limits_{n=2}^{\infty} \frac{1}{n(n-1)}=\lim\limits_{ n \to \infty }\sigma_{n}=1\end{align}$ 
> tj. red $\begin{align}\sum\limits_{n=2}^{\infty} \frac{1}{n(n-1)}\ \ \end{align}$ konvergira. $\quad\quad(2)$
> 
> Na osnovu $(1)$, $(2)$ i [[Kriterijumi konvergencije brojevnih redova#^4d14b2|teoreme]] red $\begin{align}\sum\limits_{n=1}^{\infty} \frac{1}{n^{2}}\ \ \end{align}$ konvergira  

$\:$
**Stav**. $\begin{align}\sum\limits_{n=1}^{\infty}\frac{1}{\sqrt[]{n}}\quad\text{divergira} \end{align}$.
> Dokaz: 
$\begin{align}\sum\limits_{n=1}^{\infty}\frac{1}{\sqrt[]{n}}=\lim\limits_{ n \to \infty }s_{n}=\lim\limits_{ n \to \infty }\sum\limits_{k=1}^{n} \frac{1}{\sqrt[]{k}} \end{align}$
>
>$\begin{align}s_{n}=\sum\limits_{k=1}^{n} \frac{1}{\sqrt[]{k}}\geqslant\sum\limits_{k=1}^{n} \frac{1}{\sqrt[]{n}} =\frac{n}{\sqrt[]{n}}=\sqrt[]{n}\end{align}$
>
>$\lim\limits_{ n \to \infty }\sqrt[]{n}=+\infty\quad\Rightarrow\quad\lim\limits_{ n \to \infty }s_{n}=+\infty$
>
>Stoga, $\begin{align}\sum\limits_{n=1}^{\infty} \frac{1}{\sqrt[]{n}}\ \ \end{align}$ divergira

$\:$
**Stav**. $\begin{align}\sum\limits_{n=1}^{\infty} \frac{1}{n^{\alpha}}\end{align}$ $\quad$ konvergira za $\alpha>1$, divergira za $\alpha\leqslant1$
