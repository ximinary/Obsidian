#fax #math #alg [deo [[Komutativan prsten sa jedinicom|poglavlja "prsten"]]]
$\:$ 


**Def**. Neka je $A$ komutativan prsten sa jedinicom. **Skup svih invertibilnih elemenata** u $A$ u odnosu na $\cdot$ je $U(A)=\{x\in A\ \big|\ \exists y\in A\quad a\cdot b = 1\}$ 
$\big(U(A),\,\cdot\big)$ je **grupa invertibilnih elemenata** prstena $A$. ^d07f3d

> Napomena: $0$ nema inverz: $x\cdot0=0\ne1$, ako $A\ne\{0\}$

**Stav**. $\big(U(A),\,\cdot\big)$ je Abelova grupa.
> Dokaz: 
> zatvorenost: $x,\,y\in U(A)\quad \exists x',\,y'\in U(A)\quad x\cdot x'=y\cdot y'=1$
> $(x\cdot y)\cdot(y'\cdot x')=x\cdot(y\cdot y')\cdot x'=x\cdot 1\cdot x'=x\cdot x'=1\quad\Rightarrow\quad x\cdot y\in U(A)$;
> asocijativnost se čuva;
> neutral: $1\in U(A)$, jer $1\cdot1=1$;
> inverz: iz definicije skupa

$\:$
**Def**. **Polje** je komutativan prsten sa jedinicom $A$ u kojem $U(A)=A\setminus\{0\}$ ^b98e89

**Stav**. $(\mathbb{Z}_{n},\,+_{n},\,\cdot_{n})$ je polje akko $n$ je prost broj. ^9c82dc
> Dokaz: $U(\mathbb{Z}_{n})=\Phi(n)$
> Jer $x\in \mathbb{Z}_{n}$ ima inverz po $\cdot$ akko $x$ delji $n$.

$\:$
**Def**. Element $x\ne0$ prstena $A$ je **pravi delitelj nule** u prstenu $A$ ako $\exists y\in A\setminus\{0\}\quad x\cdot y=0$

**Stav**. U polju nema pravih delitelja nule.
> Dokaz: 
> U polju $A$: $\ \:$ $\forall x\ne 0\quad\exists x'\ne 0\quad x\cdot x'=x'\cdot x=1\quad\quad(1)$
> 
> PPS, u polju $A$ postoji pravi delitelj nule:
> $\exists x,\,y\ne0\quad x\cdot y =0$ 
> iz $(1)$ $\ \:$ $\exists x'\quad x'\cdot x=1$
> $0=x'\cdot0=x'\cdot(x\cdot y)=(x'\cdot x)\cdot y=1\cdot y=y$
> Kontradikcija

$\:$
**Def**. Komutativan prsten sa jedinicom u kojem nema pravih delilaca nule je **domen** (oblast celih)

![[prsten-domen-polje.png]]

**Stav**. Svaki konačan domen je polje
> Dokaz:
> Neka je $A$ konačan domen (konačan prsten koji ne sadrži pravih delitelja nule).
> PPS, $\exists x\in A\setminus\{0\}$ koji nema inverz, tj. $\forall y\in A\quad x\cdot y\ne 1$
> $A$ je domen $\quad\Rightarrow\quad$ $\forall y\in A\setminus\{0\}\quad x\cdot y\ne 0$
> Odakle, za $\forall y\in A\setminus \{0\}\quad y\cdot x\in A\setminus\{0,\,1\}$
> po [[Prebrojavanja#^3dcb3c|Dirihleovom principu]] $\exists y'\ne y''\quad y'\cdot x=y''\cdot x$
> $(y''-y')\cdot x=0\quad\Rightarrow\quad$ $x$ je delitelj nule. Kontradikcija.

$\:$
**Def**. $x\in A\setminus\{0\}$ je **regularan** ako $x\cdot y=0\quad\Rightarrow\quad y=0$

> Svaki invertibilni element $a$ je regularan:
> $\exists a'\in A\setminus\{0\}\quad a'\cdot a=1$
> Množenjem relacije $a\cdot x=a\cdot y$
> sa $a'$ sleva dobijamo $x=y$

> Prsten je disjunktna unija skupova
> - svojih pravih delitelja nule
> - svojih regularnih elemenata
> - $\{0\}$

$\:$
**Stav**. U konačnom prstenu svaki regularan element je invertibilan.
> Dokaz: analogni dokazu prethodnog stava.

$\:$
![[regularan-i-pravi-delitelj.png]]

