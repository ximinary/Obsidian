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
- $A(0)=0$
- $A(-x)=-A(x)$
### Primeri LO
- **Nula preslikavanje**. $\mathbb{O}:\ U\to V$ def. sa $\:$ $\forall x\in U\quad \mathbb{O}(x)=\mathbf{0}\in V$.
- **Identičko preslikavanje**. $\mathrm{id}:\ V\to V$ def. sa $\:$ $\forall x\in V\quad \mathrm{id}(x)=x$.
- **Projekcije**.
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
### Slika i jezgro. Rang i defekt
Napomene: [[direktna i inverzna slika skupa]], [[Potprostor. Operacije nad potprostorima|potprostor]]

Stav. $A\in \mathrm{Hom}(U,\,V)$. Tada
- $U_{1}\leqslant U\quad\Rightarrow\quad A[U_{1}] \leqslant V$
- $V_{1}\leqslant V\quad\Rightarrow\quad A^{-1}[V_{1}] \leqslant U$
___
$\:$
**Def**. $A\in \mathrm{Hom}(U,\,V)$. Tada
- **slika** lin. operatora $A$ je $\ \mathrm{Im}\,A=\Big\{ A(u)\ \Big|\ u\in U \Big\}=A[U]\subseteq V$
- **jezgro** lin. operatora $A$ je $\ \mathrm{Ker}\,A=\Big\{ u\in U\ \Big| \ A(u) = \mathbf{0} \Big\}= A^{-1}[\mathbf{0}]\subseteq U$

Stav. $A\in \mathrm{Hom}(U,\,V)$. Tada
- $\mathrm{Im}\,A\leqslant V$
- $\mathrm{Ker}\,A\leqslant U$
- $\mathrm{Ker}\,A=\{ 0 \}\quad\Leftrightarrow\quad A$ je monomorfizam (1-1)
___
**Def**. $A\in \mathrm{Hom}(U,\,V)\quad\dim U,\,V\in\mathbb{N}$. Tada
- **rang** $A$ je $\mathrm{rang}\,A=\mathrm{Rank}\,A=\dim(\mathrm{Im}\,A)$
- **defekt** $A$ je $\mathrm{defekt}\,A=\mathrm{Nullity}\,A=\dim(\mathrm{Ker}\,A)$

**Teorema** (o rangu i defektu). $A\in \mathrm{Hom}(U,\,V)\quad\dim U,\,V\in\mathbb{N}$. Tada $\boxed{\mathrm{rang}\,A\,+\,\mathrm{defekt}\,A\,=\,\dim U}$

Posledica 1. 

Posledica 2. 

Posledica 3. 


### Algebra $\mathrm{Hom}\,V$
### Matrica LO
### [[Zavisnost koordinata vektora i matrice linearnog operatora o bazi#Zavisnost matrice operatora o bazi|Zavisnost matrice LO o bazi]]
### Linearni funkcional
### Anihilator
