#fax #math #alg [deo [[Komutativan prsten sa jedinicom|poglavlja "prsten"]]]

### Prsten polinoma
Skup svih polinoma sa koeficijentima u komutativnom prstenu sa jedinicom $A$ u sa neodređenom $X$ je $A[X]=\{a_{0}+a_{1}X+\dots+a_{n}X^{n}\ \ \big|\ \ n\in \mathbb{N},\ \ a_{i}\in A\}$ uz operacije $+'$ i $\cdot'$ čini komutativan prsten sa jedinicom:
- $(a_{0}+a_{1}X+\dots+a_{n}X^{n})+'(a'_{0}+a'_{1}X+\dots+a'_{m}X^{m})=(a_{0}+a'_{0})+(a_{1}+a'_{1})X+\dots+(a_{m}+a'_{m})X^{m}+ a_{m+1}X^{m+1}+\dots+a_{n}X^{n}$
  za $m\leqslant n$ i gde je $+$ operacija u $A$.
- $\begin{align}(a_{0}+a_{1}X+\dots+a_{n}X^{n})\cdot'(a'_{0}+a'_{1}X+\dots+a'_{m}X^{m})=\sum\limits_{k=0}^{n+m}\bigg(\sum\limits_{i=0}^{k}a_{i}\cdot a'_{k-i}\bigg)X^{k}\end{align}$
  gde su $\cdot$ i $+$ operacije u $A$.

$\:$
**Stav**. Sa $f\big(a(X)\big)=p(i)$ definisan je homomorfizam $f:\ \mathbb{R}[X]\to \mathbb{C}$. 

**Def**. Neka je $F$ polje. Polinom $p\in F[X]$ je **nerastavljiv** nad poljem $F$, ako
$\forall s,\,t\in F[X]$ — stepena bar jedan $\quad$ $s\cdot t\ne p$

**Teorema**. Neka je $F$ polje i neka je $a(X)\in F[X]\setminus\{0\}$ <u>nerastavljiv</u> polinom. Tada za  $E=F[X]\big/\big\langle a(X)\big\rangle$ važi: ^a01330
- $E$ je polje  ^ea3d8d
- $E$ sadrži potpolje izomorfno polju $F$
- $a(X)$ ima bar jednu nulu u $E$ 
- dimenzija [[Vektorski prostor|vektorskog prostora]] $E$ nad poljem $F$ je jednaka stepenu polinoma $a(X)$.

> Dokaz:
> Označimo [[Potprsten i ideal|ideal]] $\big\langle a(X) \big\rangle$ u prstenu $F[X]$ sa $I$,
> tada $E=\big\{b(X)+I\ \big|\ b(x)\in F[X]\big\}$.
> $E$ jeste komutativan prsten sa jedinicom ([[Potprsten i ideal#Kongruencija po idealu|*]]).
> - Pokazati da svaki nenula element $E$ ima inverz:
>   $0_{E}=I$. $\quad$ Za $b(X)+I\ne I$ naći inverz
>   Jer $b(X)+I\ne I$, $\ \:$ $b(X)\not\in I$
>   i kako je $a(X)$ nerastavljiv, $\ \:$ $\mathrm{NZD}(a,\,b)=1$.
>   Tada $\exists p(X),\,q(X)\in F[X]\quad p(X)a(X)+q(X)b(X)=1$
>   Prelazimo na $E$: $\ \:$ $\big(p(X)a(X)+I\big)+\big(q(X)b(X)+I\big)=1 + I$
>   Kako je $a(X)\in I$, dobijamo $\big(q(X)+I\big)\big(b(X)+I\big)=1+I$
>   Tj. $q(X)$ je inverz od $b(X)$.
>   $\:$
> - Neka je $\:$ $f:\ F\to E$ $\:$ fja def. sa $\:$ $f(\alpha)=\alpha+I$, koja jeste homomorfizam.
>   Kako je $\mathrm{Ker}\,f$ [[Homomorfizam komutativnih prstena sa jedinicom#^131642|ideal]] i kako [[Potprsten i ideal#^680460|ideal polja]] je ili $\{0\}$ ili celo polje, važi $\mathrm{Ker}\,f=\{0\}$; [[Homomorfizam komutativnih prstena sa jedinicom#^2420ae|stoga]] $f$ je "1-1".
>   Tada $F\cong \mathrm{Im}\,f$
>   $\:$
> - Neka je $a(X)=a_{0}+a_{1}X+\dots+a_{n}X^{n}$ polinom nad $F$, 
>    i neka $X+I\in E$. $\:$ Tada $\begin{align}a(X+I)&=(a_{0}+I)+(a_{1}+I)(X+I)+\dots+(a_{n}+I)(X+I)^{n}=\\&=(a_{0}+a_{1}X+\dots+a_{n}X^{n})+I=a(X)+I=I \end{align}$
>    $\:$
>  - Kako $F\subset E$, $\:$ $E$ čini [[Vektorski prostor|vektorski prostor]].
>    Pokažemo da je dimenzija $E$ jednaka stepenu polinoma $a(X)$, da je $[1+I,\,X+I,\,\dots,\,X^{n-1}+I]$ [[Linearna zavisnost i nezavisnost. Skup generatora, baza i dimenzija VP-a#Baza i dimenzija|baza]] tog VP ($n$ je stepen polinoma $a(X)$).
>    
>    Da li je to [[Linearna zavisnost i nezavisnost. Skup generatora, baza i dimenzija VP-a#Skup generatora|skup generatora]]?
>    Za bilo koji $b(X)+I\in E$
>    $b(X)=\underbrace{q(X)a(X)}_{\in I}+r(X),\ \:$ stepen polinoma $r$ je strogo manji $n$.
>    $r(X)=r_{0}+r_{1}X+\dots+r_{n-1}X^{n-1}$
>    Tada $b(x)+I=r_{0}(1+I)+r_{1}(X+I)+\dots+r_{n-1}(X^{n-1}+I)$
>    
>    Da li je to [[Linearna zavisnost i nezavisnost. Skup generatora, baza i dimenzija VP-a#^004a66|linearno nezavisan]] skup?
>    Neka nije: $\exists c_{0},\,c_{1},\,\dots,\,c_{n-1}\in F\quad c_{0}(1+I)+c_{1}(X+I)+\dots+c_{n-1}(X^{n-1}+I)=0+I$
>    Neka  $\:$ $c(x)=c_{0}+c_{1}X+\dots+c_{n-1}X^{n-1}$
>    Tada imamo $\:$ $c(X)+I=I\quad\Rightarrow\quad c(X)\in I=\big\langle a(X) \big\rangle$,
>    $c$ je stepena $n-1$, a $a$ stepena $n$ generiše $I$. Kontradikcija.

$\:$
**Def**. Ako polje $E$ sadrži potpolje izomorfno polju $F$, onda kažemo da je polje $E$ **raširenje polja** $F$. 
Tada je $E$ vektorski prostor nad $F$, a dimenziju raširenja zovemo **stepen raširenja**, koju označavamo sa $[E:F]$.

$\:$
> Konstruisanje polja sa $p^{n}$ elemenata, gde je $p$ prost i $n\in \mathbb{N}$:
> Nađemo nerastavljiv polinom $a(X)\in\mathbb{Z}_{p}[X]$ stepena $n$.
> Tada je $\mathbb{Z}_{p}[X]/\big\langle a(X)\big\rangle$ VP dimenzije $n$ nad $\mathbb{Z}_{p}$, tj. ima $p^{n}$ elemenata.
> A iz prethodne teoreme znamo da je to polje.

$\:$
**Posledica**. $F$ je polje i $a(X)\in F[X]$. Tada postoji raširenje $E$ polja $F$ u kojem se $a(X)$ faktoriše na linearne faktore.

**Def**. Neka je $F$ polje i $a(X)\in F[X]\setminus\{0\}$. **Korensko polje** polinoma $a(X)$ je najmanje raširenje polja $F$ u kojem se $a(X)$ faktoriše na linearne faktore.

### Algebarska raširenja
**Def**. Neka je $F$ potpolje do $\mathbb{C}$. Tada je  $\alpha$ **algebarski** nad $F$ ako postoji polinom $p(X)\in F[X]$ za koji  $p(\alpha)=0$.

**Stav**. Neka je $F$ pole. Tada je svaki ideal u $F[X]$ [[Potprsten i ideal#^938480|glavni]].

$F[\alpha]:=\big\{p(\alpha)\ \big|\ p(X)\in F[X]\big\}$

**Stav**. Neka je $F$ potpolje od $\mathbb{C}$ $\:$ i $\:$ $\alpha\in \mathbb{C}$. Tada je $F[\alpha]$ polje akko je $\alpha$ algebarski nad $F$.
> Dokaz: 
> $\boxed{\Rightarrow}$ Neka je $F[\alpha]$ polje.
> Tada i element $\:$ $\alpha\in F[\alpha]$ $\:$ ima inverz: $\:$ $\exists b\in F[\alpha]\setminus\{0\}\quad \alpha\cdot b=1$
> za $b\quad\exists q(X)\quad b=q(\alpha)$
> Stoga $\alpha\cdot q(\alpha)-1=0$, $\ \:$ tj. $\:$ $X\cdot q(X)-1$ $\:$ je traženi polinom.
> 
> $\boxed{\Leftarrow}$ Kako je $\alpha$ algebarski nad $F$,  skup $I=\big\{p(X)\in F[X]\ \ \big|\ \ p(\alpha)=0\big\}$ nije prazan.
> $I$ jeste ideal u $F[X]$, jer $\forall p(X),\,q(X)\in I\quad p(\alpha)=q(\alpha)=0$; odakle $p(\alpha)+q(\alpha)=0$ $\ \:$ i $\ \:$ $\forall f(X)\in F[X],\ \ p(X)\in I\quad f(\alpha)\cdot p(\alpha)=f(\alpha)\cdot 0=0$.
> 
> Iz prethodnog stava $\exists \mu(X) \text{ − moničan}\quad I=\big\langle\mu(X)\big\rangle$
> 
> $\mu(X)$ je nerastavljiv, jer u suprotnom $\mu(X)=a(X)\cdot b(X)$, onda $0=\mu(\alpha)=a(\alpha)\cdot b(\alpha)$; kako je $F$ polje, ili $a(\alpha)=0$ ili $b(\alpha)=0$; neka je to $a(\alpha)=0$. Tada $a(X)\in I$, stoga $\mu$ deli $a$, ali $a$ je manjeg stepena, kontradikcija.
> 
> Posmatrajmo sad homomorfizam $\:$ $f:\ F[X]\to F[\alpha]$ $\:$ def. sa $\:$ $f\big(p(X)\big)=p(\alpha)$
> Jasno je da je $f$ "na" i da je $\:$ $\mathrm{Ker}\,f=I$.
> Tada po [[Homomorfizam komutativnih prstena sa jedinicom#^023ba8|teoremi o izomorfizmu]] $\:$ $F[X]/I\cong F[\alpha]$,
> a $F[X]/I$ je polje iz [[Raširenja polja#^a01330|stava]] [[Raširenja polja#^ea3d8d|važi]] da je $F[X]/I$ polje.
> Konačno smo dobili da je $F[\alpha]$ polje. 


$\:$
**Def**. Raširenje $E$ polja $F$ je **algebarsko** ako je svaki element iz $E$ algebarski nad $F$.

**Stav**. Svako konačno raširenje je algebarsko.