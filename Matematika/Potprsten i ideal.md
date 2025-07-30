#fax #math #alg [deo [[Komutativan prsten sa jedinicom|poglavlja "prsten"]]]
$\:$ 

**Def**. Neka su $(A,\,+,\,\cdot)$ i $(B,\,+',\,\cdot')$ komutativni prsteni sa jedinicom. Tada je $B$ potprsten sa jedinicom prstena $A$ ako važe:
- $B\subseteq A$
- $\forall x,\,y\in B\quad x+y=x+'y$
- $\forall x,\,y\in B\quad x\cdot y=x\cdot'y$
- $1_{A}=1_{B}$

> Napomena: iz tih uslova sledi $0_{A}=0_{B}$

$\:$
**Def**. Neka je $A$ komutativan prsten sa jedinicom i $I$ je neprazan skup. $I$ je ideal u $A$ (oznaka $I\triangleleft A$) ako važe:
- $I\subseteq A$
- $\forall x,\,y\in I\quad x+y\in I$
- $\forall a\in A,\ x\in I\quad a\cdot x\in I$
___

$\:$
**Stav**. Neka je $I$ ideal u $A$. Tada $(I,\,+)\leqslant(A,\,+)$.
> Dokaz: zatvorenost iz drugog uslova;
> asocijativnost se čuva;
> neutral ($0$) iz trećeg uslova: $0\in A\quad0\cdot x=0\in I$;
> inverz elementa $x\in I$ iz trećeg uslova: $(-1)\in A\quad(-1)\cdot x=(-x)\in I$

**Posledica** (prethodnog stava i [[Red grupe i elementa. Indeks podgrupe#^077b13|teoreme]]). Svaki ideal u $\mathbb{Z}$ je oblika $⟨m⟩,\ \ m\in\mathbb{N}_{0}$

$\:$
**Def**. Neka je $A$ komutativan prsten sa jedinicom i $a\in A$. Tada je $⟨a⟩:=\{r\cdot a\ \big|\ r\in A\}$ **glavni ideal** generisan elementom $a$. ^938480

**Stav**. Neka je $n\geqslant 2$ prirodan broj. Tada svaki ideal u $\mathbb{Z}_{n}$ je glavni. ^15271e
> Dokaz: Neka je $\rho_{n}:\ \mathbb{Z}\to\mathbb{Z}_{n}$ def sa $\rho_{n}(x)=x\, \mathrm{mod}\, n$.
> $\rho_{n}$ je [[Homomorfizam komutativnih prstena sa jedinicom|homomorfizam]], koji je "na".
> Neka je $J\triangleleft \mathbb{Z}_{n}$, [[Homomorfizam komutativnih prstena sa jedinicom#^7dc661|tada]] $\rho_{n}^{-1}[J]\triangleleft \mathbb{Z}$
> Na osnovu prethodne posledice $\exists m\in\mathbb{N}_{0}\ \ :\ \ \rho_{n}^{-1}[J]=⟨m⟩$
> Sa jedne strane $\rho_{n}\big[\rho_{n}^{-1}[J]\big]=J$ $\ \:$ (jer je $f$ "na")
> Sa druge strane $\begin{align}\rho_{n}\big[⟨m⟩\big]&=\rho_{n}\big[\{r\cdot m\ \big|\ r\in \mathbb{Z}\}\big]=\{\rho_{n}(r\cdot m)\ \big|\ r\in \mathbb{Z}\}=\{\rho_{n}(r)\cdot \rho_{n}(m)\ \big|\ r\in \mathbb{Z}\}\\&=\{a\cdot \rho_{n}(m)\ \big|\ a\in \mathbb{Z}_{n}\}=⟨\rho_{n}(m)⟩\end{align}$
> Konačno, $J=⟨\rho_{n}(m)⟩$, tj. $J$ je glavni ideal.
___
$\:$
**Def**. Neka su $I$ i $J$ ideali komutativnog prstena sa jedinicom $A$. Tada
$I+J:= \{x+y\ \big|\ x\in I,\,y\in J\}$
$I\,\cdot\, J\,:=\left\{x_{1}y_{1}+\dots+x_{n}y_{n}\quad  \Bigg|\quad n\in\mathbb{N},\quad \begin{array}{l}\forall i=\overline{1,n}\quad x_{i}\in I\\\forall j=\overline{1,n}\quad y_{j}\in J\end{array}\right\}$



**Stav**. Neka su $I$ i $J$ ideali komutativnog prstena sa jedinicom $A$. Tada su $I+J$,  $\:$ $I\cdot J$ $\:$ i $\:$ $I\cap J$ ideali u $A$
> Dokaz: pokažemo $I\cdot J\triangleleft A$, ostala dva se slično trivijalno dokazuju.
> Jer su $+$ i $\cdot$ operacije, $I\cdot J\subseteq A$.
> 
> Za $x_{1}y_{1}+\dots+x_{n}y_{n},\ \ x'_{1}y'_{1}+\dots+x'_{m}y'_{m}\in I\cdot J$
> jasno je da $(x_{1}y_{1}+\dots+x_{n}y_{n})\ +\ (x'_{1}y'_{1}+\dots+x'_{m}y'_{m})=x_{1}y_{1}+\dots+x_{n}y_{n}+x'_{1}y'_{1}+\dots+x'_{m}y'_{m}\in I\cdot J$
> 
> Za $x_{1}y_{1}+\dots+x_{n}y_{n}\in I\cdot J$ $\:$ i $\:$ $a\in A$
> imamo da $a(x_{1}y_{1}+\dots+x_{n}y_{n})=\underbrace{(ax_{1})}_{\in I}y_{1}+\dots+\underbrace{(ax_{n})}_{\in I}y_{n}\in I\cdot J$

___
$\:$
**Stav**. Neka je $K$ polje i $I\triangleleft K$. Tada ili $I=\{0\}$ ili $I=K$. ^680460
> Dokaz: Neka je $K$ polje i $I\triangleleft K\ \ :\ \ I\ne\{0\}$.
> $K$ je polje tj. $\forall x\in K\setminus\{0\}\quad \exists x'\in K\quad x\cdot x'=x'\cdot x=1$
> Kako $I\ne\{0\}$, $\ \:$ $\exists x\in I,\quad x\ne 0$, a za njega $\ \:$ $\exists x'\in K\quad x'\cdot x=1$
> Iz trećeg uslova i $\forall a\in K\quad a\cdot x'\in K$
> dobijamo $\forall a\in K \quad (a\cdot x')\cdot x=a\cdot(x'\cdot x)=a\in I$, $\ \:$ tj. $I=K$

$\:$
### Kongruencija po idealu
**Def**. $I\triangleleft A$. Na $A$ definišemo relaciju kongruencije po idealu $I$ sa $a\equiv_{I} b\quad\Leftrightarrow\quad a-b\in I$

> Napomena: umesto $\:$ $a\equiv_{m\mathbb{Z}}b$ $\:$ pišemo $\:$ $a\equiv_{m} b$ $\:$ u prstenu celih brojeva.

$\:$
**Stav**. Upravo definisana relacija je [[Relacija ekvivalencije|relacija ekvivalencije]].
> Dokaz:
> Refleksivnost. Kako $0\in I\quad\Rightarrow\quad a-a\in I\quad\Rightarrow\quad a\equiv_{I} a$
> Simetričnost. $a\equiv_{I} b\quad\Rightarrow\quad a-b\in I\quad\Rightarrow\quad(-1)(a-b)=b-a\in I\quad\Rightarrow\quad b\equiv_{I }a$
> Tranzitivnost. $a\equiv_{I}b\ \text{ i }\ b\equiv_{I}c\quad\Rightarrow\quad a-b,\,c-b\in I$
> $\Rightarrow\quad(a-b)+(b-c)=a-c\in I\quad\Rightarrow\quad a\equiv_{I}c$   
> Slaganje sa $+$. Neka $a\equiv_{I}a'\ \text{ i }\ b\equiv_{I}b'\quad\Rightarrow\quad a-a',\,b-b'\in I$
> $\Rightarrow\quad(a-a')+(b-b')=(a+b)-(a'+b')\in I\quad\Rightarrow\quad a+b\equiv_{I} a'+b'$
> Slaganje sa $\cdot$. Neka $a\equiv_{I}a'\ \text{ i }\ b\equiv_{I}b'\quad\Rightarrow\quad a-a',\,b-b'\in I$
> $\Rightarrow\quad (a-a')\cdot b'+a\cdot (b-b')=a\cdot b-a'\cdot b'\quad\Rightarrow\quad a\cdot b\equiv_{I} a'\cdot b'$

$\:$
Klasa ekvivalencije elementa $a$ je $a+I=\{a+x\ \big|\ x\in I\}$.

Skup klasa ekvivalencije $A/I=\{a+I\ \big|\ a\in A\}$.
$(A/I,\,+,\,\cdot)$ je komutativni prsten sa jedinicom, koji zovemo **količnički prsten** prstena $A$ po idealu $I$. Operacije:
- $(a+I)+(b+I)=(a+b)+I$
- $(a+I)\cdot(b+I)=(a\cdot b)+I$

