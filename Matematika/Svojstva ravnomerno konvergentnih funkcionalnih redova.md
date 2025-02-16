#fax #math #a2 [deo poglavlja [[Funkcionalni red|"funkcionalni red"]]]
$\:$

**Stav**. Neka je $f_{n}:\ A\to\mathbb{R}$ funkcionalni niz i neka je $g:\ B\to\mathbb{R}$ ograničena funkcija ($B\subseteq A$). Tada
$\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)\ \ \text{ravnomerno konvergira na }\ B\quad\Rightarrow\quad\sum\limits_{n=1}^{\infty}g(x)f_{n}(x)\ \ \text{ravnomerno konvergira na }\ B\end{align}$
> Dokaz:
> Neka je $(s_{n})$ niz parcijalnih suma reda $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)\end{align}$
> i neka je $(\sigma_{n})$ niz parcijalnih suma reda $\begin{align}\sum\limits_{n=1}^{\infty}g(x) f_{n}(x)\end{align}$
>$\:$
>$g$ je ograničena $\quad\Leftrightarrow\quad$ $\exists C\in\mathbb{R}_{+}\quad\forall x\in B\quad |g(x)|\leqslant C$
>$\:$
> $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)\ \ \text{ravnomerno konvergira na }\ B\quad\Rightarrow\end{align}$ ([[Funkcionalni red#^d724ad|Košijev kriterijum]])
> $\begin{align}\forall \varepsilon>0 \quad\exists N\in\mathbb{N}\quad \forall m,\,k\geqslant N\quad\forall x\in B\quad|s_{m}(x)-s_{k}(x)|<\frac{\varepsilon}{M}\end{align}$
>
>Tada, $\begin{align}\forall \varepsilon>0 \quad \exists N\in\mathbb{N}\quad\forall m,\,k\geqslant N\quad\forall x\in B\quad|\sigma_{m}(x)-\sigma_{k}(x)|=|g(x)(s_{m}-s_{k})|<M\cdot\frac{\varepsilon}{M}=\varepsilon\quad\end{align}$
>iz [[Funkcionalni red#^d724ad|Košijevog kriterijuma]] $\begin{align}\sum\limits_{n=1}^{\infty}g(x)f_{n}(x)\ \ \text{ravnomerno konvergira na }\ B\end{align}$

$\:$
**Stav** (limes funkcionalnog reda). Neka je $f_{n}:\ A\to\mathbb{R}$ funkcionalni niz i neka je $a\in A$ [[Vrste tačaka u odnosu na neki skup#^3de7f2|tačka nagomilavanja]] skupa $A$. Tada ako važi:
- $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)\ \ \text{ravnomerno konvergira na }\ A\end{align}$
- $\forall n\in\mathbb{N}\quad\exists\lim\limits_{ x \to a }f_{n}(x)\in\mathbb{R}$

onda red brojeva $\begin{align}\sum\limits_{n=1}^{\infty}\lim\limits_{ x \to a } f_{n}(x)\ \ \text{ konvergira}\ \ \end{align}$ i važi
$\begin{align}\sum\limits_{n=1}^{\infty}\lim\limits_{ x \to a } f_{n}(x)=\lim\limits_{ x \to a }\underbrace{\sum\limits_{n=1}^{\infty}f_{n}(x)}_{\text{funkcionalni red}}\end{align}$

> Dokaz: Neka je $b_{n}=\lim\limits_{ x \to a }f_{n}(x), \quad\forall n\in\mathbb{N}$
> neka je $(s_{n})$ niz parcijalnih suma reda $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)\end{align}$
> i neka je $(\sigma_{n})$ niz parcijalnih suma reda $\begin{align}\sum\limits_{n=1}^{\infty}\lim\limits_{ x \to a }f_{n}(x)\end{align}$
>
> Tada,  $\begin{align}\lim\limits_{ x \to a }s_{n}(x)=\lim\limits_{ x \to a }\sum\limits_{k=1}^{n}f_{n}(x)=\sum\limits_{k=1}^{n}\lim\limits_{ x \to a }f_{n}(x)=\sigma_{n}\quad\quad(1)\end{align}$
>
> Iz ravnomerne konvergencije reda $\begin{align}\sum\limits_{n=1}^{\infty}f_{n}(x)\end{align}$ ([[Funkcionalni red#^d724ad|Košijev kriterijum]]) imamo
> $\begin{align}\forall \varepsilon>0\quad\exists N\in\mathbb{N}\quad\forall m,\,k\geqslant N\quad\forall x\in A\quad |s_{m}(x)-s_{k}(x)|\leqslant\frac{\varepsilon}{2}\quad\quad\bigg|\lim\limits_{ m \to \infty } \ \text{ pa           }\ \lim\limits_{ k \to \infty }(1)\end{align}$
> $\begin{align}\Rightarrow\quad\forall\varepsilon>0\quad\exists N\in\mathbb{N}\quad\exists m,\,k\geqslant N\quad|\sigma_{m}-\sigma_{k}|\leqslant\frac{\varepsilon}{2}<\varepsilon\end{align}$
> Iz [[Kriterijumi konvergencije redova brojeva#^f4afac|Košijevog kriterijuma]] red $\begin{align}\sum\limits_{n=1}^{\infty} \lim\limits_{ x \to a }f_{n}(x)\ \ \text{konvergira}\end{align}$
> 
> Neka $\begin{align}\sum\limits_{n=1}^{\infty} \lim\limits_{ x \to a }f_{n}(x)=\sigma\in\mathbb{R}\quad\Big(\Leftrightarrow\quad\forall\varepsilon>0\quad\exists N_{1}\in\mathbb{N}\quad\forall n\geqslant N_{1}\quad|\sigma_{n}-\sigma|<\frac{\varepsilon}{3}\Big)\end{align}$
> i neka $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)=s(x)\quad\Big(\Leftrightarrow\quad\forall x\in A\quad\forall\varepsilon>0\quad\exists N_{2}\in\mathbb{N}\quad\forall n\geqslant N_{2}\quad|s_{n}(x)-s(x)|<\frac{\varepsilon}{3}\Big)\end{align}$ 
>
>$\begin{align}(1)\quad\Leftrightarrow\quad\forall n\in\mathbb{N}\quad\forall\varepsilon>0\quad\exists \delta'\in\mathbb{N}\quad\forall\in\mathring{\mathrm{O}}_{\delta'}(a)\quad|s_{n}(x)-\sigma_{n}|<\frac{\varepsilon}{3}\end{align}$
>
> Dokazati da $\lim\limits_{ x \to a }s(x)=\sigma\quad\Big(\Leftrightarrow\quad\forall \varepsilon>0\quad\exists\delta>0\quad\forall x\in \mathring{\mathrm{O}}_{\delta}(a)\cap  A\quad|s(x)-\sigma|<\varepsilon\Big)$
> 
> $N:=\max\{N_{1},\,N_{2}\}$, tada za $\delta=\delta'$ važi:
> 
>  $\begin{align}|s(x)-\sigma|&=|s(x)-s_{N}(x)+s_{N}(x)-\sigma_{N}+\sigma_{N}-\sigma|\leqslant\\&\leqslant|s(x)-s_{N}(x)|+|s_{N}(x)-\sigma_{N}|+|\sigma_{N}-\sigma|=\frac{\varepsilon}{3}+\frac{\varepsilon}{3}+\frac{\varepsilon}{3}=\varepsilon\end{align}$
>  
>  tj. $\lim\limits_{ x \to a }s(x)=\sigma$


$\:$
**Posledica** (neprekidnost funkcionalnog reda). Neka je $f_{n}:\ A\to\mathbb{R}$ niz neprekidnih u tački $a\in A$ funkcija. Tada 
$\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)\ \ \text{ ravnomerno konvergira ka }\ s\quad\Rightarrow\quad s\,\mathcal{C}\,a\end{align}$ 