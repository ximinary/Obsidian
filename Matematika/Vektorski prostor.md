#fax #math #laag [deo [[Linearna algebra|linearne algebre]]]
$\:$

**Def**. $V\ne \varnothing$ tada uređenja četvorka $(V,\,\mathbb{F},\,+,\,\cdot)$ zove se **vektorski prostor** nad poljem $\mathbb{F}$ ako $\forall x,\,y \in V,\ \ \forall \alpha,\,\beta\in\mathbb{F}\ \:$ važi:
- VP1) $\ \ (V,\,+)$ je [[Vektor#^7e6521|Abelova grupa]].
- VP2) $\ \ \alpha\,(\beta\,x)=(\alpha\,\beta)\,x$
- VP3) $\ \ (\alpha+\beta)\,x=\alpha\,x+\beta\,x$
- VP4) $\ \ \alpha\,(x+y)=\alpha\,x+\alpha\,y$
- VP5) $\ \ 1\cdot x=x$

Teorema. Neka je $V$ VP nad poljem $\mathbb{F}$, $x\in V$, $\alpha\in\mathbb{F}$. Tada
1. $\alpha\,(-x)=(-\alpha)\,x=-(\alpha\,x)$
2. $0\,x=\overrightarrow{\rm 0}$
3.  $\alpha\,\overrightarrow{\rm 0}=\overrightarrow{\rm 0}$
4. $\alpha\,x=\overrightarrow{\rm 0}\quad\Rightarrow\quad\alpha=0\ \ \ \mathrm{ili}\ \ \ x=\overrightarrow{\rm 0}$

### Primeri VP
- $(\mathbb{F},\ \mathbb{F},\ +,\ \cdot)$ — polje nad samim sobom.
- Skup [[Vektor|vektora]] u prostoru $\mathbb{E}^{2}\ \text{ ili }\ \mathbb{E}^{3}$
- Skup radijus-vektora u prostoru $\mathbb{E}^{2}\ \text{ ili }\ \mathbb{E}^{3}$
- $(\mathbb{F}^{n},\ \mathbb{F},\ +,\ \cdot)$ — skup uređenih $n$-torki
- $(\mathbb{M}_{mn}(\mathbb{F}),\ \mathbb{F},\ +,\ \cdot)$ — [[Matrica|matrice]]
- $(\mathbb{F}_{n}[x],\ \mathbb{F},\ +,\ \cdot)$ — polinomi
- Skup [[Niz brojeva|nizova]] $\mathbb{F}^{\mathbb{N}}=\{ (x_{1},\,x_{2},\,\dots,\,x_{n},\,\dots)\ \ \big| \ \ x_{i}\in\mathbb{F},\ \forall i=\overline{1,\mathbb{N}}\}$
- [[Red|Redovi]] $\mathbb{F}[[x]]=\left\{  \sum\limits_{i=0}^{\infty} a_{i}\,x^{i}\ \  \bigg|\ \ a_{i}\in\mathbb{F},\ i=\overline{0,\mathbb{N}}\}\right\}$
- Funkcije $\mathbb{F}^{S}=\{f\ \ \big|\ \ f:\ S\to\mathbb{F}\}$. $S\ne \varnothing\:$ i $\:$$\forall f,\, g\in \mathbb{F}^{S},\ \forall\lambda\in \mathbb{F}:$
  (s) $\quad\ (f+g)(x)=f(x)+g(x)$
  (ms) $\ \,f(\lambda\,x)=\lambda\,f(x)$

### [[Linearna zavisnost i nezavisnost. Skup generatora, baza i dimenzija VP-a]]

### [[Potprostor. Operacije nad potprostorima]]


### Izomorfizam
**Def**. $V$ i $W$ su VP nad $\mathbb{F}$. Preslikavanje $A:\ V\to W$ zove se **izomorfizam** VP-a $V$ i $W$ ako 
- $\forall x,\,y\in V\quad A(x+y)=A(x)+A(y)$
- $\forall x\in V,\ \forall \lambda\in \mathbb{F}\quad A(\lambda\,x)=\lambda\,A(x)$
- $A$ je bijekcija
### [[Zavisnost koordinata vektora i matrice operatora o bazi#Zavisnost koordinata vektora o bazi|Zavisnost koordinata vektora o bazi]]
