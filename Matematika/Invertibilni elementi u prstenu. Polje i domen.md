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
**Def**. Element $x\ne0$ prstena $A$ je **pravi delitelj nule** u prstenu $A$ ako $\exists y\in A\setminus\{0\}\quad x\cdot y=0$

**Def**. $x\in A\setminus\{0\}$ je **regularan** ako $\forall y\in A\quad x\cdot y=0\quad\Rightarrow\quad y=0$
> Napomena: 
> $\forall y\in A\quad x\cdot y=0\quad\Rightarrow\quad y=0$
> $\forall y\in A\quad y\ne0\quad\Rightarrow\quad x\cdot y\ne0$
> $\forall y\in A\setminus\{0\}\quad x\cdot y\ne 0$
> 
> Tj. svaki ne-nula element ili je regularan ili je pravi delitelj nule.  

$\:$
**Stav**.  Svaki invertibilni element $x$ je regularan:
> Dokaz: neka je $x$ invertibilan, tj. > $\exists x'\in A\setminus\{0\}\quad x'\cdot x=1$
> Množenjem relacije $\:$ $x\cdot y=0$ $\:$ sa $\:$ $x'$ $\:$  dobijamo $\:$ $x'\cdot x\cdot y=x'\cdot0$, $\:$ odakle $\:$ $y=0$

$\:$
![[regularan-i-pravi-delitelj.png]]
$\:$

**Def**. Komutativan prsten sa jedinicom u kojem nema pravih delilaca nule je **domen** (oblast celih).

**Def**. **Polje** je komutativan prsten sa jedinicom $A$ u kojem $U(A)=A\setminus\{0\}$ ^b98e89

**Stav**. $(\mathbb{Z}_{n},\,+_{n},\,\cdot_{n})$ je polje akko $n$ je prost broj. ^9c82dc
> Dokaz: $U(\mathbb{Z}_{n})=\Phi(n)$
> Jer $x\in \mathbb{Z}_{n}$ ima inverz po $\cdot$ akko $x$ delji $n$.


$\:$
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
> [[prsten-domen-polje.png|Napomena]].

$\:$
**Stav**. U <u>konačnom</u> prstenu svaki regularan element je invertibilan.
> Dokaz: Neka je $A$ konačan komutativan prsten sa jedinicom i neka je $R\subseteq A$ skup svih regularnih elemenata prstena $A$, tada 
> Neka su $\:$ $x,\,y\in R$, tada $\:$ $\forall z\in A\setminus\{0\}\quad x\cdot z\ne0\ \text{ i }\ y\cdot z\ne 0$
> stoga $\:$ $(x\cdot y)\cdot z\ne 0$, $\:$ tj. $\:$ $x\cdot y\in R$
> 
> Iz definicije je očigledno da $\:$ $1\in R$.
> 
> PPS, $\exists x\in R$ koji nema inverz, tj. $\:$ $\forall y\in A\quad x\cdot y\ne 1$
> Odakle, za $\:$ $\forall y\in R\quad x\cdot y\in R\setminus\{1\}$.
> Po [[Prebrojavanja#^3dcb3c|Dirihleovom principu]], jer $\:$ $|R\setminus\{1\}|<|R|$, $\:$ važi $\:$ $\exists y'\ne y''\quad x\cdot y'=x\cdot y''$
> $x\cdot(y''-y')=0\quad\Rightarrow\quad$ $x$ je delitelj nule. Kontradikcija.

$\:$
**Posledica**. Svaki <u>konačan</u> domen je polje



