#fax #math #laag [deo [[Linearna algebra|linearne algebre]]]
$\:$

**Def**. $V\ne \varnothing$ tada uređenja četvorka $(V,\,\mathbb{F},\,+,\,\cdot)$ zove se **vektorski prostor** nad poljem $\mathbb{F}$ ako $\forall x,\,y \in V,\ \ \forall \alpha,\,\beta\in\mathbb{F}\ \:$ važi:
- VP1) $\ \ (V,\,+)$ je Abelova grupa.
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


### [[Linearna zavisnost i nezavisnost. Skup generatora, baza i dimenzija VP-a]]

### [[Potprostor. Operacije nad potprostorima]]


### Izomorfizam
**Def**. $V$ i $W$ su VP nad $\mathbb{F}$. Preslikavanje $A:\ V\to W$ zove se **izomorfizam** VP-a $V$ i $W$ ako 
- $\forall x,\,y\in V\quad A(x+y)=A(x)+A(y)$
- $\forall x\in V,\ \forall \lambda\in \mathbb{F}\quad A(\lambda\,x)=\lambda\,A(x)$
- $A$ je bijekcija
### Zavisnost koordinata vektora o bazi

**Def**. $V$ je VP dimenzije $n$ nad poljem $\mathbb{F}$, $\:$ $e=\{ e_{1},\,e_{2},\,\dots,\,e_{n} \}$ je neka baza VP-a $V$. Tada za bazu $e$, koordinatizacija je preslikavanje $\kappa_{e}:\ V\to \mathbb{F}^{n}$, koje je definisano formulom $\kappa_{e}(x)=\kappa_{e}\left( \sum\limits_{i=1}^{n}x_{i}\,e_{i} \right)=(x_{1},\,x_{2},\,\dots,\,x_{n})=x(e)$.

$\kappa_{e}$ je izomorfizam VP-a $V$ i $\mathbb{F}^{n}$ jer važe:
- $\forall x,\,y\in V\quad \kappa_{e}(x+y)=\kappa_{e}(x)+\kappa_{e}(y)$
- $\forall x\in V,\ \forall \lambda\in \mathbb{F}\quad \kappa_{e}(\lambda\,x)=\lambda\,\kappa_{e}(x)$
- $\kappa_{e}$ je bijekcija

###### Prelazak sa jedne baze na drugu:
Neka su $e= \{e_{1},\,e_{2},\,\dots,\,e_{n}\}$ i $e'= \{e'_{1},\,e'_{2},\,\dots,\,e'_{n}\}$ baze VP-a $V$.

$e'_{k}=\sum\limits_{i=1}^{n}\alpha_{ik}\,e_{i}\quad\forall k=\overline{1,n}$

$\left(\begin{array}{c}e'_{1}&e'_{2}&\dots&e'_{n}  \end{array}\right)=\left(\begin{array}{c}e_{1}&e_{2}&\dots&e_{n}  \end{array}\right)\left(\begin{array}{c}\alpha_{11}&\alpha_{12}&\dots&\alpha_{1n}\\ \alpha_{21}&\alpha_{22}&\dots&\alpha_{2n}\\ \dots&\dots&\dots&\dots\\\alpha_{n1}&\alpha_{n2}&\dots&\alpha_{nn}  \end{array}\right)$

$T_{ee'}:=(\alpha_{ij})$ — matrica prelaska sa $e$ u $e'$