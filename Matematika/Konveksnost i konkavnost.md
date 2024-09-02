#fax #math #a1 [deo poglavlja [[Izvod|"izvod"]]]
$\:$

$\forall z\in[x,\,y]\quad z=x+\underset{=:\lambda\,\in[0,\,1]}{\boxed{\frac{z-x}{y-x}}}\,(y-x) =x+\lambda\,(y-x)=(1-\lambda)\,x+\lambda\,y$
tj $\quad\forall \lambda\in[0,\,1]\quad z=(1-\lambda)\,x+\lambda\,y\in[x,\,y]$

![[analiza1_2_konveksnostGrafik.png]]
$\begin{align}\mathrm{tg}\,\alpha=\frac{f(y)-f(x)}{y-x}=\frac{a-f(x)}{z-x}\end{align},\quad z\in(x,\,y)$
Tada:
$\begin{align}a=f(x)+\frac{f(y)-f(x)}{y-x}\,(z-x)=f(x)+\underset{=\lambda}{\boxed{\frac{z-x}{y-x}}}\,\big(f(y)-f(x)\big)=\end{align}$
$=(1-\lambda)\,f(x)+\lambda\,f(y)$

Funkcija je konveksna ($\mathrm{I}$) u $z$ ako $f(z)<a$
Funkcija je konkavna ($\mathrm{II}$) u $z$ ako $f(z)>a$

---
**Def**. $f$ je **konveksna** (**konkavna**) na $A\subseteq D_{f}$ ako
$\forall x,\,y\in A\quad\forall\lambda\in[0,\,1]\quad f\big((1-\lambda)\,x+\lambda\,y\big)\underset{(\geqslant)}{\leqslant}(1-\lambda)\,f(x)+\lambda\,f(y)$

**Def**. $f$ je **prevojna tačka** fje $f$ ako je $f$ konveksna (konkavna) na $\mathrm{O}^{+}(x_{0})$ i konkavna (konveksna) na $\mathrm{O}^{-}(x_{0})$

Stav. $f$ je konveksna (konkavna) na $\mathrm{O}(x_{0})$ $\ \ \Leftrightarrow$
$\Leftrightarrow\ \:$ **tangenta** fje $f$ u tački $x_{0}$ je **ispod** (**iznad**) grafika fje $f$ na $\mathrm{O}(x_{0})$
$\:$

**Def**. **Nagib** fje $f$ u $x$ za fiksirano $a$ je $\begin{align}\nu_{a}(x)=\frac{f(x)-f(a)}{x-a}\end{align}$

[[analiza1_2_10.png|Stav]].  $f$ je konveksna (konkavna) na $A$ $\ \ \Leftrightarrow$
$\Leftrightarrow\ \ \Big( \forall x,\,y,\,a\in A\quad \underset{(x<y<a)\ \mathrm{ili}\ (a<x<y)}{x<a<y}\ \ \Rightarrow\ \ \nu_{a}(x)\leqslant\nu_{a}(y) \Big)$ 

[[analiza1_2_11.png|Teorema]]. Na nekom intervalu važi:
- $f\,\mathcal{D}\,(a,\,b).\quad$ $f$ je konveksna (konkavna) $\ \ \Leftrightarrow \ \ f'\!\uparrow\!(\!\downarrow\!)$
- $f\,\mathcal{D}^{1}\,(a,\,b).\quad$ $f$ je konveksna (konkavna) $\ \ \Leftrightarrow$ $\Leftrightarrow \ \ f''\geqslant0\ \ (f''\leqslant0)$

Stav. $f$ je konveksna (konkavna) na $(a,\,b)$ $\ \ \Leftrightarrow$
$\Leftrightarrow\ \ f^{-1}$ je konkavna (konveksna) na $f[(a,\,b)]$