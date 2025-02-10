#fax #math #a1 [deo poglavlja [[Red brojeva|"red brojeva"]]]
$\:$

**Teorema** (Košijev kriterijum). Neka je $(a_{n})$ niz. Tada
$\begin{align}\sum\limits_{n=1}^{\infty}a_{n}\quad\text{konvergira}\quad\Leftrightarrow\quad\forall\varepsilon>0\quad \exists N\in\mathbb{N}\quad \forall m,\,k\geqslant N\quad\left|s_{m}-s_{k}\right|<\varepsilon\end{align}$
> Dokaz: tvrđenje direktno sledi iz [[Košijev niz|teoreme: niz konvergira akko je Košijev]].

$\:$
**Stav**. Neka su $(a_{n})$ i $(b_{n})$ su nizovi, i $\exists N\in\mathbb{N}\quad \forall n\geqslant N\quad \boxed{|a_{n}|\leqslant b_{n}}$. Tada
$\begin{align}\sum\limits_{n=1}^{\infty}b_{n}\quad\text{konvergira}\quad\Rightarrow\quad\sum\limits_{n=1}^{\infty}a_{n}\quad\text{konvergira}\end{align}$ ^9d13dd
> Dokaz:
> Neka je $\forall n\in\mathbb{N}\quad\begin{align}s_{n}=\sum\limits_{k=1}^{n}b_{n}\end{align}$ parcijalna suma za niz $(b_{n})$ 
> i neka je $\begin{align}\forall n\in\mathbb{N}\quad\sigma_{n}=\sum\limits_{k=1}^{n}a_{n}\end{align}$ parcijalna suma za niz $(a_{n})$.
>
> Iz Košijevog kriterijuma:
> $\begin{align}\sum\limits_{n=1}^{\infty}b_{n}\quad\text{konvergira}\quad\Rightarrow\quad\forall\varepsilon>0\quad \exists N_{1}\in\mathbb{N}\quad \forall m,\,k\geqslant N_{1}\quad\left|s_{m}-s_{k}\right|<\varepsilon\end{align}$
> 
> pretpostavimo da je $m>k$ (za $m<k$ je analogno).
> 
> $\begin{align}&|\sigma_{m}-\sigma_{k}|=|a_{k+1}+a_{k+2}+\dots+a_{m}|\leqslant|a_{k+1}|+|a_{k+2}|+\dots+|a_{m}|\leqslant\\&\leqslant b_{k+1}+b_{k+2}+\dots+b_{m}= s_{m}-s_{k}<\varepsilon\end{align}$
> 
> Konačno:
> $\begin{align}\forall\varepsilon>0\quad \exists N_{2}:=\max\{N,\,N_{1}\}\quad \forall m,\,k\geqslant N_{2}\quad\left|\sigma_{m}-\sigma_{k}\right|<\varepsilon\quad\Rightarrow\end{align}$
> $\begin{align}\Rightarrow\quad\sum\limits_{n=1}^{\infty}a_{n}\quad\text{konvergira}\end{align}$

$\:$
**Teorema** (posledica stava). Neka su $(a_{n})$ i $(b_{n})$ su nizovi, i $\exists N\in\mathbb{N}\quad \forall n\geqslant N\quad \boxed{0\leqslant a_{n}\leqslant b_{n}}$. Tada
- $\begin{align}\sum\limits_{n=1}^{\infty}b_{n}\ \ \text{konvergira}\quad\Rightarrow\quad\sum\limits_{n=1}^{\infty}a_{n}\ \ \text{konvergira}\end{align}$
- $\begin{align}\sum\limits_{n=1}^{\infty}a_{n}\ \ \text{divergira}\quad\Rightarrow\quad\sum\limits_{n=1}^{\infty}b_{n}\ \ \text{divergira}\end{align}$

$\:$
**Teorema**.  Neka su $(a_{n})$ i $(b_{n})$ su nizovi, $\ \:$  $\forall n\in\mathbb{N}\quad a_{n},\,b_{n}>0$ $\ \:$ i $\ \:$ $\begin{align}\exists\lim\limits_{ n \to \infty }\frac{a_{n}}{b_{n}}=A\end{align}$. Tada 
- Ako je $A=0$ onda $\begin{align}\sum\limits_{n=1}^{\infty}b_{n}\ \ \text{konvergira}\quad\Rightarrow\quad\sum\limits_{n=1}^{\infty}a_{n}\ \ \text{konvergira}\end{align}$
- Ako je $a = +\infty$ onda $\begin{align}\sum\limits_{n=1}^{\infty}a_{n}\ \ \text{konvergira}\quad\Rightarrow\quad\sum\limits_{n=1}^{\infty}b_{n}\ \ \text{konvergira}\end{align}$
- Ako je $0<A<+\infty$ onda su $\begin{align}\sum\limits_{n=1}^{\infty}a_{n}\end{align}$ i $\begin{align}\sum\limits_{n=1}^{\infty}b_{n}\end{align}$ ekvikonvergentni
(tj. ili oba konvergiraju ili oba divergiraju).

> Dokaz:
> Prvo tvrđenje.
>>$\begin{align}\lim\limits_{ n \to \infty }\frac{a_{n}}{b_{n}}=0\quad\Rightarrow\quad\forall\varepsilon>0\quad\exists N\in\mathbb{N}\quad\forall n\geqslant N\quad\left|\frac{a_{n}}{b_{n}}\right|<\varepsilon\end{align}$
>> Uzimamo $\varepsilon = 1$ i jer su nizovi pozitivne  važi $\exists N\in\mathbb{N}\quad\forall n\geqslant N\quad a_{n}<b_{n}$
>> i iz prethodne teoreme slede tvrđenje.
> 
> Drogo tvrđenje dobijamo iz prvog zamenom mesta $a_{n}$ i $b_{n}$.
> Treće tvrđenje.
>>$\begin{align}\lim\limits_{ n \to \infty }\frac{f(x)}{g(x)}=A\quad\Rightarrow\quad\forall\varepsilon>0\quad\exists N\in\mathbb{N}\quad\forall n\geqslant N\quad&\left|\frac{a_{n}}{b_{n}}-A\right|<\varepsilon\\&A-\varepsilon<\frac{a_{n}}{b_{n}}< A+\varepsilon\end{align}$
>>
>>Iz pozitivnosti nizova i koristeći prethodnu teoremu dobijamo:
>> 1. Uzimamo $\varepsilon = \varepsilon_{1}$ tada važi 
>>  $\exists N\in\mathbb{N}\quad\forall n\geqslant N\quad a_{n}<(A+\varepsilon_{1})\cdot b_{n}$
>> Odakle ako $\begin{align}\sum\limits_{k=1}^{n} (A+\varepsilon_{1})b_{n} = (A+\varepsilon_{1})\sum\limits_{k=1}^{n} b_{n}\end{align}$ konvergira onda i $\begin{align}\sum\limits_{k=1}^{n} a_{n}\end{align}$ konvergira
>> 2. Uzimamo $\varepsilon = \varepsilon_{2} < A$ tada važi 
>>  $\begin{align}\exists N\in\mathbb{N}\quad\forall n\geqslant N\quad b_{n}<\frac{a_{n}}{A-\varepsilon_{2}}\end{align}$
>> Odakle ako $\begin{align}\sum\limits_{k=1}^{n}\frac{a_{n}}{A-\varepsilon_{2}} = \frac{1}{A-\varepsilon_{2}}\sum\limits_{k=1}^{n} a_{n}\end{align}$ konvergira onda i $\begin{align}\sum\limits_{k=1}^{n}b_{n}\end{align}$ konvergira

___

