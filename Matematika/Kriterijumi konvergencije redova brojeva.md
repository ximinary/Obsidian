#fax #math #a2 [deo poglavlja [[Red brojeva|"red brojeva"]]]
$\:$

**Teorema** (Košijev kriterijum). Neka je $(a_{n})$ niz. Tada
$\begin{align}\sum\limits_{n=1}^{\infty}a_{n}\quad\text{konvergira}\quad\Leftrightarrow\quad\forall\varepsilon>0\quad \exists N\in\mathbb{N}\quad \forall m,\,k\geqslant N\quad\left|s_{m}-s_{k}\right|<\varepsilon\end{align}$ ^f4afac
> Dokaz: tvrđenje direktno sledi iz [[Košijev niz|teoreme: niz konvergira akko je Košijev]].

$\:$
**Stav**. Neka su $(a_{n})$ i $(b_{n})$ su nizovi, i $\exists N\in\mathbb{N}\quad \forall n\geqslant N\quad \boxed{|a_{n}|\leqslant b_{n}}$. Tada
$\begin{align}\sum\limits_{n=1}^{\infty}b_{n}\quad\text{konvergira}\quad\Rightarrow\quad\sum\limits_{n=1}^{\infty}a_{n}\quad\text{konvergira}\end{align}$ ^9d13dd
> Dokaz:
> Neka je $\forall n\in\mathbb{N}\quad\begin{align}s_{n}=\sum\limits_{k=1}^{n}b_{n}\end{align}$ parcijalna suma reda $\begin{align}\sum\limits_{n=1}^{\infty} b_{n}\end{align}$ 
> i neka je $\begin{align}\forall n\in\mathbb{N}\quad\sigma_{n}=\sum\limits_{k=1}^{n}a_{n}\end{align}$ parcijalna suma reda $\begin{align}\sum\limits_{n=1}^{\infty} a_{n}\end{align}$.
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
**Teorema** (posledica stava). Neka su $(a_{n})$ i $(b_{n})$ su nizovi, i $\exists N\in\mathbb{N}\quad \forall n\geqslant N\quad \boxed{0\leqslant a_{n}\leqslant b_{n}}$. Tada ^4d14b2
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

**Teorema** (Dalamberov kriterijum). Neka je $(a_{n})$ niz takav da $\forall n\in\mathbb{N}\quad a_{n}>0$ $\ \:$ i $\ \:$ $\begin{align}\exists \lim\limits_{ n \to \infty }\frac{a_{n+1}}{a_{n}}=A\in[0,\,+\infty]\end{align}$. Tada ^cf63a2
- Ako $0\leqslant A<1$ onda $\begin{align}\sum\limits_{n=1}^{\infty} a_{n}\ \ \text{konvergira}\end{align}$
- Ako $A>1$ onda $\begin{align}\sum\limits_{n=1}^{\infty} a_{n}\ \ \text{divergira}\end{align}$

> Dokaz:
> $\begin{align}\exists \lim\limits_{ n \to \infty }\frac{a_{n+1}}{a_{n}}=A\quad \Leftrightarrow\quad \forall\varepsilon>0\quad \exists N\in\mathbb{N}\quad\forall n\geqslant N\quad &\frac{a_{n+1}}{a_{n}}\in\mathrm{O}_{\varepsilon}(A)\\\text{za }A\in\mathbb{R}\quad&A-\varepsilon<\frac{a_{n+1}}{a_{n}}< A+\varepsilon\\\text{za }A=+\infty\quad&\frac{a_{n+1}}{a_{n}}>\frac{1}{\varepsilon}\end{align}$
>
>Prvo tvrđenje.
> Definišemo $q:=A+\varepsilon$, pri tome uzimamo $\varepsilon$ tako da $0<q<1$, što je moguće jer $0\leqslant A<1$. Tada
> $\exists N\in\mathbb{N}\quad\forall n\geqslant N\quad a_{n+1}<q\,a_{n}$
>
>$\begin{array}{l}\text{za }N&a_{N+1}< q\,a_{N}\\\text{za }N+1&a_{N+2}< q\,a_{N+1}< q^{2}\,a_{N}\\\dots\\\text{za }n-1&a_{n}< q\,a_{n-1}<\dots<q^{n-N}a_{N}\end{array}$
>
>Odakle, $\forall n\geqslant N\quad a_{n}\leqslant q^{n-N}a_{N}\quad\quad(1)$
>
>Red $\begin{align}\sum\limits_{n=N+1}^{\infty} q^{n-N}a_{N}=a_{N}\sum\limits_{n=1}^{\infty}q^{n}\end{align}$ [[Konvergencija nekih redova#^20d439|konvergira]] za $0<q<1$
> 
> Iz (1) i jer $\begin{align}\sum\limits_{n=N+1}^{\infty} q^{n-N}a_{n}\ \ \text{konvergira}\end{align}$ na osnovu [[Kriterijumi konvergencije redova brojeva#^4d14b2|teoreme]] važi da $\begin{align}\sum\limits_{n=N+1}^{\infty} a_{n}\ \ \text{konvergira}\end{align}$, odakle na osnovu [[Red brojeva#^6bf0d1|stava]] $\begin{align}\sum\limits_{n=1}^{\infty} a_{n}\ \ \text{konvergira}\end{align}$.
> $\:$
>
> Drugo tvrđenje.
> Definišemo $q:=\begin{cases}A-\varepsilon&\text{za }1<A<+\infty\\\frac{1}{\varepsilon}&\text{za }A=+\infty\end{cases}$, pri tome uzimamo $\varepsilon$ tako da $q>1$. Tada slično kao u prvom tvrđenju dobijamo
> $\exists N\in\mathbb{N}\quad\forall n\geqslant N\quad a_{n}\geqslant\,q^{n-N}\,a_{N}\quad\quad(2)$
> 
> Red $\begin{align}\sum\limits_{n=N+1}^{\infty} q^{n-N}a_{N}=a_{N}\sum\limits_{n=1}^{\infty}q^{n}\end{align}$ [[Konvergencija nekih redova#^20d439|divergira]] za $q>1$
> 
> Iz (2) i jer $\begin{align}\sum\limits_{n=N+1}^{\infty} q^{n-N}a_{n}\ \ \text{divergira}\end{align}$ na osnovu [[Kriterijumi konvergencije redova brojeva#^4d14b2|teoreme]] važi da $\begin{align}\sum\limits_{n=N+1}^{\infty} a_{n}\ \ \text{divergira}\end{align}$, odakle na osnovu [[Red brojeva#^6bf0d1|stava]] $\begin{align}\sum\limits_{n=1}^{\infty} a_{n}\ \ \text{divergira}\end{align}$.

$\:$
**Teorema** (Košijev koreni kriterijum). Neka je $(a_{n})$ niz takav da $\forall n\in\mathbb{N}\quad a_{n}\geqslant0$ $\ \:$ i $\ \:$ $\begin{align}\exists \lim\limits_{ n \to \infty }\sqrt[n]{a_{n}}=A\in[0,\,+\infty]\end{align}$. Tada ^d13f64
- Ako $0\leqslant A<1$ onda $\begin{align}\sum\limits_{n=1}^{\infty} a_{n}\ \ \text{konvergira}\end{align}$
- Ako $A>1$ onda $\begin{align}\sum\limits_{n=1}^{\infty} a_{n}\ \ \text{divergira}\end{align}$

> Dokaz je sličan dokazu prethodne teoreme.

$\:$
**Teorema** (konvergencija reda i nesvojstvenog integrala). 
Neka je $f:\ [1,\,+\infty)\to[0,\,+\infty)$ neprekidna opadajuća funkcija.
Tada $\begin{align}\sum\limits_{n=1}^{\infty} f(n)\ \ \text{konvergira}\quad\Leftrightarrow\quad\int_{1}^{+\infty} f(x) \, dx\ \ \text{konvergira}\end{align}$
> Dokaz:
> $\begin{align}\forall n\in\mathbb{N}\quad f(n)\leqslant\int_{n}^{n+1} f(x) \, dx \leqslant f(n+1) \end{align}$
> $\begin{align}f(2)+f(3)+\dots+f(n)\leqslant\int_{1}^{n} f(x) \, dx \leqslant f(1)+f(2)+\dots+f(n-1)\end{align}$
> $\begin{align}s_{n}-f(1)\leqslant\int_{1}^{n} f(x) \, dx \leqslant s_{n-1}\end{align}$
> 
> Odakle, 
> $\begin{align}\int_{1}^{n} f(x) \, dx \leqslant s_{n-1}\quad\quad\quad\quad\quad\quad\,(1)\end{align}$
> $\begin{align}s_{n}\leqslant\int_{1}^{n} f(x) \, dx+f(1)\quad\quad\quad\quad(2)\end{align}$
> 
> $\boxed{\Rightarrow}$ 
> Jer $\begin{align}\sum\limits_{n=1}^{\infty}f(n)\ \ \text{konvergira}\end{align}$ i $(s_{n})$ je rastući niz, taj niz je ograničen odozgo.
 Odakle koristeći $(1)$ fja $\begin{align}\int_{1}^{n} f(x) \, dx \end{align}$ ograničena je odozgo i jer je ona rastuća, $\begin{align}\exists\lim\limits_{ x \to +\infty }\int_{1}^{n} f(x) \, dx=\int_{1}^{+\infty} f(x) \, dx\in\mathbb{R} \quad\end{align}$ (tj. integral konvergira)
 >
 >$\boxed{\Leftarrow}$ 
> Jer $\begin{align}\int_{1}^{+\infty} f(x) \, dx\ \ \text{konvergira}\end{align}$ i $\begin{align}\int_{1}^{n} f(x) \, dx \end{align}$ je rastuća fja, ta fja je ograničena odozgo.
 Odakle koristeći $(2)$  niz $(s_{n})$ ograničen odozgo i jer je on rastući, $\begin{align}\exists\lim\limits_{ n \to +\infty }\sum\limits_{k=1}^{n}f(k)=\sum\limits_{n=1}^{\infty}f(n) \in\mathbb{R} \quad\end{align}$ (tj. red konvergira)

$\:$
**Stav** (Lajbnicov kriterijum). Neka je $(a_{n})$ strogo opadajući niz takav da $\lim\limits_{ n \to \infty }a_{n}= 0$. Tada $\begin{align}S=\sum\limits_{n=1}^{\infty} (-1)^{n-1}a_{n}\ \ \text{konvergira}\end{align}$ i važi $0<S \leqslant a_{1}$. ^94970b
> Dokaz: Neka je $\begin{align}s_{n}=\sum\limits_{k=1}^{n}(-1)^{n-1}a_{n}\end{align}$ niz parcijalnih suma.
>
> Sa jedne strane,
> $s_{2n}=(a_{1}-a_{2})+(a_{3}-a_{4})+\dots+(a_{2n-1}-a_{2n})$
> Odakle, jer je $(a_{n})$ opadajući važi da je $(s_{n})$ rastući
>
>Sa druge strane,
> $s_{2n}=a_{1}-\underbrace{(a_{2}-a_{3})}_{\geqslant0}-\underbrace{(a_{4}-a_{5})}_{\geqslant0}-\dots-\underbrace{(a_{2n-2}-a_{2n-1})}_{\geqslant0}-\underbrace{a_{2n}}_{\geqslant0}$
> Važi $\forall n\in\mathbb{N}\quad s_{2n}\leqslant a_{1}$
> 
> $(s_{2n})$ je ograničeni i rastući niz $\quad\Rightarrow\quad$ $\exists\lim\limits_{ n \to \infty }s_{2n}=S\in\mathbb{R}$
> 
> $s_{2n-1}=a_{1}-a_{2}+\dots+a_{2n-1}+(-s_{2n}+s_{2n})=s_{2n}+a_{2n}$
> $\lim\limits_{ n \to \infty }s_{2n-1}=\lim\limits_{ n \to \infty }(s_{2n}+a_{2n})=\lim\limits_{ n \to \infty }s_{2n}+\lim\limits_{ n \to \infty }s_{2n}=S+0=S$
> 
> Konačno, $\lim\limits_{ n \to \infty }s_{n}=S$
> i jer $\forall n\in\mathbb{N} \quad0\leqslant a_{n}\leqslant a_{1}$ važi i $0\leqslant S\leqslant a_{1}$