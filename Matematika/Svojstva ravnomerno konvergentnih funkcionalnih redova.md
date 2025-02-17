#fax #math #a2 [deo poglavlja [[Funkcionalni red|"funkcionalni red"]]]
$\:$

**Stav**. Neka je $f_{n}:\ A\to\mathbb{R}$ funkcionalni niz i neka je $g:\ B\to\mathbb{R}$ ograničena funkcija ($B\subseteq A$). Tada
$\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)\ \ \text{ravnomerno konvergira na }\ B\quad\Rightarrow\quad\sum\limits_{n=1}^{\infty}g(x)f_{n}(x)\ \ \text{ravnomerno konvergira na }\ B\end{align}$
> Dokaz:
> Neka je $(s_{n})$ niz parcijalnih suma reda $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)\end{align}$
> i neka je $(\sigma_{n})$ niz parcijalnih suma reda $\begin{align}\sum\limits_{n=1}^{\infty}g(x) f_{n}(x)\end{align}$
>$\:$
>$g$ je ograničena $\quad\Leftrightarrow\quad$ $\exists C\in\mathbb{R}_{+}\quad\forall x\in B\quad |g(x)|\leqslant M$
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
> $\begin{align}\forall \varepsilon>0\quad\exists N\in\mathbb{N}\quad\forall m,\,k\geqslant N\quad\forall x\in A\quad |s_{m}(x)-s_{k}(x)|\leqslant\frac{\varepsilon}{2}\quad\quad\bigg|\lim\limits_{ x \to a }\end{align}$
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

$\:$
**Teorema** (integracija funkcionalnog reda). Neka je $f_{n}:\ [a,\,b]\to\mathbb{R}$ niz neprekidnih na $[a,\,b]$ funkcija i neka je $x_{0}\in[a,\,b]$. Tada
$\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)\ \ \text{ravnomerno konvergira na }\ [a,\,b]\quad\Rightarrow\quad\sum\limits_{n=1}^{\infty}\bigg(\int_{x_{0}}^{x} f_{n}(t) \, dt\bigg)\ \ \text{ravnomerno konvergira na }\ [a,\,b]\end{align}$
i važi $\begin{align}\forall x\in[a,\,b]\quad \sum\limits_{n=1}^{\infty}\bigg(\int_{x_{0}}^{x} f_{n}(t) \, dt\bigg)=\int_{x_{0}}^{x} \bigg(\sum\limits_{n=1}^{\infty}f_{n}(t)\bigg) \, dt\end{align}$
> Dokaz:
> Neka je $(s_{n})$ niz prefiksnih suma reda $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)\end{align}$
> i neka je $(\sigma_{n})$ niz prefiksnih suma reda $\begin{align}\sum\limits_{n=1}^{\infty}\bigg(\int_{x_{0}}^{x} f_{n}(t) \, dt\bigg)\end{align}$
> 
> $\begin{align}\sigma_{n}(x)&=\sum\limits_{k=1}^{n}\bigg(\int_{x_{0}}^{x} f_{k}(t) \, dt\bigg)=\int_{x_{0}}^{x} f_{1}(t) \, dt+\int_{x_{0}}^{x} f_{2}(t) \, dt+\dots+\int_{x_{0}}^{x} f_{n}(t) \, dt=\\&=\int_{x_{0}}^{x} \bigg(f_{1}(t)+f_{2}(t)+\dots+f_{n}(t)\bigg) \, dt=\int_{x_{0}}^{x}  \bigg(\sum\limits_{k=1}^{n}f_{k}(t)\bigg)\, dt=\int_{x_{0}}^{x}  \,s_{n}(x) dx\end{align}$
> 
> $\:$
> Jer $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)\ \ \text{ravnomerno konvergira na }\ [a,\,b]\end{align}$ iz prethodne posledice dobijamo da $s:\ [a,\,b]\to\mathbb{R}$ definisana sa $\begin{align}s(x):=\sum\limits_{n=1}^{\infty} f_{n}(x)\end{align}$ neprekidna na $[a,\,b]$. Stoga, $\forall x\in[a,\,b]\quad\exists\begin{align}\int_{x_{_{0}}}^{x} s(t) \, dt \end{align}$
> 
> $\begin{align}&\sum\limits_{n=1}^{\infty} f_{n}(x)\ \ \text{ravnomerno konvergira ka }\ s \ \text{ na } \ [a,\,b]\quad\Leftrightarrow\\&\Leftrightarrow\quad\forall\varepsilon>0\quad\exists N\in\mathbb{N}\quad \forall n\geqslant N\quad\forall x\in[a,\,b]\quad|s_{n}(x)-s(x)|<\frac{\varepsilon}{b-a}\end{align}$
> 
> Dokazati da red $\begin{align}\sum\limits_{n=1}^{\infty} \bigg(\int_{x_{0}}^{x} f_{n}(t) \, dt\bigg)\end{align}$ ravnomerno konvergira ka $\begin{align}\int_{x_{0}}^{x} s(t) \, dt\end{align}$ na $[a,\,b]$ tj. 
> $\begin{align}\forall\varepsilon>0\quad\exists N\in\mathbb{N}\quad\forall n\geqslant N\quad\forall x\in[a,\,b] \quad\bigg|\sigma_{n}(x)-\int_{x_{0}}^{x} s(t) \, dt\bigg|=\\=\bigg|\int_{x_{0}}^{x}\Big( s_{n}(t)-s(t) \Big)\, dt\bigg|<\bigg|\int_{x_{0}}^{x}\frac{\varepsilon}{b-a}\, dt\bigg|=\varepsilon\frac{|x-x_{0}|}{b-a}<\varepsilon\end{align}$

$\:$
**Stav** (diferenciranje funkcionalnog reda). Neka je $f_{n}:\ [a,\,b]\to\mathbb{R}$ niz funkcija, takvih da $\forall n\in\mathbb{N}\quad f_{n}\,\mathcal{C}^{1}\,[a,\,b]$. Tada ako važi:
- $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)\ \ \text{tačka po tačku konvergira na }\ [a,\,b]\end{align}$
- $\begin{align}\sum\limits_{n=1}^{\infty} f'_{n}(x)\ \ \text{ravnomerno konvergira na }\ [a,\,b]\end{align}$

onda $\begin{align}\bigg(\sum\limits_{n=1}^{\infty} f_{n}(x)\bigg)\,\mathcal{C}^{1}\,[a,\,b]\end{align}$ i važi $\begin{align}\forall x\in[a,\,b]\quad \bigg(\sum\limits_{n=1}^{\infty}f_{n}(x)\bigg)'=\sum\limits_{n=1}^{\infty}f'_{n}(x)\end{align}$
> Dokaz: Neka je $\begin{align}\sum\limits_{n=1}^{\infty} f_{n}(x)=s(x)\end{align}$ i neka $\begin{align}\sum\limits_{n=1}^{\infty} f'_{n}(x)=\sigma(x)\end{align}$
> (iz posledice $\sigma\,\mathcal{C}\,[a,\,b]$)
> 
> Iz prethodnog stava $\begin{align}\forall x,\,x_{0}\in[a,\,b]\quad\int_{x_{0}}^{x} \sigma(t) \, dt&=\int_{x_{0}}^{x} \bigg(\sum\limits_{n=1}^{\infty}f'_{n}(x)\bigg) \, dt=\sum\limits_{n=1}^{\infty}\bigg(\int_{x_{0}}^{x}f'_{n}(x) \, dx\bigg)=\\&=\sum\limits_{n=1}^{\infty}\bigg(f_{n}(x)-f_{n}(x_{0})\bigg)=s(x)-s(x_{0}) \end{align}$
> 
> Jer je $\sigma\,\mathcal{C}\,[a,\,b]$ imamo $\sigma(x)=s'(x)$, i samim tim $s\,\mathcal{C}^{1}\,[a,\,b]$