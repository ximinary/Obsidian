#note/not_linked nazad: [[Algebarska struktura]]
$\:$

**Def**. **Grupa** je [[Algebarska struktura|algebarska struktura]] $(G,\,\cdot)$, gde je $G$ neprazan skup a za binarnu operaciju $\cdot$ na $G$ važi:
- $\forall x,\,y,\,z\in G\quad(x\cdot y)\cdot z=x\cdot(y\cdot z)$
- $\forall e\in G\quad \forall x\in G\quad e\cdot x=x\cdot e=x$
- $\forall x\in G\quad\exists \overline{x}\in G\quad \overline{x}\cdot x=x\cdot\overline{x}=e$

$e$ je **neutral** grupe
**Stav**. Postoji jedinstven neutral.
> Dokaz: pps $e$ i $f$ su neutrali tada 
> ako je $e$ neutral onda $e\cdot f=f$
> ako je $f$ neutral onda $e\cdot f=e$
> odakle $e=f$, kontradikcija

$\overline{x}$ je **inverz** za $x$. Inverz se često označava sa $x^{-1}.$
**Stav**. Za svaki element grupe postoji jedinstven inverz.

**Def**. **Abelova** (komutativna) **grupa** je grupa $(G,\,\cdot)$ za koju važi: 
- $\forall x,\,y\in G\quad x\cdot y=y\cdot x$

Proizvod $\prod\limits_{i=1}^{n}x_{i},\quad x_{i}\in G$ se definiše rekurentnom formulom:
$\begin{cases}\prod\limits_{i=1}^{n}x_{i}=e,&n=0\\\prod\limits_{i=1}^{n}x_{i}=\prod\limits_{i=1}^{n-1}x_{i}\cdot x_{n},&n>0\end{cases}$

oznake:
$\prod\limits_{i=1}^{n}x_{i}=(x_{1}\cdots x_{n})$
$\prod\limits_{i=1}^{n}x=x^{n}$

pri tome za $-n<0$ definišemo $x^{-n}=\big(x^{-1}\big)^{n}$,
i važi $x^{0}=e$

**Def**. Za konačnu grupu možemo formirati **Kejlijevu tablicu**: vrste i kolone označavamo sa elementima grupe, a u preseku vrste označene sa $a$ i kolone označene sa $b$ zapisujemo element $a\cdot b$.


### Svojstva grupe
**Stav**. Neka je $(G,\,\cdot)$ grupa, $\ \:$ $n\geqslant2,\quad1\leqslant r<n$. 
Tada $(x_{1}\cdots x_{r})\cdot(x_{r+1}\cdots x_{n})=(x_{1}\cdots x_{n})$

**Stav**. Neka je $(G,\,\cdot)$ Abelova grupa. Tada ako $\{1,\,2,\,\dots,\,n\}=\{i_{1},\,i_{2},\,\dots,\,i_{n}\}$ onda $(x_{i_{1}}\cdots x_{i_{n}})=(x_{1}\cdots x_{n})$

**Stav**. Neka je $(G,\,\cdot)$ grupa. Tada $\big(x^{-1}\big)^{-1}=x$

**Stav**. Neka je $(G,\,\cdot)$ grupa. Tada $(x_{1}\cdots x_{n})^{-1}=(x_{n}^{-1}\cdots x_{1}^{-1})$

**Stav**. Neka je $(G,\,\cdot)$ grupa. Tada 
- jednačina $a\cdot x=b$ ima jedinstveno rešenje $x=a^{-1}\cdot b$
- jednačina $x\cdot a=b$ ima jedinstveno rešenje $x=b\cdot a^{-1}$

**Stav**. Neka je $(G,\,\cdot)$ grupa. Tada $(a\,x\,a^{-1})^{n}=a\,x^{n}\,a^{-1}$

$\:$
**Def**. $a\,x\,a^{-1}$ je **konjugovan** elementu $x$

$\:$
**Stav**. Neka je $(G,\,\cdot)$ grupa, $\:$ $x\in G$, $\:$ $n,\,m\in\mathbb{Z}$. $\:$ Tada
- $x^{n}\cdot x^{m}=x^{n+m}$
- $\big(x^{n}\big)^{m}=x^{nm}$

### Ciklična grupa
**Def**. Grupa $G$ je **ciklična** ako važi $G=\{x^{m}\ |\ m\in\mathbb{Z}\}$.
Element $x$ je **generator ciklične grupe** $G$.
Oznaka ciklične grupe generisane elementom  $G=\langle x\rangle$

### Diedarska grupa
Razmatramo simetrije pravilnog $n$-ugaonika:
$\varepsilon$ — neutral, identičko preslikavanje.
$\rho$  — rotacija za ugao $\begin{align}\frac{2\pi}{n}\end{align}$ u smeru suprotnom od kazaljke;
tada su $\rho,\,\rho^{2},\,\dots,\,\rho^{n-1}$ sve rotacije i $\rho^{n}=\varepsilon$.
$\sigma$ — neka osna refleksija;
tada su $\sigma,\,\sigma\rho,\,\sigma\rho^{2},\,\dots,\,\sigma\rho^{n-1}$ sve refleksije i $\sigma^{2}=\varepsilon$.

Skup $\{\varepsilon,\,\rho,\,\rho^{2},\,\dots,\,\rho^{n-1},\,\sigma,\,\sigma\rho,\,\sigma\rho^{2},\,\dots,\,\sigma\rho^{n-1}\}$ od $2n$ elemenata u odnosu na operaciju [[Kompozicija funkcija|kompozicije preslikavanja]] predstavlja **diedarsku grupu** $\mathbb{D}_{n}$ 

### Podgrupa
**Def**. Neka su $(G,\,\cdot)$ i $(H,\,*)$ dve grupe. $(H,\,\cdot)$ je **podgrupa** od $(G,\,*)$ ako 
$H\subseteq G$ $\quad$ i $\quad$ $\forall x,\,y\in H\quad x*y=x\cdot y$
Oznaka $H\leqslant G$.
Operacija $*$ je **restrikcija** operacije $\cdot$ na $H$.

**Stav**.
- Neutral u $G$ je jednak neutralu u $H$
- Ako je $x\in H$ onda inverz od $x$ u $G$ je jednak inverzu od $x$ u $H$

$\:$
**Stav**. Neprazan podskup $H$ grupe $G$ je podgrupa grupe $G$ u odnosu na restrikciju operacije iz $G$ akko $\forall x,\,y \in H\quad x\cdot y^{-1}\in H$
> Dokaz:
> $\boxed{\Rightarrow}$ $\quad$ $y\in H\quad\Rightarrow\quad y^{-1}\in H$, $\quad$ pa i $x\cdot y^{-1}\in H$
> $\boxed{\Leftarrow}$ $\quad$ Neka $H\ne\varnothing$ $\ \:$ i $\ \:$ $\forall x,\,y \in H\quad x\cdot y^{-1}\in H$
$\:$
**Stav**. Neka su $H$ i $K$ podgrupe grupe $G$, tada
- $H\cap K$ je podgrupa grupe $G$
- $H\cup K$ je podgrupa grupe $G$ akko $H\subseteq K$ ili $K\subseteq H$