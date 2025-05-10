#fax #math #alg [deo [[Algebarska struktura|poglavlja "algebarska struktura"]]]
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
**Stav**. Neprazan podskup $H$ grupe $G$ je podgrupa grupe $G$ u odnosu na restrikciju operacije iz $G$ akko $\forall x,\,y \in H\quad x\cdot y^{-1}\in H$
> Dokaz:
> $\boxed{\Rightarrow}$ $\quad$ $y\in H\quad\Rightarrow\quad y^{-1}\in H$, $\quad$ pa i $x\cdot y^{-1}\in H$
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
$X$ je **skup generatora** te podgrupe.

$X^{-1}=\{x^{-1}\ |\ x\in X\}$ je skup svih inverza elemenata iz $X$.
**Stav**. $\langle X\rangle =\{(a_{1}\cdots a_{n})\ |\ n\in \mathbb{N}_{0},\,a_{i}\in X\cup X^{-1}\}$
(ako je $n=0$, imamo neutral $e$)

### Red grupe i elementa
**Def**. Ako je $G$ konačna grupa, onda broj njenih elemenata zovemo **red grupe** i označavamo sa $|G|$. Ako je grupa beskonačna, kažemo da je ona **beskonačnog reda**.

**Def**. Neka je $a$ element neke grupe. Ako postoji $n\geqslant1$ za koji važi $a^{n}=e$, onda je **red elementa** $a$ jednak $\omega(a)=\min\{m\geqslant1\ |\ a^{m}=e\}$, inače je $a$ **beskonačnog reda**.

**Stav**. Red bilo kojeg elementa grupe je jednak redu podgrupe generisane tim elementom.
> Dokaz: Neka je podgrupa $\langle a\rangle$ generisana elementom $a$.
> 
> Ako je $a$ beskonačnog reda, važi $\forall n\geqslant 1\quad a^{n}\ne e$
> Da li neke za neke $l> m$ može važiti $a^{l}=a^{m}$?
> Pomnožimo jednačinu sa $a^{-m}$, imamo $a^{l-m}=e$, pri tome $l - m \geqslant 1$. Kontradikcija, važi da su sve $a^{n}$ različite za različite $n$, stoga $\langle a\rangle$ ima beskonačno mnogo elemenata.
> 
> Ako je $a$ reda $n\geqslant 1$, tj. $\ \:$ $a^{n}=e$ $\ \:$ i $\ \:$ $\forall m=\overline{1,\,n\!-\!1}\quad a^{n}\ne e$
> Stoga, $\forall m\in\mathbb{Z}\quad \exists r=\overline{1,\,n\!-\!1}\quad a^{m}=a^{n\cdot k+r}=(a^{n})^{k}\cdot a^{r}=e^{k}\cdot a^{r}=a^{r}$
> Imamo, $\langle a\rangle=\{e,\,a,\,a^{2},\,\dots,\,a^{n-1}\}$
> Da li taj skup sadrži ponavljajuće elemente? Pretpostavimo da za neke $0\leqslant m < l< n$ važi $a^{l}=a^{m}$, tj. $a^{l-m}=e$, 
> $l-m< n$, kontradikcija jer je $n$ najmanji broj za koji važi $a^{n}=e$.
> Dakle, skup ne sadrži ponavljajuće elemente i samim tim je red $\langle a\rangle$ jednak $n$.

$\:$
**Stav**. Neka je $a$ reda $n$. Tada
$\forall m\in\mathbb{Z}\quad\big(a^{m}=e\quad\Leftrightarrow\quad n\,|\,m\big)$

$\:$
**Stav**. Neka je $m\in\mathbb{Z}\setminus \{0\}$.
Ako je $a$ beskonačnog reda, onda je i $a^{m}$ beskonačnog reda;
ako je $a$ reda $n$, onda je $a^{m}$ reda $\begin{align}\frac{n}{\mathrm{NZD}(m,\,n)}\end{align}$. ^1698b9
> Dokaz:
> $a$ je beskonačnog reda, tj. $\forall n\in\mathbb{Z}\quad a^{n}\ne e$
> Odakle $\forall n\in\mathbb{Z}\quad a^{m\cdot n}\ne e$, tj. $a^{m}$ je beskonačnog reda.
>
>$a$ je reda $n$. Neka je $d=\mathrm{NZD}(m,\,n)$, tada
>$m = m_{1}\cdot d$ $\ \:$ i $\ \:$ $n=n_{1}\cdot d$, $\ \:$ pri tome $\mathrm{NZD}(m_{1},\,n_{1})=1$
> Pokazati da je $a^{m}$ reda $n_{1}$.
> $\big(a^{m}\big)^{n_{1}}=a^{m_{1}\cdot d\cdot n_{1}}=a^{n\cdot m_{1}}=e^{m_{1}}=e$, da li je $n_{1}$ najmanji ($\geqslant1$)-broj za koji to važi?
> pps: neka je $1\leqslant k< n_{1}\ \ :\ \ \big(a^{m}\big)^{k}=e$  — najmanji broj za koji to važi.
> tada $\exists r\in\overline{0,\,k\!-\!1}\ \:\ \ n_{1}=p\cdot k+r$
> $e=\big(a^{m}\big)^{n_{1}}=\big(a^{m}\big)^{p\cdot k+r}=a^{r}$
> $\big(a^{m}\big)^{r}=e$ i $r<k$, kontradikcija. $n_{1}$ jeste najmanji.

$\:$
**Teorema**. 
1. Svaka podgrupa ciklične grupe i sama je ciklična.
2. $G$ je ciklična grupa reda $n$. Tada
  $k\,|\,n\quad\Rightarrow\quad\exists!H\leqslant G\ \ \:\ \ |H|=k$

> Dokaz: 
> 1. Neka je $G= \langle a \rangle$ i $H\leqslant G$.
> $H=\{e\}$ jeste ciklična, razmatramo proizvoljnu $H\ne\{e\}$.
> Neka je $s=\min\{t>0\ |\ a^{t}\in H\}$. Pokazati da $H= \langle a^{s}\rangle$.
> $a^{s}\in H\quad\Rightarrow\quad\Big(\forall k\in\mathbb{Z}\quad \big(a^{s}\big)^{k}\in H\Big)\quad\Rightarrow\quad\langle a^{s} \rangle\subseteq H$
> pps $H\not\subseteq \langle a^{s} \rangle$, $\ \:$tj. $\exists x\in H\ \ :\ \ x\not\in \langle a^{s} \rangle$
> $x\in H\quad\Rightarrow\quad x\in G\quad\Rightarrow\quad\Big(\exists m\in\mathbb{Z}\ \ :\ \ x=a^{m}\Big)$
> $\exists r=\overline{0,\,s-1}\quad m = p\cdot s+r$
> Tada $a^{r}=a^{m-ps}=x\cdot(a^{s})^{-p}\in H$, $\ \:$ jer $x,\,a^{s}\in H$
> Jer je $s$ najmanji pozitivan broj za koji $a^{s}\in H$, a $0\leqslant r<s$, sledi da $r =0$, tj. $m=p\cdot s$
> $x=a^{m}=a^{p\cdot s}=\big(a^{s}\big)^{p}\in \langle a^{s} \rangle$. Kontradikcija
> $H=\langle a^{s} \rangle$
> $\:$
> 2. Neka je $G=\langle a \rangle$ reda $n$ i $k\,|\,n$.
> iz [[Grupa#^1698b9|stava]] $\langle a^{n/k} \rangle$ je reda $\begin{align}\frac{n}{\mathrm{NZD}(n,\,n/k)}=\frac{n}{n/k}=k\end{align}$
> $H:=\langle a^{n/k} \rangle$, pretpostavimo da postoji i druga podgrupa $\widetilde{H}$ reda $k$ odlična od $H$.
> iz 1. $\widetilde{H}$ je ciklična, tj. $\widetilde{H}=\langle a^{l} \rangle$.
> $a^{lk}=\big(a^{l}\big)^{k}=e$ (jer je $\widetilde{H}$ reda $k$)
> a $G$ je reda $n$ ($a^{n}=e$), imamo da $n\,|\,lk$
> iz $k\,|\,n$ dobijamo da $\begin{align}\frac{n}{k}\,\bigg|\,l\end{align}$, $\ \:$ tj $\begin{align}l=p\cdot\frac{n}{k}\end{align}$, za neko $p\in\mathbb{Z}$.
> $a^{l}=\big(a^{n/k}\big)^{p}\in H$, odakle $\widetilde{H}\subseteq H$ i kako $|H|=|\widetilde{H}|$ važi da $H=\widetilde{H}$.
> Kontradikcija.
> $H=\langle a^{n/k} \rangle$ je jedinstvena podgrupa reda $k$.

$\:$
### Izomorfizam grupa
**Def**. Neka su $(G,\,\cdot)$ i $(H,\,*)$ grupe. $G$ i $H$ su **izomorfni** ako postoji bijekcija $f:\ G\to H$ takva da $\forall x,\,y\in G\quad f(x\cdot y)=f(x)*f(y)$. $f$ je **izomorfizam grupa** $G$ i $H$.
Oznaka: $G\cong H$

**Stav**. Ako je $f:\ G\to H$ izomorfizam grupa, onda je i $f^{-1}$ izomorfizam grupa.
> Dokaz: Jer je $f$ bijekcija, $f^{-1}:\ H\to G$ jeste bijekcija.
> Pokazati da $\forall u,\,v\in H\quad f^{-1}(u*v)=f^{-1}(u)\cdot f^{-1}(v)$
> 
> Jer je $f$ surjekcija $\exists x,\,y\in G\ \ :\ \ f(x)=u\ \ \text{i}\ \ f(y)=v$
> $f^{-1}(u*v)=f^{-1}\big(f(x)*f(y)\big)\xlongequal{f\ \text{ je izomorfizam}}f^{-1}\big(f(x\cdot y)\big)=x\cdot y=f^{-1}(u)\cdot f^{-1}(v)$

$\:$
**Stav**. Neka je $e$ neutral u $G$, $\varepsilon$ neutral u $H$, i $f:\ G\to H$ izomorfizam. Tada
- $f(e)=\varepsilon$
- $\forall x\in G\quad f(x^{-1})=f(x)^{-1}$
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
