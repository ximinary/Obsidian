#fax #math #laag [deo poglavlja [[Matrica|"matrica"]]]
$\:$

$\mathbb{M}_{n}=\mathbb{M}_{n}(\mathbb{F})=\mathbb{M}_{nn}(\mathbb{F})$ — [[Vektorski prostor|VP]] svih kvadratnih matrica $n\times n$.

Jedinična matrica:
$\mathbb{E}_{n}=\left(\begin{array}{c}1&0&\dots&0\\0&1&\dots&0\\\dots&\dots&\dots&\dots\\0&0&\dots&1\end{array}\right)=\begin{cases}e_{ij}=1,&i=j\\e_{ij}=0,&i\ne j\end{cases}$

Stav. $\mathbb{E}_{n}$ je neutral za množenje, tj. $\forall \mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})\quad\mathcal{A\cdot\mathbb{E}_{n}}=\mathbb{E}_{n}\cdot\mathcal{A}=\mathcal{A}$
$\:$ ^f56ca1

**Teorema**. $\mathbb{M}_{n}(\mathbb{F})$ je asocijativna $\mathbb{F}$-[[Algebra nad poljem|algebra]] sa jedinicom.
> Dokaz: [[Matrica#^9c7738|asocijativna]] $\mathbb{F}$-algebra ([[Matrica#^66baee|A2.1]], [[Matrica#^43f815|A2.2]], [[Matrica#^fda602|A3]]) [[Kvadratna matrica#^f56ca1|sa jedinicom]].

$\:$

### [[Determinanta]]
### [[Inverzna matrica]]

### Nilpotentna matrica
**Def**. $\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})$ je **nilpotentna** ako $\exists k>1\ \ :\ \ \mathcal{A}^{k}=\mathcal{O}_{n}$.

Ako $\mathcal{A}^{k-1}\ne\mathcal{O}_{n}\:$ i $\:\mathcal{A}^{k}=\mathcal{O}_{n}$, $\ k$ je **indeks nilpotentnosti** matrice $\mathcal{A}$.

**!** Na glavnoj dijagonali su $0$. $\ \:$ $\mathrm{Tr}\,\mathcal{A}=\det\mathcal{A}=0$
$\:$

Kanonska nilpotentna matrica indeksa $k$:
$\mathcal{N}_{k}=\left(\begin{array}{c}0&1&0&\dots&0\\0&0&1&\dots&0\\\dots&\dots&\dots&\dots&\dots\\0&0&0&\dots&1\\0&0&0&\dots&0\end{array}\right)_{k\times k}$
$\big(\mathcal{N}_{k}\big)^{k}=\mathcal{O}_{k}$

### Opšta linearna grupa
$(\mathbb{M}_{n},\ \cdot)$ je monoid jer operacija množenja je:
- zatvorena: $\forall A,\,B\in\mathbb{M}_{n}(\mathbb{F})\quad A\cdot B\in\mathbb{M}_{n}(\mathbb{F})$
- asocijativna
- postoji neutral za množenje

$(\mathbb{M}_{n},\ \cdot)$ nije grupa jer postoje matrice koje nemaju inverz.

Opšta linearna grupa $\mathrm{GL}(n,\,\mathbb{F})$ ili $\mathrm{GL_{n}}$ sostoji od svih matrica iz $\mathbb{M}_{n}(\mathbb{F})$, koji imaju inverz.


### Podskupovi od $\mathbb{M}_{n}(\mathbb{F})$
##### Simetrična matrica
$\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})$ je simetrična ako $\mathcal{A}=\mathcal{A}^{\mathrm{T}}$

Skup simetričnih matrica: $\mathcal{S}_{n}$
$(\mathcal{S}_{n},\ \mathbb{F},\ +,\ \cdot)$ je [[Vektorski prostor|VP]]. 
$(\mathcal{S}_{n},\ \cdot)$ nije grupa, jer nije zatvorena za množenje.

##### Antisimetrična matrica
$\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})$ je (koso-)antisimetrična ako $\mathcal{A}=-\mathcal{A}^{\mathrm{T}}$

Skup antisimetričnih matrica: $\mathcal{A}_{n}$
$(\mathcal{A}_{n},\ \mathbb{F},\ +,\ \cdot)$ je [[Vektorski prostor|VP]]. 
$(\mathcal{A}_{n},\ \cdot)$ nije grupa, jer $\mathbb{E}_{n}$ nije antisimetrična.

##### Ortogonalna matrica
$\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})$ je ortogonalna ako $\mathcal{A}^{-1}=\mathcal{A}^{\mathrm{T}}$

Skup ortogonalnih matrica: $\mathcal{O}(n,\ \mathbb{F})$
$\mathcal{O}(n,\ \mathbb{F})$ nije [[Vektorski prostor|VP]]. 
$\mathcal{O}(n,\ \mathbb{F})$ je podgrupa $\mathrm{GL}(n,\,\mathbb{F})$, i zove se **ortogonalna grupa**.
##### Dijagonalna matrica
$\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})$ je dijagonalna ako $a_{ij}=0$ za sve $i\ne j$

Oznaka: $\mathcal{A}=\mathrm{diag}\,[a_{11},\,a_{22},\,\dots,\,a_{nn}]$

Skup dijagonalnih matrica $\mathcal{D}_{n}$ je [[Vektorski prostor|VP]]. 
$\mathcal{D}_{n}$ i $\mathbb{F}^{n}$ su izomorfni.

Skup invertibilnih dijagonalnih matrica $\mathcal{D}^{*}_{n}$ je podgrupa $\mathrm{GL}(n,\,\mathbb{F})$.

##### Skalarna matrica
$\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})$ je skalarna ako $\mathcal{A}=\lambda\,\mathbb{E}_{n},\quad\lambda\in \mathbb{F}$.

Skup skalarnih matrica: $\mathrm{Sc}_{n}$
$(\mathrm{Sc}_{n},\ \mathbb{F},\ +,\ \cdot)$ je [[Vektorski prostor|VP]].
$\mathrm{Sc}_{n}$ i $\mathbb{F}$ su izomorfni.

Skup skalarnih ne-nula matrica $\mathrm{Sc}^{*}_{n}\:$ je  podgrupa $\mathrm{GL}(n,\,\mathbb{F})$.

