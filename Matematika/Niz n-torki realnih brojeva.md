#fax #math #a3 [deo [[Analiza|analize]]]
$\:$

Zbog toga što je [[Skup n-torki realnih brojeva|skup n-torki realnih brojeva]] [[Unitarni prostor. Euklidski prostor|Euklidski prostor]], niz n-totki smatramo specijalnim slučajem [[Beskonačnodimenzioni Euklidski prostor. Niz i red vektora#Niz vektora Euklidskog prostora|niza vektora]].

Detaljnije, neka su $\forall k\in\mathbb{N}\quad a_{k}\in\mathbb{R}^{n}$; tada niz $(a_{k})$ konvergira ka $a\in\mathbb{R}^{n}$ $\:$ $\Big(\lim\limits_{ k \to \infty } a_{k}=a\Big)$ ako za [[Niz brojeva|niz realnih brojeva]] $||a_{k} −a||$ važi $\lim\limits_{ k \to \infty }||a_{k}-a||=0$ 
tj. $\forall\varepsilon>0 \quad\exists N\in\mathbb{N}\quad\forall k\geqslant N\quad||a_{k}-a||<\varepsilon$

Stav. Neka $\forall k\in\mathbb{N}\quad a_{k}=(x_{1k},\,x_{2k},\,\dots,\,x_{nk})\in\mathbb{R}^{n}$ i neka je $a=(x_{1},\,x_{2},\,\dots,\,x_{n})\in\mathbb{R}^{n}$. Tada
$\lim\limits_{ k \to \infty }a_{k}=a\quad\Leftrightarrow\quad\begin{cases}\lim\limits_{ k \to \infty }x_{1k}=x_{1}\\\lim\limits_{ k \to \infty }x_{2k}=x_{2}\\\dots\\\lim\limits_{ k \to \infty }x_{nk}=x_{n}\end{cases}$
> Dokaz:
> $\lim\limits_{ k \to \infty }a_{k}=a\quad\Leftrightarrow\quad\forall\varepsilon>0 \quad\exists N\in\mathbb{N}\quad\forall k\geqslant N\quad\sqrt[]{(x_{1k}-x_{1})^{2}+(x_{2k}-x_{2})^{2}+\dots+(x_{nk}-x_{n})^{2}}<\varepsilon$
> $\boxed{\Rightarrow}$ $\forall i =\overline{1,n}\quad|x_{ik}-x_{i}|<\sqrt[]{(x_{1k}-x_{1})^{2}+(x_{2k}-x_{2})^{2}+\dots+(x_{nk}-x_{n})^{2}}<\varepsilon$
> Odakle, $\forall i =\overline{1,n}\quad\lim\limits_{ k \to \infty }x_{ik}=x_{i}$
> $\boxed{\Leftarrow}$ $\forall i =\overline{1,n}\quad\lim\limits_{ k \to \infty }x_{ik}=x_{i}\quad\Rightarrow$
>  $\begin{align}\Rightarrow\quad\forall i =\overline{1,n}\quad\forall\varepsilon>0\quad\exists N_{i}\in\mathbb{N}\quad\forall k\geqslant N_{i}\quad|x_{ik}-x_{i}|<\frac{\varepsilon}{n}\end{align}$
>  $\begin{align}\Rightarrow\quad\forall\varepsilon>0\quad\exists N:=\max_{i=\overline{1,n}}N_{i}\quad\forall k\geqslant N\quad&\sqrt[]{(x_{1k}-x_{1})^{2}+(x_{2k}-x_{2})^{2}+\dots+(x_{nk}-x_{n})^{2}}<\\&<|x_{1k}-x_{1}|+|x_{2k}-x_{2}|+\dots+|x_{nk}-x_{n}|<n\cdot\frac{\varepsilon}{n}=\varepsilon\end{align}$