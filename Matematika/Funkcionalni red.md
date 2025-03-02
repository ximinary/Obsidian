#fax #math #a2 [deo [[Analiza|analize]]]
$\:$

**Def**. Neka je $f_{n}:\ A\to\mathbb{R}$ [[Niz funkcija|niz funkcija]]. Tada **funkcionalni red generisan nizom** $(f_{n})$ $\Big($ili **funkcionalni red sa opštim članom** $f_{n}$$\Big)$ na skupu $B\subseteq A$ je  $\begin{align}\sum\limits_{n=1}^{\infty} f_{n} =f_{1}+f_{2}+\cdots+f_{n}+\cdots\end{align}$
- $\begin{align}s_{n}:\ A\to\mathbb{R}\ \text{ definisana sa } \ s_{n}=\sum\limits_{k=1}^{n}f_{k},\quad \forall i\in\mathbb{N}\end{align}$ $\quad$ je parcijalna suma reda.
- $\begin{align}(s_{n})=(s_{1},\,s_{2},\,\dots,\,s_{n},\,\dots)\end{align}$ $\quad$ je niz parcijalnih suma reda.

### Tačka po tačku konvergencija
**Def**. Neka je $f_{n}:\ A\to\mathbb{R}$ niz funkcija i neka je $s:\ B\to\mathbb{R}$, gde je $B\subseteq A$. Tada $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}\ \ \end{align}$ **tačka po tačku konvergira** ka funkcije $s$ na skupu $B$, ako niz parcijalnih suma $(s_{n})$ [[Niz funkcija#^05c72e|tačka po tačku konvergira]] ka funkcije $s$ na skupu $B$.
Tada pišemo $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}=s\end{align}$ $\ \:\Big(\Leftrightarrow\quad s_{n}\to s\Big)\ \:$ na skupu $B$.

$\:$
Detaljnije ([[Niz funkcija#^05c72e|*]], [[Brojevni red#^7a6e28|**]]),
$\begin{align}\sum\limits_{n=1}^{\infty}f_{n}=s\ \text{ na }\ B\quad&\Leftrightarrow\quad s_{n}\to s \ \text{ na } \ B\quad\Leftrightarrow\quad\forall x\in B\quad s(x)\overset{*}=\lim\limits_{ n \to \infty }s_{n}(x)\overset{**}=\overbrace{\sum\limits_{n=1}^{\infty}f_{n}(x)}^{\text{brojevni red}}\\\\&\Leftrightarrow\quad\forall x\in B\quad \forall\varepsilon>0\quad\exists N\in\mathbb{N}\quad\forall n\geqslant N\quad\left|s_{n}(x)-s(x)\right|<\varepsilon\end{align}$ ^05935c

> Napomena: Stoga, funkcija $s:\ A\to\mathbb{R}$ iz prethodne definicije je definisana sa $\begin{align}s(x) =\sum\limits_{n=1}^{\infty} f_{n}(x)\end{align}$

$\:$
**[[Brojevni red#^7e0ab5|Stav]]**. $\begin{align}\sum\limits_{n=1}^{\infty} f(x)\end{align}$ tačka po tačku konvergira na $B$ $\quad\Rightarrow\quad$ $f_{n}\to0$ $\:$ na $\:$ $B$

___
**Def**. $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}\end{align}$ **apsolutno tačka po tačku konvergira** na  $B$ ako $\begin{align}\sum\limits_{n=1}^{\infty}|f_{n}|\end{align}$ tačka po tačku konvergira na $B$.

**[[Brojevni red#^3872fa|Stav]]**. Ako red $\begin{align}\sum\limits_{n=1}^{\infty}f_{n}\end{align}$ apsolutno tačka po tačku konvergira na $B$ tada on tačka po tačku konvergira na $B$.
___
### Ravnomerna konvergencija

**Def**. Neka je $f_{n}:\ A\to\mathbb{R}$ niz funkcija. Tada funkcionalni red $\begin{align}\sum\limits_{n=1}^{\infty}f_{n} \end{align}$ **ravnomerno** (uniformno) **konvergira** ka $s$ na skupu $B$, ako niz parcijalnih suma $(s_{n})$ [[Niz funkcija#^6f4432|ravnomerno konvergira]] ka $s$ na skupu $B$.

$\:$
**[[Niz funkcija#^f64c89|Stav]]**. Ako red $\begin{align}\sum\limits_{n=1}^{\infty}f_{n}\end{align}$ ravnomerno konvergira na $B$ tada on tačka po tačku konvergira na $B$.

$\:$
**Stav**. $\begin{align}\sum\limits_{n=1}^{\infty} f(x)\end{align}$ ravnomerno konvergira na $B$ $\quad\Rightarrow\quad$ $f_{n}\rightrightarrows0$ $\:$ na $\:$ $B,$ $\:$ $n\to\infty$

$\:$
**Teorema** ([[Niz funkcija#^a1dec4|Košijev kriterijum ravnomerne konvergencije]] funkcionalnog reda). Red $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)\end{align}$ ravnomerno konvergira na skupu $B$ akko $\forall\varepsilon>0\quad\exists N\in\mathbb{N}\quad\forall m,\,k\geqslant N\quad\forall x\in B\quad|s_{m}(x)-s_{k}(x)|<\varepsilon$  ^d724ad

$\:$
**Teorema** (Vajerštrasov kriterijum ravnomerne konvergencije funkcionalnog reda). Neka je $f_{n}:\ A\to\mathbb{R}$ niz funkcija. Ako postoji red brojeva $(a_{n})$ za koji važi  ^b72d33
- $\begin{align}\sum\limits_{n=1}^{\infty} a_{n}\ \ \end{align}$ konvergira 
- $\exists N\in\mathbb{N}\quad\forall n\geqslant N\quad\forall x\in B\quad |f_{n}(x)|\leqslant a_{n}$

onda red $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)\end{align}$ ravnomerno konvergira na skupu $B$.
> Dokaz:
> Neka je $\forall n\in\mathbb{N}\quad\begin{align}s_{n}=\sum\limits_{k=1}^{n}f_{n}\end{align}$ parcijalna suma reda $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}\end{align}$ 
> i neka je $\begin{align}\forall n\in\mathbb{N}\quad\sigma_{n}=\sum\limits_{k=1}^{n}a_{n}\end{align}$ parcijalna suma reda $\begin{align}\sum\limits_{n=1}^{\infty} a_{n}\end{align}$.
>
> [[Kriterijumi konvergencije brojevnih redova#^f4afac|Iz Košijevog kriterijuma konvergencije brojevnog reda]]:
> $\begin{align}\sum\limits_{n=1}^{\infty}a_{n}\quad\text{konvergira}\quad\Rightarrow\quad\forall\varepsilon>0\quad \exists N_{1}\in\mathbb{N}\quad \forall m,\,k\geqslant N_{1}\quad\left|\sigma_{m}-\sigma_{k}\right|<\varepsilon\end{align}$
> 
> pretpostavimo da je $m>k$ (za $m<k$ je analogno).
> 
> $\begin{align}\forall x\in B\quad |s_{m}(x)-s_{k}(x)|&=|f_{k+1}(x)+f_{k+2}(x)+\dots+f_{m}(c)|\leqslant|f_{k+1}(x)|+|f_{k+2}(x)|+\dots+|f_{m}(x)|\leqslant\\&\leqslant a_{k+1}+a_{k+2}+\dots+a_{m}= \sigma_{m}-\sigma_{k}<\varepsilon\end{align}$
> 
> Konačno,
> $\begin{align}\forall\varepsilon>0\quad \exists N_{2}:=\max\{N,\,N_{1}\}\quad \forall m,\,k\geqslant N_{2}\quad\forall x\in B\quad\left|s_{m}(x)-s_{k}(x)\right|<\varepsilon\end{align}$
> tj. $\begin{align}\ \ \sum\limits_{n=1}^{\infty}f_{n}\ \ \end{align}$ ravnomerno konvergira na $B$

$\:$
### [[Svojstva ravnomerno konvergentnih funkcionalnih redova]]

### [[Stepeni red]]

### [[Furijeov red]]