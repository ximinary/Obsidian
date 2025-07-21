#fax #math #alg  [deo [[Grupa|poglavlja "grupa"]]]
$\:$

**Def**. Neka je $G$ grupa, a $X\ne\varnothing$ je skup. **Dejstvo grupe** $G$ na skupu $X$ je funkcija $\Theta:\ G\times X\to X$ za koju važi:
- $\forall x\in X\quad\Theta(e,\,x)=x$
- $\forall x\in X,\ \ g,\,h\in G\quad\Theta\big(g,\ \Theta(h,\,x)\big)=\Theta(gh,\,x)$

Skraćeno zapisujemo $\Theta(g,\,x)$ kao $g\cdot x$, tada uslovi se zapisuju kao
- $\forall x\in X\quad e\cdot x=x$
- $\forall x\in X,\ \ g,\,h\in G\quad g\cdot(h\cdot x)=(gh)\cdot x$

> Napomena: ne treba mešati $\cdot$ (dejstvo) sa operacijom u grupi!

$\:$
**Def**. Neka grupa $G$ dejstvuje na $X\ne\varnothing$.
- **Orbita elementa** $x\in X$ je $\Omega(x):=\{g\cdot x\ \big|\ g\in G\}$
- **Stabilizator elementa** $x\in X$ je $\Sigma_{x}:=\{g\in G\ \big|\ g\cdot x=x\}$
 - **Skup svih fiksnih tačaka elementa** $g\in G$ je $X^{g}:=\{x\in X\ \big|\ g\cdot x=x\}$.

Važi $\ \:$ $x\in X^{g}\quad\Leftrightarrow\quad g\in \Sigma_{x}$

$\:$
> Primer 1: Neka je $X=\mathbb{R}^{2}$, $G=\mathbb{Z}_{2}$. Tada je sa 
> $0\cdot(x_{1},\,x_{2})=(x_{1},\,x_{2}),\quad 1\cdot(x_{1},\,x_{2})=(-x_{1},\,-x_{2})$ 
> zadato dejstvo $G$ na $X$.
> 
> Pokažemo da je to zapravo dejstvo.
> $0$ je neutral, jer važi $0\cdot(x_{1},\,x_{2})=(x_{1},\,x_{2})$, zadovoljen je prvi uslov.
> Za drugi uslov proveravamo sve mogućnosti:
> $(0+0)\cdot(x_{1},\,x_{2})=0\cdot(x_{1},\,x_{2})=(x_{1},\,x_{2})=0\cdot\big(0\cdot(x_{1},\,x_{2})\big)$
> $(0+1)\cdot(x_{1},\,x_{2})=1\cdot(x_{1},\,x_{2})=(-x_{1},\,-x_{2})=0\cdot\big(1\cdot(x_{1},\,x_{2})\big)$
> $(1+0)\cdot(x_{1},\,x_{2})=1\cdot(x_{1},\,x_{2})=(-x_{1},\,-x_{2})=1\cdot\big(0\cdot(x_{1},\,x_{2})\big)$
> $(1+1)\cdot(x_{1},\,x_{2})=0\cdot(x_{1},\,x_{2})=(x_{1},\,x_{2})=0\cdot\big(0\cdot(x_{1},\,x_{2})\big)$
> 
> Nađemo i orbitu proizvoljnog elementa:
> $\Omega\big((x_{1},\,x_{2})\big)=\{(x_{1},\,x_{2}),\,(-x_{1},\,-x_{2})\}$


> Primer 2: Neka je $G$ grupa, $H\leqslant G$. Tada sa 
> $g\cdot h= gh$ $\ \:$ <u>nije</u> definisano dejstvo $G$ na $H$,
> jer u opštem slučaju $\exists g\in G\ \:\ \ gh\not\in H$

> Primer 3: Neka je $G$ grupa, $H\leqslant G$. Tada je sa 
> $h\cdot g= hg$ $\ \:$ dato dejstvo $H$ na $G$.
> $\Omega(g)=\{hg\ \big|\ h\in H\}=Hg$

> Primer 4: Neka je $G$ grupa, $H\leqslant G$. Tada je sa 
> $g\cdot (aH)= (ga)H$ $\ \:$ dato dejstvo $G$ na $G/H$.
> $\Omega(aH)=\{(ga)H\ \big|\ g\in G\}=G/H$

> Primer 5: Neka je $G$ grupa, $X=G$. Tada je sa 
> $g\cdot x=gxg^{-1}$ $\ \:$ zadato dejstvo $G$ na $G$.
> 
> Pokažemo da je to zapravo dejstvo.
> Prvi uslov: $e\cdot x=exe^{-1}=x$
> Drugi uslov: $g_{1}\cdot(g_{2}\cdot x)=g_{1}g_{2}xg_{2}^{-1}g_{1}^{-1}=g_{1}g_{2}x(g_{1}g_{2})^{-1}=(g_{1}g_{2})\cdot x$
> 
> Orbite su [[Normalne podgrupe#^49fdd9|klase konjugacije]] grupe $G$, a stabilizator je *centralizator* $C(x)=\{g\in G\ \big|\ xg=gx\}$.

$\:$
**Stav**. Neka grupa $G$ dejstvuje na $X\ne\varnothing$. Tada
- $\forall x\in X\quad \Sigma_{x}\leqslant G$;
- postoji bijekcija između $G/\Sigma_{x}$ i $\Omega(x)$.

>Dokaz:
> Prvo tvrđenje. 
> Iz definicije dejstva i stabilizatora $e\in \Sigma_{x}$
> Za $g,\,h\in \Sigma_{x}$, važi $\ \:$ $g\cdot x=x\ \text{ i }\ h\cdot x =x$
> imamo, $(gh^{-1})\cdot x=g\cdot(h^{-1}\cdot x)=g\cdot\big(h^{-1}\cdot (h\cdot x)\big)=g\cdot\big((hh^{-1})\cdot x\big)=g\cdot(e\cdot x)=g\cdot x= x$
> $\Rightarrow\quad gh^{-1}\in \Sigma_{x}$ 
> Pomoću [[Grupa#^2ea486|stava]] dobijamo $\Sigma_{x}\leqslant G$
>
>Drugo tvrđenje. 
>$f:\ G/\Sigma_{x}\to \Omega(x)$ data sa $f(g\Sigma_{x})=g\cdot x$
> Pokazati da je $f$ bijektivna funkcija:
> funkcija. Neka $g\Sigma_{x}=h\Sigma_{x}$, tada $g^{-1}h\in \Sigma_{x}$
> $\quad$ tj. $(g^{-1}h)\cdot x=x$, $\ \:$ $g\cdot\big((g^{-1}h)\cdot x\big)=g\cdot x$,
> $\quad$ $(gg^{-1}h)\cdot x=g\cdot x$, $\ \:$ $h\cdot x=g\cdot x$
> "na". Jeste po def. 
> "1-1". Pretpostavljamo $h\cdot x=g\cdot x$;
> $\quad$ odakle postupkom obratnim od postupka u kojem
> $\quad$ je dokazano da je $f$ fja dobijamo da $g\Sigma_{x}=h\Sigma_{x}$

$\:$
**Posledica** (prethodnog stava i [[Red grupe i elementa. Indeks podgrupe#^cd291f|Lagranžove teoreme]]). Neka grupa $G$ dejstvuje na $X\ne\varnothing$. Tada $\ \:$ $\forall x\in X\quad |G|=|\Sigma_{x}|\cdot|\Omega(x)|$ ^72d803

$\:$
> Napomena: [[Red grupe i elementa. Indeks podgrupe#^d9c566|Dokaz]] [[Red grupe i elementa. Indeks podgrupe#^ebbac3|Košijeve teoreme]]

$\:$
**Stav**. $G$ dejstvuje na $X$. $\ \:$ $x$ i $y$ su iz iste orbite. Tada 
$\exists g\in G\ \ :\ \ \Sigma_{y}=g\Sigma_{x}g^{-1}$

**Stav**. $G$ dejstvuje na $X$. $\ \:$ $g,\,h\in G$ su konjugovani. Tada postoji bijekcija između $X^{g}$ i $X^{h}$.

**Teorema**. Konačna grupa $G$ dejstvuje na konačnom skupu $X$. Tada je broj različitih orbita jednak $\begin{align}\frac{1}{|G|}\sum\limits_{g\in G}|X^{g}|\end{align}$.
> Dokaz: Označimo broj različitih orbita $k$. $X=\Omega_{1}\sqcup\Omega_{2}\sqcup\dots\sqcup\Omega_{k}$.
> 
> Neka je $E:=\{(g,\,x)\in G\times X\ |\ g\cdot x =x\}$.
> Tada $x\in X^{g}\quad\Leftrightarrow\quad(g,\,x)\in E\quad\Leftrightarrow\quad g\in \Sigma_{x}$
> 
> Odakle, $\begin{align}\bigsqcup_{g\in G}\{g\}\times X^{g}=E=\bigsqcup_{x\in X}\Sigma_{x}\times \{x\}\end{align}$;
> 
> dalje, $\begin{align}\sum_{g\in G}|X^{g}|=|E|=\sum_{x\in X}|\Sigma_{x}|=\sum_{i=1}^{k}\sum_{x\in\Omega_{i}}|\Sigma_{x}|\end{align}$
> 
> $|\Sigma_{x}|=|\Sigma_{y}|$ za $x$ i $y$ iz iste orbite. Izabraćemo $x_{i}\in \Omega_{i}$, tada
>  $\begin{align}\sum_{g\in G}|X^{g}|=|E|=\sum_{i=1}^{k}|\Omega_{i}|\cdot|\Sigma_{x_{i}}|\overset{*}{=}\sum_{i=1}^{k}|G|=k|G|\end{align}$ $\quad$ ([[Dejstvo grupe#^72d803|*]])
>  Odakle sledi tvrđenje.