#fax #math #laag [deo poglavlja [[Linearni operator|"linearni operator"]] i [[Unitarni prostor|"unitarni prostor"]]]

### [[Linearni funkcional]] u unitarnom prostoru
$V$ je unitarni prostor.
Preslikavanje $f_{x}:V\to\mathbb{C}$ def. sa $f_{x}(y)=\langle y,\ x\rangle$ je linearni funkcional.

**Teorema**. $V$ je konačnodimenzioni unitarni prostor, $f: V\to\mathbb{C}$. Tada $\exists!v_{0}\in V\ \ :\ \ \forall v\in V \quad f(v)= \langle v,\ v_{0}\rangle$

**Def**. Reprezentacija linearnog funkcionala pomoću skalarnog proizvoda: $\delta: V^{*}\to V$ def. sa $\delta(f)=v_{0}\quad\big(\forall v\in V \quad f(v)= \langle v,\ v_{0}\rangle\big)$

Stav. Važi:
- $\forall f,\,g\in V^{*}\quad\delta(f+ g)=\delta(f)+\delta(g)$
- $\forall f\in V^{*}\quad \forall\lambda\in\mathbb{C}\quad\delta(\lambda\,f)=\overline{\lambda}\,\delta(f)$
- $\delta$ je bijekcija
### Hermitski adjungovani operator
**Def**.
$A\in \mathrm{Hom}\,V$, $\:$ $w\in V$, $\:$ $f: V\to\mathbb{C}$ def. sa $f(v)= \langle A(v),\ w\rangle$.
Iz prethodne teoreme $\exists!w_{0}\in V\ \ :\ \ \forall v\in V\quad f(v)= \langle v,\ w_{0}\rangle$

Operator  $A^{*}:\ V\to V$ dat sa $A^{*}(w)=w_{0}$ je **hermitski adjungovani** operatoru $A$.

tj. $A^{*}$ je takav da važi: $\:$ $\boxed{\forall v,\,w\in V\quad\Big\langle A(v),\ w\Big\rangle= \Big\langle v,\ A^{*}(w)\Big\rangle}$

Stav. $V$ je unitarni konačnodimenzioni prostor. Tada $A\in\mathrm{Hom}\,V\quad\Rightarrow\quad A^*\!\in\mathrm{Hom}\,V$

Stav. $V$ je konačnodimenzioni unitarni prostor, $e$ je [[Unitarni prostor#Ortonormirana baza|ortonormirana baza]] od $V$, $A\in \mathrm{Hom}\,V$. Tada ako je $\mathcal{A}$ matrica operatora $A$ u bazi $e$ onda je $\mathcal{A}^{*}$ \[[[Matrica#Hermitsko konjugovanje|?]]\] matrica operatora $A^{*}$.

**Teorema**. $V$ je konačnodimenzioni unitarni prostor, $A\in \mathrm{Hom}\,V$. Tada $V=\mathrm{Ker}\,A\oplus\mathrm{Im}\,A^{*}=\mathrm{Ker}\,A^{*}\oplus\mathrm{Im}\,A$
### Klase operatora u unitarnom prostoru
**Def**. $V$ je unitarni prostor, $A\in \mathrm{Hom}\,V$. Tada je $A$
- **normalan** ako $A\,A^{*}=A^{*}A$
	- **hermitski** ako $A^{*}=A$
	- (koso-)**antihermitski** ako $A^{*}=-A$
	- **unitaran** ako $A\,A^{*}=A^{*}A=\mathrm{id}_{V}$ $\ \:$ (tj. $A^{*}=A^{-1}$)

**Teorema**. [[Karakteristični i minimalni polinom#Sopstvene vrednosti|Sopstvene vrednosti]]:
- hermitskog operatora su realni;
- antihermitskog operatora su čisto imaginarni;
- unarnog operatora imaju apsolutnu vrednost $1$.

**Teorema**. $V$ je unitaran prostor, $A\in \mathrm{Hom}\,V$. Tada
- $A$ je hermitski/antihermitski/unitarni, $L$ je [[Redukcija linearnog operatora|invarijantni prostor]] od $A$. Tada je $L^{\perp}$ invarijantni prostor od $A$.
- $A$ je unitaran. Tada $A$ i $A^{*}$ čuvaju skalarni proizvod.
- $A$ je unitaran $\quad\Leftrightarrow\quad$ $A$ preslikava opronormiranu bazu u ortonormiranu bazu.
___
**Teorema**. $V$ je unitaran prostor, $A\in \mathrm{Hom}\,V$ je normalan. Tada
- $\lambda$ je sopstvena vrednost $A$ $\quad\Rightarrow\quad$ $\overline{\lambda}$ je sopstvena vrednost $A^{*}$ uz isti sopstveni vektor
- Sopstveni vektori koji odgovaraju različitim sopstvenim vrednostima su ortogonalni.

**Lema**. $V$ je unitaran prostor, $A\in \mathrm{Hom}\,V$.
$\forall v\in V\quad||A^{*}(v)||\leqslant||A(v)||\quad\Rightarrow\quad A$ je normalan

**Teorema**. $V$ je unitaran prostor, $A\in \mathrm{Hom}\,V$ je normalan. Tada postoji ortonormirana baza $V$ u kojoj je matrica operatora $A$ dijagonalna.

### Pozitivnost hermitskog operatora
**Def**. Hermitski operator $A\in\mathrm{Hom}\,V$ je **pozitivan** $(A\geqslant0)$ ako $\forall v\in V\quad \big\langle A(v),\ v\big\rangle\geqslant0$.
$A$ je strogo pozitivan ako još važi $\big\langle A(V),\ v\big\rangle =0\quad\Leftrightarrow\quad v=\mathbf{0}$

**Teorema**. $A\in\mathrm{Hom}\, V$ je hermitski operator. Tada $A$ je pozitivan $\quad\Leftrightarrow\quad$ $\forall \lambda\in \mathrm{Sp}(A)\quad \lambda\geqslant0$.

**Def**. Operator $B\in \mathrm{Hom}\,V$ je **kvadratni** (drugi) **koren** iz operatora $A\in\mathrm{Hom}\,V$ ako $B^{2}=A$.

**Teorema**. $A\in\mathrm{Hom}\,V$ je pozitivan hermitski operator, tada postoji jedinstven pozitivan kvadratni koren iz $A$ — operator $B\in\mathrm{Hom}\,V$, koji komutira sa svim operatorima sa kojima komutira $A$.