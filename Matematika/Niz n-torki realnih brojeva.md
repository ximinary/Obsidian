#fax #math #a3 [deo [[Analiza|analize]]]
$\:$

Zbog toga što je [[Skup n-torki realnih brojeva|skup n-torki realnih brojeva]] [[Unitarni prostor. Euklidski prostor|Euklidski prostor]], niz n-totki smatramo specijalnim slučajem [[Beskonačnodimenzioni Euklidski prostor. Niz i red vektora#Niz vektora Euklidskog prostora|niza vektora]].

Detaljnije, neka su $\forall k\in\mathbb{N}\quad \mathbf{a}_{k}\in\mathbb{R}^{n}$; tada niz $(\mathbf{a}_{k})$ konvergira ka $\mathbf{a}\in\mathbb{R}^{n}$ $\:$ $\Big(\lim\limits_{ k \to \infty } \mathbf{a}_{k}=\mathbf{a}\Big)$ ako za [[Niz brojeva|niz realnih brojeva]] $||\mathbf{a}_{k}−\mathbf{a}||$ važi $\lim\limits_{ k \to \infty }||\mathbf{a}_{k}-\mathbf{a}||=0$ 
tj. $\forall\varepsilon>0 \quad\exists N\in\mathbb{N}\quad\forall k\geqslant N\quad||\mathbf{a}_{k}-\mathbf{a}||<\varepsilon$

Stav. Neka $\forall k\in\mathbb{N}\quad \mathbf{a}_{k}=(a_{1k},\,a_{2k},\,\dots,\,a_{nk})\in\mathbb{R}^{n}$ i neka je $\mathbf{a}=(a_{1},\,a_{2},\,\dots,\,a_{n})\in\mathbb{R}^{n}$. Tada
$\lim\limits_{ k \to \infty }\mathbf{a}_{k}=\mathbf{a}\quad\Leftrightarrow\quad\begin{cases}\lim\limits_{ k \to \infty }a_{1k}=a_{1}\\\lim\limits_{ k \to \infty }a_{2k}=a_{2}\\\dots\\\lim\limits_{ k \to \infty }a_{nk}=a_{n}\end{cases}$
> Dokaz:
> $\lim\limits_{ k \to \infty }\mathbf{a}_{k}=\mathbf{a}\quad\Leftrightarrow\quad\forall\varepsilon>0 \quad\exists N\in\mathbb{N}\quad\forall k\geqslant N\quad\sqrt[]{(a_{1k}-a_{1})^{2}+(a_{2k}-a_{2})^{2}+\dots+(a_{nk}-a_{n})^{2}}<\varepsilon$
> $\boxed{\Rightarrow}$ $\forall i =\overline{1,n}\quad|a_{ik}-a_{i}|<\sqrt[]{(a_{1k}-a_{1})^{2}+(a_{2k}-a_{2})^{2}+\dots+(a_{nk}-a_{n})^{2}}<\varepsilon$
> Odakle, $\forall i =\overline{1,n}\quad\lim\limits_{ k \to \infty }a_{ik}=a_{i}$
> $\boxed{\Leftarrow}$ $\forall i =\overline{1,n}\quad\lim\limits_{ k \to \infty }a_{ik}=a_{i}\quad\Rightarrow$
>  $\begin{align}\Rightarrow\quad\forall i =\overline{1,n}\quad\forall\varepsilon>0\quad\exists N_{i}\in\mathbb{N}\quad\forall k\geqslant N_{i}\quad|a_{ik}-a_{i}|<\frac{\varepsilon}{n}\end{align}$
>  $\begin{align}\Rightarrow\quad\forall\varepsilon>0\quad\exists N:=\max_{i=\overline{1,n}}N_{i}\quad\forall k\geqslant N\quad&\sqrt[]{(a_{1k}-a_{1})^{2}+(a_{2k}-a_{2})^{2}+\dots+(a_{nk}-a_{n})^{2}}<\\&<|a_{1k}-a_{1}|+|a_{2k}-a_{2}|+\dots+|a_{nk}-a_{n}|<n\cdot\frac{\varepsilon}{n}=\varepsilon\end{align}$