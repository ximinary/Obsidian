#fax #math #alg  [deo [[Grupa|poglavlja "grupa"]]]
$\:$
**Def**. Ako je $G$ konačna grupa, onda broj njenih elemenata zovemo **red grupe** i označavamo sa $|G|$. Ako je grupa beskonačna, kažemo da je ona **beskonačnog reda**.

**Def**. Neka je $a$ element neke grupe. Ako postoji $n\geqslant1$ za koji važi $a^{n}=e$, onda je **red elementa** $a$ jednak $\omega(a)=\min\{m\geqslant1\ |\ a^{m}=e\}$, inače je $a$ **beskonačnog reda**.

**Stav**. Red bilo kojeg elementa grupe je jednak redu podgrupe generisane tim elementom.
> Dokaz: Neka je podgrupa $\langle a\rangle$ generisana elementom $a$.
> 
> Ako je $a$ beskonačnog reda, važi $\forall n\geqslant 1\quad a^{n}\ne e$
> Da li neke za neke $l> m$ može važiti $a^{l}=a^{m}$?
> Pomnožimo jednačinu sa $a^{-m}$, imamo $a^{l-m}=e$, pri tome $l - m \geqslant 1$. Kontradikcija, važi da su sve $a^{n}$ različite za različite $n$, stoga $\langle a\rangle$ ima beskonačno mnogo elemenata.
> 
> Ako je $a$ reda $n\geqslant 1$, tj. $\ \:$ $a^{n}=e$ $\ \:$ i $\ \:$ $\forall m=\overline{1,\,n\!-\!1}\quad a^{m}\ne e$
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
> iz [[Red grupe i elementa. Indeks podgrupe#^1698b9|stava]] $\langle a^{n/k} \rangle$ je reda $\begin{align}\frac{n}{\mathrm{NZD}(n,\,n/k)}=\frac{n}{n/k}=k\end{align}$
> $H:=\langle a^{n/k} \rangle$, pretpostavimo da postoji i druga podgrupa $\widetilde{H}$ reda $k$ odlična od $H$.
> iz 1. $\widetilde{H}$ je ciklična, tj. $\widetilde{H}=\langle a^{l} \rangle$.
> $a^{lk}=\big(a^{l}\big)^{k}=e$ (jer je $\widetilde{H}$ reda $k$)
> a $G$ je reda $n$ ($a^{n}=e$), imamo da $n\,|\,lk$
> iz $k\,|\,n$ dobijamo da $\begin{align}\frac{n}{k}\,\bigg|\,l\end{align}$, $\ \:$ tj $\begin{align}l=p\cdot\frac{n}{k}\end{align}$, za neko $p\in\mathbb{Z}$.
> $a^{l}=\big(a^{n/k}\big)^{p}\in H$, odakle $\widetilde{H}\subseteq H$ i kako $|H|=|\widetilde{H}|$ važi da $H=\widetilde{H}$.
> Kontradikcija.
> $H=\langle a^{n/k} \rangle$ je jedinstvena podgrupa reda $k$.

$\:$
**Teorema**. Neka je $G$ grupa i $a,\,b\in G$ su konačnog reda. Tada ako 
$ab=ba$ $\ \:$ i $\ \:$ $\langle a \rangle\cap\langle b \rangle=\{e\}$, $\ \:$ onda $\omega(a\,b)=\mathrm{NZS}\Big(\omega(a),\ \omega(b)\Big)$ ^5f96ab
> Dokaz:
> Neka $\omega(a)=m$, $\omega(b)=n$, $\omega(a\,b)=s$, $\mathrm{NZS}(m,n)=t=m\,t_{1}=n\,t_{2}$
> $(a\,b)^{t}=a^{t}b^{t}=a^{mt_{1}}b^{nt_{2}}=e^{t_{1}}e^{t_{2}}=e\quad\Rightarrow\quad s\,|\,t$
> $e=(a\,b)^{s}=a^{s}b^{s}\quad\Rightarrow\quad a^{s}=b^{-s}$, $\:$ $a^{s}\in \langle a \rangle$, $\:$ $b^{-s}\in\langle b \rangle$
> Jer $\langle a \rangle\cap\langle b \rangle=\{e\}$ dobijamo $a^{s}=e=b^{s}$ 
> $\Rightarrow\quad m\,|\,s\ \text{ i } \ n\,|\,s\quad\Rightarrow\quad t\,|\,s$
> Konačno, $t=s$

$\:$
**Teorema**. Neka je $G$ grupa i $a,\,b\in G$ takvi da $a\,b=b\,a$
- Ako je $a$ konačnog reda a $b$ beskonačnog, onda je $a\,b=b\,a$ beskonačnog reda.
- Ako su  i $a$ i $b$ beskonačnog reda i $\langle a \rangle\cap\langle b \rangle=\{e\}$, onda je $a\,b=b\,a$ beskonačnog reda.

> Dokaz:
> - Neka $\omega(a)=n$. PPS $ab$ je konačnog reda $m$.
>   $e=e^{n}=(ab)^{mn}=a^{mn}b^{mn}=e^{m}b^{mn}=b^{mn}$, $b$ je konačnog reda. Kontradikcija. $ab$ je beskonačnog reda.
>  - PPS $ab$ je konačnog reda $m$.
>    $e=(ab)^{m}=a^{m}b^{m}\quad\Rightarrow\quad a^{m}=e=b^{m}$
>    $a$ i $b$ su konačnog reda. Kontradikcija. $ab$ je beskonačnog reda.


$\:$
### Veza između reda grupe i reda njenih podgrupa/elemenata

**Def**. Ako je $H\leqslant G$ $\ \:$ i $\ \:$ $x\in G$
- Skup $xH=\{x\cdot h\ \big|\ h\in H\}$ se zove levi koset podgrupe $H$ u grupi $G$
- Skup $Hx=\{h\cdot x\ \big|\ h\in H\}$ se zove desni koset podgrupe $H$ u grupi $G$

Skup svih levih koseta grupe $H$ u $G$ se označava sa $G/H$
Skup svih desnih koseta grupe $H$ u $G$ se označava sa $H\!\setminus\!G$

> Napomena: u opštem slučaju važi $xH\ne Hx$ kao i $G/H\ne H\!\setminus\!G$;
> u opštem slučaju $\exists$ bijekcija $xH\mapsto Hx^{-1}$, stoga $\big|G/H\big|=\big|H\!\setminus\!G\big|$.

$\:$
**Stav**.
1. $xH=yH\quad\Leftrightarrow\quad x^{-1}y\in H$ ^a82139
2. $xH\ne yH\quad\Rightarrow\quad xH\cap yH=\varnothing$

> Dokaz:
> 1. $\boxed{\Rightarrow}$ Neka $xH=yH$. Tada, jer je $e\in H$, važi $y\in xH$, tj. $\exists h\in H\ \ :\ \ xh=y$, odakle $h=x^{-1}y$
> $\:$
> $\boxed{\Leftarrow}$ Neka je $x^{-1}y\in H$. 
> Pretpostavimo da je $z\in xH$, odakle $\exists h\ \ :\ \ z=xh=x(x^{-1}y)(x^{-1}y)^{-1}h=y\underbrace{\big((x^{-1}y)h\big)}_{\in H}\in yH$
> tj. $xH\subseteq yH$. Analogno se dokazuje i $xH\supseteq yH$, odakle $xH=yH$.
> $\:$
> 2. pps: važi $xH\ne yH\quad$ i $\quad xH\cap yH\ne\varnothing$, tj. $\exists z\in xH\cap yH$
>    $\exists h,\,h'\ \ :\ \ z=xh=yh'$ 
> odakle $x^{-1} y=\underbrace{h(h')^{-1}}_{\in H}\quad\overset{1.}{\Rightarrow}\quad xH=yH$. Kontradikcija.

$\:$
**Def**. $G$ je grupa, $H\leqslant G$.
- Ako je skup $G/H$ beskonačan, onda je podgrupa $H$ **beskonačnog indeksa** u $G$.
- Ako je skup $G/H$ konačan, onda je **indeks** podgrupe $H$ u $G$ jednak veličine tog skupa. Oznaka $[G:H]\,:=\,\big|G/H\big|$


**Stav**. $G$ je grupa, $H\leqslant G$. Tada je $G$ disjunktna unija različitih levih koseta podgrupe $H$.

**Teorema** (Lagranžova). $G$ je konačna grupa, $H\leqslant G$. Tada 
$\big|G\big|=\big|H\big|\cdot[G:H]$ $\quad$ (odakle red podgrupe $H$ deli red grupe $G$) ^cd291f

> Dokaz:
> Iz prethodnog stava $\begin{align}G=\bigsqcup_{i =1}^{k}x_{i}H\end{align}$, gde su $x_{i}\in G$ svi različiti, a $k =[G:H]$.
> i jer $\big|xH\big|=\big|H\big|$ za bilo koje $x\in G$, 
> važi da $\big|G\big|=\big|H\big|\cdot[G:H]$

$\:$
**Posledica**. Red svakog elementa konačne grupe deli red te grupe.

**Posledica**. Svaka grupa prostog reda $p$ je ciklična (tj. izomorfna $\mathbb{Z}_{p}$).

**Posledica**. Ako je $G$ konačna grupa, onda $\forall x\in G\quad x^{|G|}=e$
^026da4
> [[Kongruentnost#Ojlerova teorema|Ojlerova teorema]]

$\:$
**Teorema** (Košijeva). $G$ je konačna grupa, $p$ je prost broj, koji deli $\big|G\big|$. Tada $\exists x\in G\quad \omega(x)=p\quad\quad\Big(\exists H\leqslant G\quad\big|H\big|=p\Big)$ ^ebbac3
> Dokaz: Neka je $H=\langle a \rangle$ neka ciklična grupa reda $p$.
> I neka je $X=\{(x_{1},\,x_{2},\,\dots,\,x_{p})\in G^{p}\ |\ x_{1}x_{2}\cdots x_{p}=e\}$. Tada
> $|X|=|G|^{p-1}$, jer $x_{1},\,x_{2},\,\dots,\,x_{p-1}$ mogu biti bilo koji, a $x_{p}=(x_{1}x_{2}\cdots x_{p-1})^{-1}$.
> Stoga $p\ \big|\,|X|$.
> 
> Zadajemo [[Dejstvo grupe|dejstvo]] $H$ na $X$ sa $a\cdot(x_{1},\,x_{2},\,x_{3},\,\dots,\,x_{p})=(x_{2},\,x_{3},\,\dots,\,x_{p},\,x_{1})$
> (iz definicije pojma dejstva je jasno da je za cikličnu grupu dovoljno zadati dejstvo generatora);
> Da li je $(x_{2},\,x_{3},\,\dots,\,x_{p},\,x_{1})\in X$?
> $(x_{1},\,x_{2},\,x_{3},\,\dots,\,x_{p})\in X\quad\Rightarrow\quad x_{p}=(x_{1}x_{2}\cdots x_{p-1})^{-1}\quad\Rightarrow$
> $x_{2}x_{3}\cdots x_{p-1}x_{p}x_{1}=x_{2}x_{3}\cdots x_{p-1} (x_{1}x_{2}\cdots x_{p-1})^{-1}x_{1}=x_{2}x_{3}\cdots x_{p-1} (x_{p-1}^{-1}\cdots x_{3}^{-1}x_{2}^{-1}x_{1}^{-1} )x_{1}=e$
> Stoga je dejstvo dobro definisano.
> 
> Iz [[Dejstvo grupe#^72d803|posledice]] znamo $\forall x\in H\quad |\Omega(x)|\ \big|\ |G|\!=\!p\quad\Rightarrow\quad\left[\begin{array}{}|\Omega(x)|=1\\|\Omega(x)|=p\end{array}\right.$
> 
> Zapravo orbita nekog elementa $(x_{1},\,x_{2},\,\dots,\,x_{p})\in X$ je sve ciklične permutacije $p$-torke: $\Omega\big((x_{1},\,x_{2},\,\dots,\,x_{p})\big)=\{(x_{1},\,x_{2},\,\dots,\,x_{p}),\ (x_{2},\,x_{3},\,\dots,\,x_{p},\,x_{1}),\ \dots,\ (x_{p},\,x_{1},\,x_{2},\,\dots,\,x_{p-1})\}$
> $\Omega\big((e,\,e,\,\dots,\,e)\big)=\{(e,\,e,\,\dots,\,e)\}$
> 
> Imamo da je $X$ disjunktna unija <u>različitih</u> orbita.
> $X=\Omega_{1}\sqcup\Omega_{2}\sqcup\dots\sqcup\Omega_{k}$
> Ako je $\Omega_{1}=\{(e,\,e,\,\dots,\,e)\}$ jedina jednočlana orbita imamo:
> $p\ |\ \big(1+p(k-1)\big)$ $\quad$ (više je dokazano $p\ \big|\,|X|$),
> što nije tačno; dakle, postoji jednočlana orbita različita od $\Omega_{1}$;
> neka je ta orbita $\{(x_{1},\,x_{2},\,\dots,\,x_{p})\}$, tada
> $a\cdot(x_{1},\,x_{2},\,\dots,\,x_{p})=(x_{1},\,x_{2},\,\dots,\,x_{p})$, 
> odakle $x_{1}=x_{2}=\dots=x_{p}$ označimo sa $g:=x_{1}$;
> $g\ne e,\quad g\cdot g\cdots g=g^{p}=e$ (jer je $g\in X$)
> $g$ je traženi element reda $p$.

^d9c566

$\:$
**Stav**.
- Svaka grupa reda 4 izomorfna je ili grupi $\mathbb{Z}_{4}$ ili grupi $\mathbb{Z}_{2}\times \mathbb{Z}_{2}$
-  Svaka grupa reda 6 izomorfna je ili grupi $\mathbb{Z}_{6}$ ili grupi $\mathbb{D}_{3}$
-  Svaka grupa reda 8 izomorfna je jednoj od grupa: 
  $\mathbb{Z}_{8}$, $\ \:$ $\mathbb{Z}_{2}\times\mathbb{Z}_{4}$, $\ \:$ $\mathbb{Z}_{2}\times\mathbb{Z}_{2}\times\mathbb{Z}_{2}$, $\ \:$ $\mathbb{D}_{4}$,  $\ \:$ $Q_{8}$
-  Svaka grupa reda 9 izomorfna je ili grupi $\mathbb{Z}_{9}$ ili grupi $\mathbb{Z}_{3}\times\mathbb{Z}_{3}$
-  Svaka grupa reda 10 izomorfna je ili grupi $\mathbb{Z}_{10}$ ili grupi $\mathbb{D}_{5}$
