#fax #math #alg [deo [[Algebarska struktura|poglavlja "algebarska struktura"]]]
$\:$  ^21d3b8


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

**Def**. **Abelova** (komutativna) **grupa** je grupa $(G,\,\cdot)$ za koju važi:  ^9d2aa9
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


### Diedarska grupa
Razmatramo simetrije pravilnog $n$-ugaonika:
$\varepsilon$ — neutral, identičko preslikavanje.
$\rho$  — rotacija za ugao $\begin{align}\frac{2\pi}{n}\end{align}$ u smeru suprotnom od kazaljke;
tada su $\rho,\,\rho^{2},\,\dots,\,\rho^{n-1}$ sve rotacije i $\rho^{n}=\varepsilon$.
$\sigma$ — neka osna refleksija;
tada su $\sigma,\,\sigma\rho,\,\sigma\rho^{2},\,\dots,\,\sigma\rho^{n-1}$ sve refleksije i $\sigma^{2}=\varepsilon$.

Skup $\{\varepsilon,\,\rho,\,\rho^{2},\,\dots,\,\rho^{n-1},\,\sigma,\,\sigma\rho,\,\sigma\rho^{2},\,\dots,\,\sigma\rho^{n-1}\}$ od $2n$ elemenata u odnosu na operaciju [[Kompozicija funkcija|kompozicije preslikavanja]] predstavlja **diedarsku grupu** $\mathbb{D}_{n}$ 

### Ciklična grupa
**Def**. Grupa $G$ je **ciklična** ako važi $G=\{x^{m}\ |\ m\in\mathbb{Z}\}$.
Element $x$ je **generator ciklične grupe** $G$.
Oznaka ciklične grupe generisane elementom $x$: $G=\langle x\rangle$

### Podgrupa
**Def**. Neka su $(G,\,\cdot)$ i $(H,\,*)$ dve grupe. $(H,\,\cdot)$ je **podgrupa** od $(G,\,*)$ ako 
$H\subseteq G$ $\quad$ i $\quad$ $\forall x,\,y\in H\quad x*y=x\cdot y$
Oznaka $H\leqslant G$.
Operacija $*$ je **restrikcija** operacije $\cdot$ na $H$.

**Stav**.
- Neutral u $G$ je jednak neutralu u $H$
- Ako je $x\in H$ onda inverz od $x$ u $G$ je jednak inverzu od $x$ u $H$

$\:$
**Stav**. Neprazan podskup $H$ grupe $G$ je podgrupa grupe $G$ u odnosu na restrikciju operacije iz $G$ akko $\forall x,\,y \in H\quad x\cdot y^{-1}\in H$ ^2ea486
> Dokaz:
> $\boxed{\Rightarrow}$ $\quad$ $x,\,y\in H\quad\Rightarrow\quad y^{-1}\in H$, $\quad$ pa i $x\cdot y^{-1}\in H$
> $\boxed{\Leftarrow}$ $\quad$ Neka $H\ne\varnothing$ $\ \:$ i $\ \:$ $\forall x,\,y \in H\quad x\cdot y^{-1}\in H$
> Jasno je da je asocijativnost sačuvana u svakom podskupu grupe.
> $h\in H\quad\Rightarrow\quad e=h\cdot h^{-1}\in H$ — neutral
> $h,\,e\in H\quad\Rightarrow\quad h^{-1}=e\cdot h^{-1}\in H$ — inverz
> $x,\,y \in H$, odakle $y^{-1}\in H$ $\quad\Rightarrow\quad x\cdot y=x\cdot\big(y^{-1}\big)^{-1}\in H$ — zatvorenost operacije

$\:$
**Stav**. Neka su $H$ i $K$ podgrupe grupe $G$, tada
- $H\cap K$ je podgrupa grupe $G$
- $H\cup K$ je podgrupa grupe $G$ akko $H\subseteq K$ ili $K\subseteq H$

> Dokaz:
> - prvo tvrđenje
> 
> $e\in G$ je neutral $\quad \Rightarrow\quad e\in H,\ e\in K\quad\Rightarrow\quad e \in H\cap K$
> Neka su $x,\,y\in H\cap K$;
> iz prethodnog stava $x\cdot y^{-1}\in H,\ x\cdot y^{-1}\in K$, pa $x\cdot y^{-1}\in H\cap K$;
> ponovo na osnovu prethodnog stava $H\cap K$ je podgrupa od $G$.
> 
> - drugo tvrđenje
> 
> $\boxed{\Leftarrow}$
> $H\subseteq K\quad\Rightarrow\quad H\cup K =K$ jeste podgrupa od $G$;
> $K\subseteq H\quad\Rightarrow\quad H\cup K =H$ jeste podgrupa od $G$.
> $\boxed{\Rightarrow}$ $H,\,K,\,H\cup K$ su podgrupe od $G$
> pps: $H\not\subseteq K$ i $K\not\subseteq H$, 
> tj. $\exists k\in K\quad k\not\in H$ $\quad$ i $\quad$ $\exists h\in H\quad h\not\in K$ $\quad$
> 
> $k,\,h\in K\cup H\quad\Rightarrow\quad k\cdot h\in K\cup H$
> tada važi $k\cdot h\in K$ ili $k\cdot h\in H$
> $\left.\begin{array}{l}k\cdot h \in K\\k^{-1}\in K\end{array}\ \ \right|\Rightarrow k^{-1}\cdot k\cdot h=h \in K\quad$ kontradikcija
> 
> $\left.\begin{array}{l}k\cdot h \in H\\h^{-1}\in H\end{array}\ \ \right|\Rightarrow k\cdot h\cdot h^{-1}=k \in H\quad$ kontradikcija

$\:$
**Def**. Najmanja podgrupa koja sadrži podskup $X$ grupe $G$ (odnosno presek svih podgrupa grupe $G$ koje sadrže $X$) zove se **podgrupa generisana skupom** $X$.
Oznaka: $\langle X\rangle$
$X$ je **skup generatora** te podgrupe. ^eb2fd0

$X^{-1}=\{x^{-1}\ |\ x\in X\}$ je skup svih inverza elemenata iz $X$.

**Stav**. $\langle X\rangle =\{(a_{1}\cdots a_{n})\ |\ n\in \mathbb{N}_{0},\,a_{i}\in X\cup X^{-1}\}$
(ako je $n=0$, imamo neutral $e$)

### [[Red grupe i elementa. Indeks podgrupe]]

### Izomorfizam grupa
**Def**. Neka su $(G,\,\cdot)$ i $(H,\,*)$ grupe. $G$ i $H$ su **izomorfni** ako postoji bijekcija $f:\ G\to H$ takva da $\forall x,\,y\in G\quad f(x\cdot y)=f(x)*f(y)$. $f$ je **izomorfizam grupa** $G$ i $H$.
Oznaka: $G\cong H$
> Napomena: izomorfizam je specijalan slučaj [[Homomorfizam grupa|homomorfizma]].

$\:$
**Stav**. Ako je $f:\ G\to H$ izomorfizam grupa, onda je i $f^{-1}$ izomorfizam grupa.
> Dokaz: Jer je $f$ bijekcija, $f^{-1}:\ H\to G$ jeste bijekcija.
> Pokazati da $\forall u,\,v\in H\quad f^{-1}(u*v)=f^{-1}(u)\cdot f^{-1}(v)$
> 
> Jer je $f$ surjekcija $\exists x,\,y\in G\ \ :\ \ f(x)=u\ \ \text{i}\ \ f(y)=v$
> $f^{-1}(u*v)=f^{-1}\big(f(x)*f(y)\big)\xlongequal{f\ \text{ je izomorfizam}}f^{-1}\big(f(x\cdot y)\big)=x\cdot y=f^{-1}(u)\cdot f^{-1}(v)$

$\:$
**Stav**. Neka je $e$ neutral u $G$, $\varepsilon$ neutral u $H$, i $f:\ G\to H$ izomorfizam. Tada
- $f(e)=\varepsilon$ ^60085a
- $\forall x\in G\quad f(x^{-1})=f(x)^{-1}$ ^9b7621
- $\forall x\in G\quad$ ako je $x$ beskonačnog reda, onda je i $f(x)$ beskonačnog reda; 
  $\ \quad\quad\quad\quad$ ako je $x$ konačnog reda, onda $\omega\big(x\big)=\omega\big(f(x)\big)$

> Dokaz:
> - $f(e)=f(e\cdot e)=f(e)*f(e)\quad\Rightarrow\quad\varepsilon=f(e)$
> - $\varepsilon=f(e)=f(x\cdot x^{-1})=f(x)*f(x^{-1})\quad\Rightarrow\quad f(x^{-1})=f(x)^{-1}$
>  - pps: $x$ je beskonačnog reda, a $f(x)$ konačnog, tj. $\exists n\in\mathbb{N}\ \ :\ \ f(x)^{n}=\varepsilon$. 
>    imamo $\varepsilon=f(x)^{n}=f(x)*\cdot\!\cdot\!\cdot*f(x)=f(x\cdot \cdot\!\cdot\!\cdot \cdot x)=f(x^{n})\quad\Rightarrow\quad x^{n}=e$ 
>    ($x$ je reda $n$). Kontradikcija
>    
>    Neka je $x$ reda $n$, pokazati da je $f(x)$ reda $n$.
>    $e=x^{n}\quad\Rightarrow\quad \varepsilon=f(x^{n})=f(x)^{n}$, tj. je $f(x)$ konačnog reda.
>    Pretpostavimo da $n$ nije najmanji broj takav da $f(x)^{n}=\varepsilon$, a $m$ jeste ($f(x)$ je reda $m$). Tada $\exists r=\overline{0,m\!-\!1} \quad n=p\cdot m +r$.
>    $f(x)^{r}=f(x)^{n-p\cdot m}=f(x)^{n}*\big(f(x)^{m}\big)^{-p}=\varepsilon$, jer je $m$ najmanji takav pozitivan broj, $r=0$, tj. $m\,|\,n$.
>    $\varepsilon=f(x)^{m}=f(x^{m})\quad\Rightarrow\quad e=x^{m}$, odakle  $n\,|\,m$, jer je $x$ reda $n$.
>    konačno imamo $n=m$.   

$\:$
**Teorema**. Svaka ciklična grupa je izomorfna ili grupi $\mathbb{Z}$ ili grupi $\mathbb{Z}_{n},\quad n\in\mathbb{N}$.
> Dokaz:
> Neka je $G$ beskonačna ciklična grupa, tada $\exists a\in G\ \ :\ \ G= \langle a \rangle$. Definišemo $f:\ \mathbb{Z}\to G$ $\ \:$ sa $\ \:$ $f(m)=a^{m}$, koja jeste bijekcija. Važi i $f(m+k)=f(m)\cdot f(k)$, jer $a^{m+k}=a^{m}\cdot a^{k}$. Stoga je $f$ izomorfizam i $G\cong \mathbb{Z}.$
> 
> Neka je $G$ reda $n$, $G=\{e,\,a,\,\dots,\,a^{n-1} \}$. Slično prethodnom definišemo $f:\ \mathbb{Z}_{n}\to G$ $\ \:$ sa $\ \:$ $f(m)=a^{m}$, koja je bijekcija. Pokazati $f(m+_{n}k)=f(m)\cdot f(k)$.
> $m+k=(m+_{n}k)+p\cdot n\quad\Rightarrow\quad f(m+_{n}k)=f(m+k-p\cdot n)=a^{m}\cdot a^{k}\cdot \big(\underbrace{a^{n}}_{=\, e}\big)^{-p}=f(m)\cdot f(k)$ Stoga je $f$ izomorfizam i $G\cong \mathbb{Z}_{n}.$

$\:$
### [[Grupa permutacija]]
> Napomena: $\mathbb{D}_{3}\cong \mathbb{S}_{3}$

$\:$
**Teorema** (Kejlijeva). Svaka grupa $G$ izomorfna je nekoj podgrupi grupe $\mathbb{S}_{G}$
> Dokaz:
> Neka je $g\in G$. Definišemo fju $L_{g}:\,G\to G$ sa $L_{g}(x)=g\cdot x$ 
> $(L_{g}\circ L_{h})(x)=L_{g}(h\cdot x)=g\cdot h\cdot x=(g\cdot h)\cdot x=L_{g\cdot h}(x)$
> $\forall x\in G\quad L_{e}(x)=x$, tj. $L_{e}=\mathrm{id}_{G}$
> Dakle, $(L_{g})^{-1}=L_{g^{-1}}$
> Važi $L_{g}\circ (L_{h})^{-1}=L_{g\cdot h^{-1}}$
> [[Grupa#^2ea486|Stoga]], $G'=\{L_{g}\ |\ g\in G\}\leqslant \mathbb{S}_{G}$
> Definišemo fju $f:\ G\to G'$ sa $f(g)=L_{g}$, koja jeste bijekcija i važi 
> $f(g\cdot h)=L_{g\cdot h}=L_{g}\circ L_{h}=f(g)\circ f(h)$
> Tj. je $f$ izomorfizam grupa $G$ i $G'\leqslant\mathbb{S}_{n}.$

$\:$
**Posledica**. Svaka konačna grupa $G$ reda $n$ izomorfna je nekoj podgrupi grupe $\mathbb{S}_{n}$

### [[Direktan proizvod grupa]]
### [[Normalne podgrupe]]
### [[Homomorfizam grupa]]
### [[Dejstvo grupe]]
### [[Konačno generisana Abelova grupa]]