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
$(\mathbb{M}_{n},\ \cdot)$
