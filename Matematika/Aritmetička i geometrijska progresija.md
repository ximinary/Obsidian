#fax #math [deo poglavlja [[Niz brojeva|"niz brojeva"]]] 

### Aritmetički niz
$a_{1}$ — prvi član
$a_{n+1} = a_{n}+d,\quad \forall n\in \mathbb{N}$

odakle važe:
- $a_{n+1} = a_{1} + n\,d$
- $a_{n}-a_{m}= (m-n)\,d$

Zbir prvih $n$ članova:
$\begin{align}S_{n}=\sum\limits_{k=1}^{n}a_{k}=\frac{a_{1}+a_{n}}{2}\cdot n=\bigg(a_{1}+\frac{(n-1)\,d}{2}\bigg)\cdot n\end{align}$

### Geometrijski niz
$b_{1}$ — prvi član
$b_{n+1} = q\,b_{n},\quad \forall n\in \mathbb{N}, \ \ q\ne1$

odakle važe:
- $b_{n+1} = q^{n}\,b_{1}$
- $\begin{align}\frac{b_{n}}{b_{m}}= q^{n-m}\end{align}$

Zbir prvih $n$ članova:
$\begin{align}S_{n}=\sum\limits_{k=1}^{n}b_{k}=b_{1}\cdot\sum\limits_{k=1}^{n}q^{k-1}\xlongequal{\text{dokaz dole}} b_{1}\cdot\frac{q^{n}-1}{q-1}\end{align}$

> $\begin{align}1+q+q^{2}+\dots+q^{n-1}\overset{?}{=}\frac{q^{n}-1}{q-1}\end{align}$
> $(1+q+q^{2}+\dots+q^{n-1})(q-1)\overset{?}{=}q^{n}-1$
> $(q+q^{2}+q^{3}+\dots+q^{n})-(1+q+q^{2}+\dots+q^{n-1})\overset{?}{=}q^{n}-1$
> $q^{n}-1=q^{n}-1$

Zbir celog niza ako $-1<q<1$:
$\begin{align}S_{\infty}=\sum\limits_{k=1}^{\infty}b_{k}=b_{1}\cdot\sum\limits_{k=1}^{\infty}q^{k} \xlongequal{\text{dokaz dole}} \frac{b_{1}}{1-q} \end{align}$

> $\begin{align}1+q+q^{2}+\dots+q^{k}+\dots=\end{align}$
> $\begin{align}(1+q+q^{2}+\dots+q^{k}+\dots)\frac{1-q}{1-q}=\end{align}$
>$\begin{align}=\frac{(1-\cancel{q})+(\cancel{q}-\cancel{q^{2}})+(\cancel{q^{2}}-\cancel{q^{3}})+\dots+(\cancel{q^{k}}-\cancel{q^{k+1}})+\dots}{1-q}=\end{align}$
>$\begin{align}=\frac{1}{1-q}\end{align}$

^adeab1

