#fax #math #a1 [deo [[Analiza|analize]]]
$\:$

 **Def**. $f: D_{f}\to \mathbb{R},\ x_{0}\in \mathrm{int}\,D_{f}$
 ako $\begin{align}\exists \lim\limits_{ x \to x_{0} }\frac{f(x)-f(x_{0})}{x-x_{0}} = \lim\limits_{ h \to 0 }\frac{f(x_{0}+h)-f(x_{0})}{h} := f'(x_{0}) \end{align}$,
 on se zove **izvod** fje $f$ u $x_{0}$, tada je $f$ **diferencijabilna** u $x_0$ (oznaka: $f\,\mathcal{D}\,x_{0}$)

 **Def**. $f: D_{f}\to \mathbb{R},\ x_{0}\in \mathrm{int}\,D_{f}$
 ako $\begin{align}\exists \lim\limits_{ x \to x_{0}^{-/+} }\frac{f(x)-f(x_{0})}{x-x_{0}} = \lim\limits_{ h \to 0^{-/+} }\frac{f(x_{0}+h)-f(x_{0})}{h} := f'_{-/+}(x_{0}) \end{align}$,
 on se zove **levi/desni izvod**

Koristeći [[Limes funkcije#^cabb77|tvrđenje]] dobijamo:
$\begin{align}\lim\limits_{ x \to x_{0} }\frac{f(x)-f(x_{0})}{x-x_{0}}=f'(x)\ \ \Leftrightarrow\end{align}$
$\begin{align}\Leftrightarrow\ \ \frac{f(x)-f(x_{0})}{x-x_{0}}=f'(x)+o(1),\ x\to x_{0}\ \ \Leftrightarrow\end{align}$
$\begin{align}\Leftrightarrow\ \ f(x)=f(x_{0})+f'(x)(x-x_{0})+o(x-x_{0}),\ x\to x_{0}\end{align}$

Tangenta ka grafiku fje u tački $x_{0}$:
$y=f(x_{0})+f'(x_{0})(x-x_{0})$

### [[analiza1_2_osnovniIzvodi.png|Izvodi osnovnih funkcija]]
### Svojstva izvoda

[[analiza1_2_1.png|Tvrđenje 1]]. $f\,\mathcal{D}\,x_{0}\ \ \Rightarrow\ \ f\,\mathcal{C}\,x_{0}$

Tvrđenje 2. $f,\,g\,\mathcal{D}\,x_{0}, \ \ c\in \mathbb{R}$. Tada
- [[analiza1_2_2_1.png|1)]] $(f+g)\,\mathcal{D}\,x_{0},\quad(f+g)'(x_{0})=f'(x_{0})+g'(x_{0})$
$\ \ \ \ \ (c\,f)\,\mathcal{D}\,x_{0},\quad(c\,f)'(x_{0})=c\,f'(x_{0})$
- [[analiza1_2_2_2.png|2)]] $(f\cdot g)\,\mathcal{D\,x_{0}},\quad (f\cdot g)'(x_{0})=f'(x_{0})\cdot g(x_{0})+f(x_{0})\cdot g'(x_{0})$
- [[analiza1_2_2_3_1.png|3.1)]] ako $g(x_0)\ne0$, $\begin{align}\ \ \frac{1}{g}\,\mathcal{D}\,x_{0}\quad\bigg(\frac{1}{g}\bigg)'(x_{0})=-\frac{g'(x_{0})}{g^{2}(x_{0})}\end{align}$
- [[analiza1_2_2_3_2.png|3.2)]] ako $g(x_0)\ne0$, $\begin{align}\ \ \frac{f}{g}\,\mathcal{D}\,x_{0}\quad\bigg(\frac{f}{g}\bigg)'(x_{0})=\frac{f'(x_{0})\cdot g(x_{0})-f(x_{0})\cdot g'(x_{0})}{g^{2}(x_{0})}\end{align}$

[[analiza1_2_3.png|Tvrđenje 3]] (Izvod [[Kompozicija funkcija|složene funkcije]]). $y_{0}:=f(x_{0})$
$\begin{align}f\,\mathcal{D}\,x_{0}\\ g\,\mathcal{D\,y_{0}}\end{align} \ \ \Rightarrow (g\circ\!f)\,\mathcal{D}\,x_{0},\quad (g\circ\!f)'(x_{0})=g'(y_{0})\cdot f'(x_{0})$

[[analiza1_2_3prim.png|Primer]]

[[analiza1_2_4.png|Tvrđenje 4]] (Izvod [[Inverzna funkcija|inverzne funkcije]]). $f\,\mathcal{D}\,x_{0},\ f'(x_{0})\ne0,\ f$ ima inverz $g$ u $\mathrm{O}(x_{0}),\ y_{0}:=f(x_{0})$.
Tada $\begin{align}g\,\mathcal{D}\,y_{0},\quad g'(y_{0})=\frac{1}{f'(x_{0})}\end{align}$

[[analiza1_2_4prim.png|Izvodi nekih inverznih funkcija]]

### [[Ekstremum. Nužni i dovoljni uslov ekstremuma]]

### [[Teoreme o srednjoj vrednosti]]

### [[Lopitalova pravila]]

### Izvodi višeg reda
$f^{(0)}:=f$
$f^{(n+1)}:=\big(f^{(n)}\big)',\ \ \forall n\in\mathbb{N}_{0}$

[[analiza1_2_izvodiVisegReda.png|Viši izvodi nekih fja]]

[[analiza1_2_lajbnicovo.png|Teorema]] (Lajbnicovo pravilo).
$(\begin{align}f\cdot g)^{(n)}=\sum\limits_{k=0}^{n}\binom{n}{k}f^{(k)}g^{(n-k)}\end{align}$

**Def**. $f$ je $n$ puta diferencijabilna u $x_{0}$ ako $\exists f^{(n)}\:\:*$
**Def**. $f\,\mathcal{C}^{n}\,x_{0}\ \ \Leftrightarrow\ \ f^{(n)}\,\mathcal{C}\,x_{0}\:\:*$
**Def**. $f\,\mathcal{D}^{n}\,x_{0}\ \ \Leftrightarrow\ \ f^{(n)}\,\mathcal{D}\,x_{0}\:\:*$
$*$ — odakle $\exists f'(x_{0}),\ \exists f''(x_{0}),\ \dots,\ \exists f^{(n)}(x_{0})$

[[analiza1_2_7.png|Tvrđenje]]. Za $n \in \mathbb{N}$
- $f$ je parna i $(2n+1)$ puta diferencijabilna u $0\ \ \Rightarrow$
$\Rightarrow\ \ f^{(2n+1)}(0)=0$
- $f$ je neparna i $2n$ puta diferencijabilna u $0\ \ \Rightarrow$
$\Rightarrow\ \ f^{(2n)}(0)=0$

### [[Tejlorov polinom]]

### [[Konveksnost i konkavnost]]