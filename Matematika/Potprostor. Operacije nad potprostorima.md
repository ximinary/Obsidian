#fax #math #laag [deo poglavlja [[Vektorski prostor|"vektorski prostor"]]]
$\:$

**Def**. $V$ je VP nad $\mathbb{F}\ \:$ i $\ \:L\subseteq V$.
$L$ je **potprostor** od $V$, ako je i sam vektorski prostor nad $\mathbb{F}$ s obzirom na iste operacije sabiranja i množenja skalarom kao u $V$.
Oznaka: $L \leqslant V$

**Teorema** (karakterizacija potprostora). $0\ne L\subseteq V$, $V$ je VP. Tada su ekvivalentni:
- $L$ je potprostor od $V$
- a) $\ \ \forall x,\,y\in L\quad x+y\in L$
  b) $\ \ \forall x\in L\quad \forall \alpha\in\mathbb{F}\quad \alpha\,x\in L$
- $\forall x,\,y\in L\quad\forall\alpha,\,\beta\in\mathbb{F}\quad (\alpha\,x+\beta\,y)\in L$
- $\forall x,\,y\in L\quad\forall\alpha\in\mathbb{F}\quad (\alpha\,x+y)\in L$

**Stav**. $V$ je konačno dim. VP, $L\leqslant V$. Tada $\dim L\leqslant\dim V.$
Specijalno ako $\dim L=\dim V$, onda $L=V.$

### Presek potprostora
**Teorema**. Neka je $\mathcal{F}=\{ L_{i}\leqslant V\ \big|\ i\in I\}$ familija potprostora VP-a $V$.
**Presek potprostora** $\:\ L=\bigcap\limits_{i\,\in\, I}L_{i}\ \:$ je potprostor od $V$.

### Direktan proizvod prostora
**Def**. $V$ i $W$ su VP nad $\mathbb{F}$. $\ \:$ $V\times W$ je **direktan proizvod** prostora ako:
- (s) $\forall v_{1},\,v_{2}\in V,\quad\forall w_{1},\,w_{2}\in W\quad$ važi:
  $\quad\quad (v_{1},\,w_{1})+(v_{2},\,w_{2})=(v_{1}+_{v}\,v_{2},\,w_{1}+_{w}\,w_{2})$
- (ms) $\forall v\in V,\quad\forall w\in W,\quad\forall\lambda\in\mathbb{F}\quad$ važi:
  $\quad\quad \lambda\cdot(v,\,w)=(\lambda \cdot_{v}\,v,\,\lambda\cdot_{w}\,w)$

**Teorema**. $V$ i $W$ su VP nad $\mathbb{F}$. $\:$ Tada je $(V\times W,\,\mathbb{F},\,+,\,\cdot)$ je VP nad $\mathbb{F}$. 

**Def**. Neka je $\mathcal{F}=\{ V_{i}\ |\ V_{i}\ \text{ je VP nad }\mathbb{F},\ i\in I\}$ familija VP-a.
$\prod\limits_{i\,\in\,I}V_{i}\ \:$ je **direktan proizvod** familije $\mathcal{F}$ ako:
- (s) $\forall i\in I\quad\forall v_{i},\,w_{i}\in V_{i}\quad$ važi:
  $\quad\quad (v_{i})_{i\in I}+(w_{i})_{i\in I}=(v_{i}+_{i}\,w_{i})_{i\in I}$
- (ms) $\forall i\in I\quad\forall v_{i}\in V_{i}\quad\forall\lambda\in\mathbb{F}\quad$ važi:
  $\quad\quad \lambda\cdot(v_{i})_{i\in I}=(\lambda\cdot_{i}\,v_{i})_{i\in I}$
  
### Lineal
**Def**. $S\subseteq V$, $V$ je VP nad $\mathbb{F}$.
**Lineal** nad skupom $S$ je najmanji potprostor od $V$ koji sadrži $S$.
Oznaka: $\:\mathcal{L}(S)$.

**Stav**. $S,\,T\subseteq V$, $V$ je VP. Tada
 1. $S\leqslant V\quad\Rightarrow\quad\mathcal{L}(S)=S$
 2. $\mathcal{L}(\mathcal{L}(S))=\mathcal{L}(S)$
 3. $S \subseteq T\quad\Rightarrow\quad \mathcal{L}(S)\subseteq\mathcal{L}(T)$

**Teorema**. $S\subseteq V$, $\:V$ je VP,  Tada
- $\mathcal{L}(S)=\{ \alpha_{1}\,a_{i_{1}}+\alpha_{2}\,a_{i_{2}}+\dots+\alpha_{k}\,a_{i_{k}}\ \big|\ k\in \mathbb{N},\ \alpha_{i}\in \mathbb{F},\ a_{i_{j}}\in S\}$
- $\mathcal{L}(S)=\bigcap\limits_{i\,\in\,I}M_{i}\,,\ \:$ gde je $\:\mathcal{F}=\{ M_{i}\leqslant V\ \big|\ i\in I\}$  familija svih potprostora od $V$ koji sadrže $S$.

**!** VP/potprostor je lineal nad svojom bazom $\mathcal{L}(B).$
### Suma i direktna suma potprostora
**Def**. $L,\,M\leqslant V$, $V$ je konačno dim. VP. Tada je **suma potprostora** $L+M=\mathcal{L}(L\cup M)$.
Suma je **direktna** ako $L\cap M=\{0\}.\ \:$ Oznaka: $L\oplus M$

**Teorema**. $L,\,M\leqslant V$, $V$ je VP. Tada
$L+M=\mathcal{L}(L\cup M)=\{v\ \ \big|\ \ v=l+m,\ \ l\in L,\ \ m\in M\}$

**Stav**. $L,\,M\leqslant V$, $V$ je VP. Tada
$L\oplus M\quad\Leftrightarrow\quad\forall v\in L+M\quad\exists!\big(l\in L,\,m\in M\big)\ \ :\ \ v=l+m.$

**Teorema** (Grasmanova formula). $L,\,M\leqslant V$, $V$ je VP. Tada $\dim(L+M)=\dim L+\dim M-\dim(L\cap M)$.

Posledica. $L\oplus M\quad\Leftrightarrow\quad\dim(L+M)=\dim L+\dim M.$

**Stav**. $\forall L\leqslant V\quad\exists M\leqslant V\ \ :\ \ L\oplus M=V.$