#fax #math #alg  [deo [[Grupa|poglavlja "grupa"]]]
$\:$

**Def**. $G$ je grupa, $x,\,y\in G$. Element $y$ je **konjugovan** elementu $x$, ako $\exists g\in G\ \ :\ \ y = gxg^{-1}$

**Stav**. Konjugacija je relacija ekvivalencije.
**Klasa** (ekvivalencije) **konjugacije**: $K_{x}=\{gxg^{-1}\ \big|\ g\in G\}$

**Def**. $G$ je klasa, $H\leqslant G$. $H$ je normalna ako je $H$ unija nekih klasa konjugacije.
Oznaka: $H\triangleleft G$

> Primeri: $\{e\}\triangleleft G$, $\ \ \:$ $G\triangleleft G$, $\ \ \:$ $\langle \rho \rangle\triangleleft \mathbb{D}_{n},\ \ n\geqslant3$

$\:$
**Stav**.  $H\leqslant G$. Uslovi su ekvivalentni: ^b96173
1. $H\triangleleft G$ ^39f461
2. $\forall g\in G\quad gHg^{-1}\subseteq H$ ^c2938d
3. $\forall g\in G\quad gH=Hg$

> Dokaz: 
>  $\boxed{1.\Rightarrow2.}$ $h\in H$ proizvoljni.
>  Jer $H$ sastoji od klasa konjugacije, važi $h\in K_{h}$, tada $K_{h}\subseteq H$
>  (za bilo koji $g$, $ghg^{-1}\in H$), tj.  $gHg^{-1}\subseteq H$.
>   $\boxed{2.\Rightarrow3.}$ iz $2.$ množenjem celog skupa sleva sa $g^{-1}$ i zdesna sa $g$, dobijamo
>   $Hg^{-1}\subseteq g^{-1}H$ $\ \:$ i $\ \:$ $gH\subseteq Hg$ $\ \:$ za sve $g$. Odakle $gH=Hg$
>$\boxed{3.\Rightarrow1.}$ Neka je $K$ neka klasa konjugacije za koju $K\cap H\ne \varnothing$. Pokazati $K\subseteq H$.
>Neka je $h\in K\cap H$, tad je svaki element klase $K$ oblika $ghg^{-1}$.
>Iz $3.$ $gH=Hg$, odakle $\exists h'\in H\ \ :\ \ gh=h'g$, tj. $\ \:$ $h=ghg^{-1}\in H$
>Konačno, imamo $K\subseteq H$.

$\:$
**Stav**. Svaka podgrupa indeksa $2$ je normalna.
> Dokaz: $G$ je grupa. $H\leqslant G$ takva da $[G:H]=2$.
> Tada, $G=H\sqcup aH=H\sqcup Ha$, za bilo koji $a\not\in H$ 
> Jer $H\cap aH=\varnothing$ $\ \:$ i $\ \:$ $H\cap Ha=\varnothing$, $\ \:$ $aH=Ha,\quad a\not\in H$ 
> Ako je $a\in H$, $aH=H=Ha$.
> Iz prethodnog stava $3.\Rightarrow1.$ sledi tvrđenje.


$\:$
**Def**. $G$ je grupa. Centar grupe $G$ je
$Z(G):=\{g\in G\ \big|\ \forall x\in G\quad xg=gx\}$

**Stav**. $Z(G)\triangleleft G$.
> Dokaz: Prvo dokažemo $Z(G)\leqslant G$
> - Asocijativnost se čuva.
> - Neutral: kako je $ex=xe$ za sve $x\in G$, $e\in Z(G)$.
> - Inverz: neka je $g\in Z(G)$, tad $gx=xg$ za sve $x\in G$.
>   Odakle množenjem sa $g^{-1}$ sa obe strane, $xg^{-1}=g^{-1}x$, tj. $g^{-1}\in Z(G)$
>  - Zatvorenost: Neka su $g,\,h\in Z(G)$, tad
>    $gx=xg$ $\ \:$ i $\ \:$ $hx=xh$ $\ \:$ za sve $x\in G$
>    $(gh)x=g(hx)=g(xh)=(gx)h=(xg)h=x(gh)$, tj. $gh\in Z(G)$
>  
>   Dokažemo $g\in Z(G)\quad\Leftrightarrow\quad K_{g}=\{g\}$
>   $\ \ \quad$ $\boxed{\Rightarrow}$ $\forall x\in G\quad gx=xg$, $\ \:$ tj. $g=xgx^{-1}$. Odakle $K_{g}=\{g\}$.
>   $\ \ \quad$ $\boxed{\Leftarrow}$ $K_{g}=\{g\}\quad\forall  x\in G\quad g=xgx^{-1}$. $\ \:$ $g\in Z(G)$
>   Dakle, $Z(G)$ je unija jednočlanih klasa konjugacije, tj. $Z(G)\triangleleft G$.

$\:$
**Stav** & **Def**. $G$ je grupa, $H\triangleleft G$. Skup levih koseta podgrupe $H$ čini grupu u odnosu na operaciju množenja podskupova $G$ $\Big(X\cdot Y=\{x\cdot y\ \big|\ x\in X,\ \ y\in Y\},\quad X,\,Y\subseteq G\Big)$.
Ova grupa $(G/H,\ \cdot)$ zove se **količnička grupa** grupe $G$ po normalnoj grupi $H$.
> Dokaz:  $H\triangleleft G$.
> $aH$ i $bH$ su proizvoljni koseti.
> 
> Zatvorenost: treba pokazati $(aH)\cdot(bH)=(ab)H$
> Važi $H\cdot H\subseteq H$ (proizvod dva el. iz $H$ je iz $H$ jer je $H$ grupa)
> kao i $H\cdot H\supseteq H=eH$, jer $e\in H$. Odakle $H\cdot H=H$
> Iz [[Normalne podgrupe#^b96173|stava]] $1.\Rightarrow3.$ $bH=Hb$
> Konačno, imamo $(aH)\cdot(bH)=a(Hb)\cdot H=(ab)H\cdot H=(ab)H$
> 
> Asocijativnost: $\big((aH)\cdot(bH)\big)\cdot(cH)=\big((ab)H\big)\cdot(cH)=(abc)H=(aH)\cdot\big((bc)H\big)=(aH)\cdot\big((bH)\cdot(cH)\big)$
> Neutral: $H=eH$ je neutral, naime $(aH)\cdot H=H\cdot(aH)=aH$
> Inverz: inverz elementa $aH$ je element $a^{-1}H$, naime $(aH)\cdot(a^{-1}H)=(a^{-1}H)\cdot(aH)=eH=H$
> 