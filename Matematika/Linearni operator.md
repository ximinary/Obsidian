#fax #math #laag [deo [[Linearna algebra|linearne algebre]]]
$\:$
**Def**. Neka su $U$ i $V$ [[Vektorski prostor|vektorski prostori]] nad istim poljem $\mathbb{F}$. [[Funkcija|Preslikavanje]] $A:\ U\to V$ se zove **linearni operator** (linearna transformacija), ako važi jedan od ekvivalentnih uslova:
- $\forall x,\,y\in U,\ \ \forall \alpha\in\mathbb{F}\quad\quad\ \ \begin{cases}A(x+y)=A(x)+A(y)\\ A(\alpha\,x)=\alpha\,A(x)\end{cases}$
- $\forall x,\,y\in U,\ \ \forall \alpha,\,\beta\in\mathbb{F}\quad\ \  A(\alpha\,x+\beta\,y)=\alpha\,A(x)+\beta\,A(y)$
- $\forall x,\,y\in U,\ \ \forall \alpha\in\mathbb{F}\quad\quad\ \ \ A(\alpha\,x+y)=\alpha\,A(x)+A(y)$
$\:$

**Def**. \_\_\_ linearni operator se zove \_\_\_:
$\begin{array}{r l} \\
\text{injektivni (1-1)}&\to&\text{monomorfizam} \\
\text{surjektivni (na)}&\to&\text{epimorfizam} \\
\text{bijektivni}&\to&\text{izomorfizam} \\
U=V&\to&\text{endomorfizam} \\
\text{bijektivni i } U=V &\to&\text{automorfizam}
\end{array}$
$\:$ ^86cf6f

Oznake:
$\mathrm{Hom}_{_{\mathbb{F}}}(U,\,V)\ \:$ — skup svih LO sa $U$ u $V$.
$\mathrm{Hom}_{_{\mathbb{F}}}\,V\quad\quad\ \:$ — skup svih LO sa $V$ u $V$ (svih endomorfizama).
($\mathbb{F}$ se ne piše, ako se i tako zna nad kojem poljem)

Stav. $A\in\mathrm{Hom}(U,\,V)$. Tada
- $A(\mathbf{0})=\mathbf{0}$
- $A(-x)=-A(x)$
$\:$

Lema. LO $A\in \mathrm{Hom}(U,\,V)$ je u potpunosti određen svojim dejstvom na bazi $e$ VP-a $U$.
> Dokaz:
> $e =(e_{1},\,e_{2},\,\dots,\,e_{n})$ je baza od $U$.
> $g_{i}:=A(e_{i}),\ \ \forall i=\overline{1,n}\ \ \:$ — slike baznih vektora (dejstvo $A$ na bazi $e$).
> 
> $\forall u\in U\quad u=\sum\limits_{i=1}^{n}u_{i}\,e_{i}$
> 
> $A(u)=A\left( \sum\limits_{i=1}^{n}u_{i}\,e_{i}\right)\xlongequal{\text{linearnost}\ A}\sum\limits_{i=1}^{n}u_{i}\,A(e_{i})=\sum\limits_{i=1}^{n}u_{i}\,g_{i}$

^e71ccc

### Primeri LO
- **Nula preslikavanje**. $\mathbb{O}:\ U\to V$ def. sa $\:$ $\forall x\in U\quad \mathbb{O}(x)=\mathbf{0}\in V$.
- **Identičko preslikavanje**. $\mathrm{id}:\ V\to V$ def. sa $\:$ $\forall x\in V\quad \mathrm{id}(x)=x$.
- **Projektor** — LO za koji važi $P\circ P=P$.
  Na primer projekcija na ravan $x_{1}\,x_{3}$ u $\mathbb{R}^{4}$:
  $P:\ \mathbb{R}^{4}\to\mathbb{R}^{4}$ def. sa $\:$ $P(x_{1},\,x_{2},\,x_{3},\,x_{4})=P(x_{1},\,0,\,x_{3},\,0)$ je LO:
  $\:$
  $\forall x=(x_{1},\,x_{2},\,x_{3},\,x_{4}),\ y = (y_{1},\,y_{2},\,y_{3},\,y_{4})\in\mathbb{R}^{4},\ \ \forall\alpha\in\mathbb{R}$
   $P(\alpha\,x+y)=P(\alpha\,x_{1}+y_{1},\,\alpha\,x_{2}+y_{2},\,\alpha\,x_{3}+y_{3},\,\alpha\,x_{4}+y_{4})=$
  $=(\alpha\,x_{1}+y_{1},\,0,\,\alpha\,x_{3}+y_{3},\,0)=\alpha\,(x_{1},\,0,\,x_{3},\,0)+(y_{1},\,0,\,y_{3},\,0)=$
  $=\alpha\,P(x)+P(y)$
  $\:$
- **Diferencirane**. $V$ je VP svih glatkih funkcija na $\mathbb{R}$. Tada $\mathbb{D}=\frac{\mathrm{d}}{\mathrm{d}t}:\ V\to V$ je LO:
  $\:$
  $\forall f,\,g\in V,\ \ \forall \alpha\in\mathbb{R}\quad\ \ \mathbb{D}(f+g)=\mathbb{D}(f)+\mathbb{D}(g);\ \ \mathbb{D}(\alpha\,f)=\alpha\,\mathbb{D}(f)$

### Kompozicija LO
Stav. [[Kompozicija funkcija|Kompozicija]] LO je LO:
$A= \mathrm{Hom}(U,\,V),\ \ B= \mathrm{Hom}(V,\,W)$.
$B\circ A:\ U\to W$ def. sa $\ \forall u\in U\quad(B\circ A)(u)=B(A(u))$
Tada $B\circ A \in \mathrm{Hom}(U,\,W)$

Stav (svojstva kompozicije LO).
1. $\forall A\in \mathrm{Hom}(V,\,W)\quad\forall B,\,C\in \mathrm{Hom}(U,\,V)$
   $A\circ(B+C)=A\circ B+A\circ B$
2. $\forall A,\,B\in \mathrm{Hom}(V,\,W)\quad\forall C\in \mathrm{Hom}(U,\,V)$
   $(A+B)\circ C=A\circ C+B\circ C$
3. $\forall A\in \mathrm{Hom}(V,\,W)\quad\forall B\in \mathrm{Hom}(U,\,V)\quad\forall\lambda\in\mathbb{F}$
   $\lambda\,(A\circ B)=(\lambda\,A)\circ B=A\circ (\lambda\,B)$
___
$( \mathrm{Hom}\,V,\ \circ)$ je monoid jer kompozicija LO je:
- zatvorena: $\forall A,\,B\in \mathrm{Hom}\,V\quad A\circ B\in \mathrm{Hom}\,V$
- asocijativna
- postoji neutral: $\mathrm{id}_{V}\in \mathrm{Hom}\,V$

$A$ ima [[Inverzna funkcija#^d44f5e|inverz]] $A^{-1}\in \mathrm{Hom}\,V$ $\quad\Leftrightarrow\quad A$ je izomorfizam (bijekcija)

### VP $\mathrm{Hom}(U,\,V)$ i algebra $\mathrm{Hom}\,V$

Stav. $\Big( \mathrm{Hom}_{_{\mathbb{F}}}(U,\,V),\,\mathbb{F},\,+,\,\cdot\Big)$ je [[Vektorski prostor|VP]] uz operacije:
- (s) $\forall A,\,B\in \mathrm{Hom}(U,\,V),\ \ \forall u\in U$
  $\quad\quad (A+B)(u)=A(u)+B(u)$
- (ms) $\forall A\in \mathrm{Hom}(U,\,V),\ \ \forall \lambda\in\mathbb{F},\ \ \forall u\in U$
  $\quad\quad (\lambda\,A)(u)=\lambda\,A(u)$

Nula preslikavanje $\mathbb{O}$ kao neutral za sabiranje.

Stav. $e = (e_{1},\,e_{2},\,\dots,\,e_{n})$ je baza $U$; $f= (f_{1},\,f_{2},\,\dots,\,f_{m})$ je baza $V$.
$E_{ij}$ je LO, tako da $\forall k \in\overline{1,n}\quad E_{ij}(e_{k})=\delta_{jk}\,f_{i}=\begin{cases}f_{i},&\text{ako }k = j\\\mathbf{0},&\text{ako }k \ne j\end{cases}$
Tada $E = \{ E_{ij}\ \big| \ i=\overline{1,m}\quad j=\overline{1,n}\}$ je **baza** $\mathrm{Hom}(U,\,V)$.
Specijalno: $\mathrm{dim}\big(\mathrm{Hom}(U,\,V)\big)=\mathrm{dim}\,U\cdot\mathrm{dim}\,V$
___
Stav. $( \mathrm{Hom}\,V,\,\mathbb{F},\,+,\,\circ,\,\cdot)$ je asocijativna $\mathbb{F}$-[[Algebra nad poljem|algebra]] sa jedinicom.

Identičko preslikavanje $id_{V}$ kao neutral za kompoziciju.

### [[Slika i jezgro, rang i defekt linearnog operatora. Regularni operator|Slika i jezgro, rang i defekt LO. Regularni operator]]
### [[Matrica linearnog operatora]]
### [[Linearni funkcional]]
### [[Kvadratna matrica#Sličnost matrica|Invarianta sličnosti]]