#fax #math #laag [deo poglavlja [[Linearni operator|"linearni operator"]]]
$\:$

**Def**. Neka je i $V$ [[Vektorski prostor|vektorski prostor]] nad poljem $\mathbb{F}$. [[Linearni operator]] $f:\ V\to \mathbb{F}$ se zove **linearni funkcional**.

$V^{*}:=\mathrm{Hom}\,(V,\,\mathbb{F})$ — skup svih linearnih funkcionala na $V$ (jeste [[Linearni operator#VP $ mathrm{Hom}(U, ,V)$ i algebra $ mathrm{Hom} ,V$|VP]]).

Neka je $\dim V=n$. Tada $\ \:\mathrm{rang}\,f\leqslant1\ \:$ i $\ \:\mathrm{defekt}\,f\geqslant n-1$

$\forall \alpha\in \mathbb{F}\quad\forall f\ne\mathbb{O}\quad\exists v\in V\ \ :\ \ f(v)=\alpha$
___
Neka je $g\in V^{*}$ — ne-nula linearni funkcional, $\dim V=n$. 
Tada $\:\ \mathrm{rang}\,g=1\ \:$ i $\ \:\mathrm{defekt}\,g=n-1\ \:$

$\mathrm{Ker}\,g$ je hiperravan u $V$.
$\mathcal{B}_{f}=(a_{1},\,a_{2},\,\dots,\,a_{n-1})$ je baza $\mathrm{Ker}\, g$.

$\mathcal{B}=(a_{0},\,a_{1},\,a_{2},\,\dots,\,a_{n-1})$ je baza $V$. $\ \:$ $g(a_{0})\ne 0$
### Primeri linearnih funkcionala
- Neka je $e=(e_{1},\,e_{2},\,\dots,\,e_{n})$ baza VP-a $V$.
  Tada $\forall x\in V\quad x = \sum\limits_{n=1}^{n}x_{i}\,e_{i}$.
  **Projektor** na $j$-tu komponentu ($j = \overline{1,n}$):
  $\pi_{j}:\ \mathbb{F}^{n}\to\mathbb{F}\ \:$ def. sa $\pi_{j}(x)=x_{j}\ \:$ je linearni funkcional.
- [[Kvadratna matrica#Trag matrice|Trag matrice]]
- $[a,\,b]\subseteq\mathbb{R}, \ \ \mathcal{C}\,[a,\,b]$ je skup svih [[Neprekidnost|neprekidnih]] realnih funkcija na $[a,\,b]$. 
  Tada je $\mathcal{C}_{[a,\,b]}=\big(\mathcal{C}\,[a,\,b],\ \mathbb{R},\ +,\ \cdot\big)$ VP.
  $\:$
  $\forall x_{0}\in[a,\,b]\quad \varphi_{x_{0}}:\ \mathcal{C}_{[a,\,b]}\to \mathbb{R}\ \:$ def. sa $\varphi_{x_{0}}(f)=f(x_{0})$.
  $\varphi_{x_{0}}$ je linearni funkcional.

### Dualna baza — baza $V^{*}$
**Stav**. Neka je $e=(e_{1},\,e_{2},\,\dots,\,e_{n})$, $\dim V = n$. Tada je $e^{*}=\{ \pi_{1},\,\pi_{2},\,\dots,\,\pi_{n} \}$ jedinstvena baza od $V^{*}$ za koju važi $\pi_{j}(e_{i})=\delta_{ij}=\begin{cases}1,&\text{ako }i=j\\0,&\text{ako }i\ne j\end{cases}$ $\quad\quad$ ($\pi_{j}$ je projektor iz premera)

$e^{*}$ je **dualna baza**.

**Stav**. $e=(e_{1},\,e_{2},\,\dots,\,e_{n})$ je baza VP-a $V$, $e^{*}=\{ \pi_{1},\,\pi_{2},\,\dots,\,\pi_{n} \}$ je baza $V^{*}$. Tada važi:
1. $\forall f\in\mathrm{Hom}(V,\,\mathbb{F})\quad f=\sum\limits_{i=1}^{n}f(e_{i})\cdot\pi_{i}$
2. $\forall x\in V\quad x =\sum\limits_{i=1}^{n}\pi_{i}(x)\cdot e_{i}$ $\quad$ — jer $\pi_{i}(x)=x_{i}$

> Dokaz 1.
> $f=\sum\limits_{i=1}^{n}f_{i}\,\pi_{i}\ ,\quad f_{i}\in\mathbb{F}$
> $\forall j = \overline{1,n}\quad f(e_{j})=\sum\limits_{i=1}^{n}f_{i}\,\pi_{i}(e_{j})=f_{j}$
> Odakle sledi tvrđenje.

$f(x)=\sum\limits_{i=1}^{n}f(e_{i})\cdot\pi_{i}(x)=\sum\limits_{i=1}^{n}f_{i}\,x_{i}$

### Anihilator

**Def**. $S\subseteq V$, $V$ je VP. Tada **anihilator** je $S^{\circ}=\{ f \in V^{*}\ \big|\ f(x)=0\quad \forall x\in S\}$.

$S^{\circ}\leqslant V^{*}$

$S=V\quad\Rightarrow\quad S^{\circ}=\{ f\equiv 0 \}$
$S=\{0\}\quad\Rightarrow\quad S^{\circ}=V^{*}$

Teorema. $V$ je konačnodimenzioni VP nad $\mathbb{F}$, $\:$ $L\leqslant V$. 
Tada $\:$ $\dim L+\dim L^{\circ}=\dim V$

Neka je $e_{L}= (e_{1},\,e_{2},\,\dots,\,e_{l})$ baza od $L$, tako da je
$e=(e_{1},\,e_{2},\,\dots,\,e_{l},\,e_{l+1},\,\dots,\,e_{n})$ baza od $V$.
$e^{*}=(\pi_{1},\,\pi_{2},\,\dots,\,\pi_{n})$ je baza od $V^{*}$.
Tada je $(\pi_{l+1},\,\pi_{l+2},\,\dots,\,\pi_{n})$ je baza od $L^{\circ}$

Posledica. $L,\,M\leqslant V$. Tada $L=M\ \ \Leftrightarrow\ \ L^{\circ}=M^{\circ}$

Stav. $V$ je konačnodimenzioni VP nad $\mathbb{F}$, $\:$ $S\subseteq V$.
Tada $\big(S^{\circ}\big)^{\circ}=\mathcal{L}(S)$