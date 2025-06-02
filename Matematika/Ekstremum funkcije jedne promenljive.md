#fax #math #a1 [deo [[Izvod funkcije jedne promenljive|poglavlja "izvod"]]]
$\:$

> Napomena: [[Ekstremum funkcije više promenljivih|Ekstremum funkcije više promenljivih]]

$\:$
**Def**. $x_{0}\in \mathrm{int}\, D_{f}$, $f$ ima u $x_{0}\ \  \{\dots|\}$ ako $\exists\mathrm{O}(x_{0})\ \ \forall x\in \mathrm{O}(x_{0})\cap D_{f}\ \ \{|\dots\}$:

$\begin{align}\mathrm{lokalni}\\ \mathrm{ekstrmum}\end{align}\left\{\begin{array}{c | c}
\mathrm{lokalni\ maksimum} & f(x)\leqslant f(x_0) \\
\mathrm{strogi\ lokalni\ maksimum} & f(x)< f(x_0) \\
\mathrm{lokalni\ minimum} & f(x)\geqslant f(x_0) \\
\mathrm{strogi\ lokalni\ minimum} & f(x)> f(x_0) \\
\end{array}\right\}$

$\:$
[[analiza1_2_ferma.png|Teorema]] (Fermaova; nužni uslov lokalnog ekstremuma).
$x_{0}\in \mathrm{int}\,D_{f},\ f\,\mathcal{D}\,x_{0},\ f$ ima lokalni ekstremum u $x_{0}$.
Tada $f'(x_{0})=0$

$\:$
**Def**. Tačka $x_{0}$ za koju važi $f'(x_{0})=0$ zove se **kritična** tačka.
> Skup tačaka ekstremuma je podskup skupa kritičnih tačaka

$\:$
[[analiza1_2_dovoljniUslovEkstremuma.png|Teorema]] (dovoljni uslov lokalnog ekstremuma).
$f\,\mathcal{C}^{k}\,\mathrm{O}(x_{0}),\ \ f'(x_{0})=f''(x_{0})=\dots=f^{(k-1)}(x_{0})=0, \ \ f^{(n)}(x_{0})\ne 0$
1\) $\ \ k$ je paran broj$\ \ \Rightarrow\ \ x_{0}$ je ekstremum
$\quad\:$ ako $f^{(n)}(x_{0})>0$, $\ \ x_{0}$ je minimum
$\quad\:$ ako $f^{(n)}(x_{0})<0$, $\ \ x_{0}$ je maksimum
2\) $\ \ k$ je neparan broj$\ \ \Rightarrow\ \ x_{0}$ nije ekstremum (ali jeste [[Konveksnost i konkavnost|prevojna tačka]])
