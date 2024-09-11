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

Skup simetričnih matrica: $S_{n}$
$(S_{n},\ \mathbb{F},\ +,\ \cdot)$ je [[Vektorski prostor|VP]]. $\:$ $(S_{n},\ \cdot)$ nije grupa

##### Antisimetrična matrica

##### Ortogonalna matrica

##### Dijagonalna matrica

##### Skalarna matrica