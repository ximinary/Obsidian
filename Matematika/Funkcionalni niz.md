#fax #math #a2 [deo [[Analiza|analize]]]
$\:$

**Def**. Neka $\forall n\in\mathbb{N}\quad f_{n}\,:A\to\mathbb{R}$. Tada je $(f_{n})=(f_{1},\,f_{2},\,\dots,\,f_{n},\dots)$ funkcionalni niz.

**Def**. Niz $f_{n}$ konvergira u tački $x_{0}\in A$ ako $\exists\lim\limits_{ n \to \infty }f_{n}(x_{0})\in\mathbb{R}$

$\:$
**Def.** Neka je $f_{n}\ :A\to\mathbb{R}$ funkcionalni niz i neka $f:\ B\to\mathbb{R}$, gde je $B\subseteq A$.
Niz $(f_{n})$ **tačka po tačku konvergira** ka funkciji $f$ na skupu $B$ ako važi
$\forall x\in B\quad\exists\lim\limits_{ n \to \infty }f_{n}(x)=f(x)\quad\bigg(\Leftrightarrow\quad\forall x\in B\quad \forall\varepsilon>0\quad\exists N\in\mathbb{N}\quad\forall n\geqslant N\quad|f_{n}(x)-f(x)|<\varepsilon\bigg)$
Oznaka: $f_{n}\to f$ na skupu $B$ ^05c72e

$\:$
**Def**. Neka je $f_{n}\ :A\to\mathbb{R}$ funkcionalni niz i neka je $f\,:B\to\mathbb{R}$, gde je $B\subseteq A$.
Niz $(f_{n})$ **ravnomerno** (uniformno) **konvergira** ka $f$ na skupu $B$ ako važi $\forall\varepsilon>0\quad\exists N\in\mathbb{N}\quad\forall n\geqslant N\quad\forall x\in B\quad|f_{n}(x)-f(x)|<\varepsilon$
Oznaka: $f_{n}\rightrightarrows f$ na skupu $B$, $n\to\infty$ ^6f4432

$\:$
**Stav**. $f_{n}\rightrightarrows f$ na skupu $B$, $n\to\infty$ $\quad\Rightarrow\quad$ $f_{n}\to f$ na skupu $B$ ^f64c89

$\:$
**Stav**. $\forall n\in\mathbb{N}\quad f_{n}\,\mathcal{C}\,B$ $\quad$ i $\quad$ $f_{n}\rightrightarrows f$ na skupu $B$, $n\to\infty$ $\quad\Rightarrow\quad$ $f\,\mathcal{C}\,B$
$\:$
> Napomena:
> Često koristimo kombinaciju prethodna dva stava:
> $\forall n\in\mathbb{N}\quad f_{n}\,\mathcal{C}\,B$ $\quad$ i $\quad$ $f_{n}\to f$ na skupu $B$, $n\to\infty$ $\quad$ pri čemu $f$ ima prekid
> $\Rightarrow\quad$ $f_{n}\,\not\rightrightarrows f$ na skupu $B$, $n\to\infty$

$\:$
**Stav**. $f_{n}\rightrightarrows f$ na skupu $B$, $n\to\infty$ $\quad\Leftrightarrow\quad\lim\limits_{ n \to \infty }\sup\limits_{x\in B}|f_{n}(x)-f(x)|=0$


$\:$
**Stav**. Neka su $f_{n},\,g_{n}:\,A\to \mathbb{R}$ funkcionalni nizovi, $\alpha,\,\beta\in\mathbb{R}$. Tada $f_{n}\rightrightarrows f\ \text{ i }\ g_{n}\rightrightarrows g,\ n\to\infty\quad\Rightarrow\quad\alpha f_{n}+\beta g_{n}\rightrightarrows\alpha f+\beta g,\ n\to\infty$
na nekom skupu $B\subseteq A$.

> Dokaz:
> $f_{n}\rightrightarrows f,\ n\to\infty\quad\Rightarrow\quad\lim\limits_{ n \to \infty }\sup\limits_{x\in B}|f_{n}(x)-f(x)|=0$
> $g_{n}\rightrightarrows g,\ n\to\infty\quad\Rightarrow\quad\lim\limits_{ n \to \infty }\sup\limits_{x\in B}|g_{n}(x)-g(x)|=0$
> 
> $\lim\limits_{ n \to \infty }\sup\limits_{x\in B}\bigg|\Big(\alpha f_{n}(x)+\beta g_{n}(x)\Big)-\Big(\alpha f(x)+\beta g(x)\Big)\bigg|=$
> $=\lim\limits_{ n \to \infty }\sup\limits_{x\in B}\bigg|\alpha\Big(f_{n}(x)-f(x)\Big)+\beta\Big(g_{n}(x)- g(x)\Big)\bigg|\leqslant$
> $\leqslant\alpha\lim\limits_{ n \to \infty }\sup\limits_{x\in B}\bigg|f_{n}(x)-f(x)\bigg|+\beta\lim\limits_{ n \to \infty }\sup\limits_{x\in B}\bigg|g_{n}(x)-g(x)\bigg|=0+0=0$
> 
> $\Rightarrow\quad\alpha f_{n}+\beta g_{n}\rightrightarrows\alpha f+\beta g,\ n\to\infty$

$\:$
**Teorema** (Košijev kriterijum ravnomerne konvergencije funkcionalnog niza). 
Funkcionalni niz $f_{n}:\ A\to\mathbb{R}$ ravnomerno konvergira na skupu $B$ akko
$\forall\varepsilon>0\quad\exists N\in\mathbb{N}\quad\forall m,\,k\geqslant N\quad\forall x\in B\quad|f_{m}(x)-f_{k}(x)|<\varepsilon$ ^a1dec4

> Dokaz: $\boxed{\Rightarrow}$
> $\begin{align}f_{n}\underset{n\to\infty}\rightrightarrows f\ \text{ na } \ B\quad\Rightarrow\quad\forall\varepsilon>0\quad\exists N\in\mathbb{N}\quad\forall n \geqslant N \quad\forall x\in B\quad|f_{n}(x)-f(x)|< \frac{\varepsilon}{2}\end{align}$
> $\begin{align}\Rightarrow\quad\forall\varepsilon>0\quad\exists m,\,k\in\mathbb{N}\quad\forall x\in B\quad\Big|f_{m}(x)-f_{k}(x)\Big|=\Big|\big(f_{m}(x)-f(x)\big)-\big(f_{k}(x)-f(x)\big)\Big|\leqslant\\\leqslant \Big|(f_{m}(x)-f(x)\Big|+\Big|f_{k}(x)-f(x)\Big|<\frac{\varepsilon}{2}+\frac{\varepsilon}{2}=\varepsilon\end{align}$
> 
> $\boxed{\Leftarrow}$ Iz tvrđenja sledi da $\forall x\in B\quad f_{n}(x)$ je [[Košijev niz]]. 
> Stoga, $\exists \lim\limits_{ n \to \infty }f_{n}(x)=f(x)\in\mathbb{R}$
> $\begin{align}\forall\varepsilon>0\quad\exists N\in\mathbb{N}\quad\forall n,\,k\geqslant N\quad\forall x\in B\quad&|f_{n}(x)-f_{k}(x)|<\frac{\varepsilon}{2}\quad\bigg|\lim\limits_{ n \to \infty }\\&|f(x)-f_{k}(x)|\leqslant\frac{\varepsilon}{2}<\varepsilon\end{align}$
> $\Rightarrow\quad f_{n}\underset{n\to\infty}\rightrightarrows f\ \text{ na } \ B$
