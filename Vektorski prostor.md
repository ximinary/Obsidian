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

### Baza i dimenzija VP-a
**Def**. $0\ne B\subseteq V$. $\ \:$ $x\in V$ je **linearna kombinacija** vektora $a_{1},\,a_{2},\,\dots,\,a_{n}\in B \ \:$ ako
$\exists\alpha_{1},\,\alpha_{2},\,\dots,\,\alpha_{n}\in\mathbb{F}\ \ : \ \ x=\alpha_{1}\,a_{1}+\alpha_{2}\,a_{2}+\dots+\alpha_{n}\,a_{n}$
---
**Def**. Ako $\forall x\in V\ \:$ $x$ je linearna kombinacija vektora $a_{1},\,a_{2},\,\dots,\,a_{n}\in B$.
Tada je $B$ **skup generatora** VP-a $V$.

Ako je $B$ skup generatora $V$, tada važi
1. $y\in V,\ \ y\ne0\quad\Rightarrow\quad B'=B\cup\{y\}$ je skup generatora $V$
2. $z\in V$ je linearna kombinacija vektora iz $B''=B\setminus\{z\}$
   $\Rightarrow\quad B''$ je skup generatora $V$
---
**Def**. Neka je $B=\{{a_{1},\,a_{2},\,\dots,\,a_{n}\}}\subseteq V$. $B$ je **linearno nezavisan** ako jednačina  $\alpha_{1}\,a_{1}+\alpha_{2}\,a_{2}+\dots+\alpha_{n}\,a_{n}= 0,\quad \alpha_{i}\in\mathbb{F}\ \ \forall i=\overline{1,n}$
ima jedinstveno rešenje $\alpha_{1}=\alpha_{2}=\dots=\alpha_{n}=0$

$B$ je **linearno zavisan** inače.

Svojstva:
1. $B\subseteq V$. $B\cup\{0\}$ je uvek linearno zavisan.
2. $B=\{a_{1}\},\quad a_{1}\ne0\quad\Rightarrow\quad B$ je linearno nezavisan.
3. $B=\{a_{1},\,a_{2}\}$ je linearno zavisan $\:\ \Leftrightarrow\ \ \exists\lambda\in\mathbb{F}\ \ :\ \ a_{1}=\lambda\,a_{2}$
4. Podskup linearno nezavisnog skupa je linearno nezavisan.
5. Nadskup linearno zavisnog slupa je linearno zavisan.

Stav. $B=\{ a_{1},\,a_{2},\,\dots,\,a_{n} \}\not\ni0$ je podskup $V$. Tada
$B$ je linearno zavisan $\,\ \Leftrightarrow\ \ \exists i>1\ \ :\ \ a_{i}$ je lin. kombinacija 
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\ \  a_{1},\,a_{2},\,\dots,\,a_{i-1}$
---
**Def**. **Baza** VP-a $V$ je $\ \ B\subseteq V\ \:$ linearno nezavisan skup generatora $V$.

**Teorema** (o bazi). $V$ je VP nad $\mathbb{F}$. Tada
1. $\exists B\subseteq V$ baza VP-a $V$.
2. Ako su $B_{1},\,B_{2}\subseteq V$ baze VP-a $V$, tada $\exists f:B_{1}\overset{\mathrm{bijekcija}}{\longrightarrow} B_{2}$

**Def**. **Dimenzija** VP-a $V$ je kardinalni broj neke baze VP-a $V$.
Oznaka: $\dim V$

VP $V$ je konačno dimenzioni ako je $\dim V\in\mathbb{N}_{0}$

**Lema**. Neka je $B=\{ a_{1},\,a_{2},\,\dots,\,a_{n} \}$ skup generatora $V$, $S=\{ b_{1},\,b_{2},\,\dots,\,b_{m} \}\subseteq V$ je linearno nezavisan skup. Tada
$m\leqslant n\ \:$ i $\:\ \exists i_{1},\,i_{2},\,\dots\,i_{n-m}=\overline{1,n} \ \ :$
$\{ b_{1},\,b_{2}\,\dots,\,b_{m},\,a_{i_{1}},\,a_{i_{2}},\,\dots,\,a_{i_{n-m}} \}$ je baza $V$

**Stav**. $V$ je VP. $\dim V=n$. Tada:
1. $B\subseteq V,\ \ |B|>n\quad\Rightarrow\quad B$ je linearno zavisan;
2. $A\subseteq V$ je linearno nezavisan$,\ \ |A|=n\quad\Rightarrow\quad A$ je baza $V$;
3. $S$ je skup generatora $V,\ \ |S|=n\quad\Rightarrow\quad S$ je baza $V$;

**Stav**. $S$ je skup generatora konačno dim. VP-a $V$. Tada
maksimalan linearno nezavisan podskup $S$ je baza $V$

**Stav**. $A\subseteq V$ je linearno nezavisan, $V$ je konačno dim. VP. Tada
$A$ je podskup neke baze $V$, koji moguće dopuniti do baze.


### Potprostor
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
___
**Teorema**. Neka je $\mathcal{F}=\{ L_{i}\leqslant V\ \big|\ i\in I\}$ familija potprostora VP-a $V$.
**Presek potprostora** $\:\ L=\bigcap\limits_{i\,\in\, I}L_{i}\ \:$ je potprostor od $V$.
___
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
  
___
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
___
**Def**. $L,\,M\leqslant V$, $V$ je konačno dim. VP. Tada je **suma potprostora** $L+M=\mathcal{L}(L\cup M)$.
Suma je **direktna** ako $L\cap M=\{0\}.\ \:$ Oznaka: $L\oplus M$

**Teorema**. $L,\,M\leqslant V$, $V$ je VP. Tada
$L+M=\mathcal{L}(L\cup M)=\{v\ \ \big|\ \ v=l+m,\ \ l\in L,\ \ m\in M\}$

**Stav**. $L,\,M\leqslant V$, $V$ je VP. Tada
$L\oplus M\quad\Leftrightarrow\quad\forall v\in L+M\quad\exists!\big(l\in L,\,m\in M\big)\ \ :\ \ v=l+m.$

**Teorema** (Grasmanova formula). $L,\,M\leqslant V$, $V$ je VP. Tada $\dim(L+M)=\dim L+\dim M-\dim(L\cap M)$.

Posledica. $L\oplus M\quad\Leftrightarrow\quad\dim(L+M)=\dim L+\dim M.$

**Stav**. $\forall L\leqslant V\quad\exists M\leqslant V\ \ :\ \ L\oplus M=V.$

### Zavisnost koordinata vektora o bazi

**Def**. $V$ je VP dimenzije $n$ nad poljem $\mathbb{F}$, $\:$ $e=\{ e_{1},\,e_{2},\,\dots,\,e_{n} \}$ je neka baza VP-a $V$. Tada za bazu $e$, koordinatizacija je preslikavanje $\kappa_{e}:\ V\to \mathbb{F}^{n}$, koje je definisano formulom $\kappa_{e}(x)=\kappa_{e}\left( \sum\limits_{i=1}^{n}x_{i}\,e_{i} \right)=(x_{1},\,x_{2},\,\dots,\,x_{n})=x(e)$.

Svojstva $\kappa_{e}$:
- $\forall x,\,y\in V\quad \kappa_{e}(x+y)=\kappa_{e}(x)+\kappa_{e}(y)$
- $\forall x\in V,\ \forall \lambda\in \mathbb{F}\quad \kappa_{e}(\lambda\,x)=\lambda\,\kappa_{e}(x)$
- $\kappa_{e}$ je bijekcija