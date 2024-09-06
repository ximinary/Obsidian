#fax #math #laag [deo poglavlja [[Vektor|"vektor"]]]

### Projektovanje
**Def**. **Osa** je prava sa vektorom ose $\ e=\overrightarrow{\rm EF}\ne\overrightarrow{\rm 0}$, gde su $\mathrm{E}$ i $\mathrm{F}$ tačke prave i $||e||=1$.

**Def**. **Paralelna vektor-projekcija** vektora $\mathbf{AB}$ na osu $s$ u odnosu na pravu $l$ je vektor $\mathbf{A'B'}$, takav da $\mathrm{A',\,B'}\in s;\ \ \ \mathrm{AA'} \parallel \mathrm{BB'}\parallel l.$

**Def**. **Paralelna skalar-projekcija** vektora $\mathbf{AB}$ na osu $s$ u odnosu na pravu $l$ je broj $\mathrm{pr}_{s}^{l}\ \mathbf{AB=}\begin{cases}||\mathbf{A'B'}||,\quad \text{ako su }\mathbf{A'B'}\ \  \text{i}\ \ e\ \ \text{istosmerni}\\-||\mathbf{A'B'}||,\quad \text{inače}\end{cases}$

Ako $||e||=1\:$ onda $\:\mathbf{A'B'}=\left(\mathrm{pr}_{s}^{l}\ \mathbf{AB}\right)\cdot e$ 
Ako je $l\perp s$, piše se $\mathrm{pr}_{s}\ \mathbf{AB}$

**Teorema**. $s$ je osa, tada $\mathrm{pr}_{s}\ \mathbf{AB}=||\mathbf{AB}||\cdot\cos \widehat{(\mathbf{AB},\,s)}$ ^59abbe

**Teorema**. Za $\forall \mathbf{AB},\,\mathbf{BC},\,\text{osu } s, \text{pravu }l\ \  (l\nparallel s)$ važi $\mathrm{pr}_{s}^{l}\ (\mathbf{AB}+\mathbf{BC})=\mathrm{pr}_{s}^{l}\ \mathbf{AB}+\mathrm{pr}_{s}^{l}\ \mathbf{BC}$

**Teorema** (Talesova). Za $\forall \mathbf{AB},\,\alpha\in\mathbb{R},\,\text{osu } s, \text{pravu }l\ \  (l\nparallel s)$ važi $\mathrm{pr}_{s}^{l}\ (\alpha\cdot\mathbf{AB})=\alpha\cdot\mathrm{pr}_{s}^{l}\ \mathbf{AB}$

### Skalarni proizvod

**Def**. **Skalarni** (unutrašnji) **proizvod** je funkcija$\ \ \cdot\,:\ V\times V\to\mathbb{R}$, takva da $\forall x,\,y\in V\quad x\cdot y=||x||\cdot||y||\cdot\cos \widehat{(x,\,y)}$

Oznake: $\ \ x\cdot y;\quad(x\,|\,y);\quad\langle x,\,y\rangle;\quad x\circ y$

Iz [[Projektovanje vektora i skalarni proizvod vektora#^59abbe|teoreme]] sledi $x\cdot y=||x||\cdot \mathrm{pr}_{x}\ y=||y||\cdot\mathrm{pr}_{y}\ x$

**Teorema** Ako su $x,\,y,\,z\in V,\ \alpha\in\mathbb{R}$ važe:
1. $(x+y)\cdot z=x\cdot z+y\cdot z$
2. $(\alpha\,x)\cdot y=\alpha\,(x\cdot y)$
3. $x\cdot y=y\cdot x$
4. $x\cdot x\geqslant0$
5. $x\cdot x=0\quad\Leftrightarrow\quad x=0$

> Dokaz: 3., 4. i 5. važe iz definicije.
> 1\. $(x+y)\cdot z=||z||\,\mathrm{pr}_{z}\ (x+y)=$ $=||z||\,\mathrm{pr}_{z}\ x+||z||\,\mathrm{pr}_{z}\ y=x\cdot z+y\cdot z$
> 2\. $(\alpha\,x)\cdot y=||y||\,\mathrm{pr}_{y}\ (\alpha\,x)=\alpha\,||y||\,\mathrm{pr}_{y}\ x=\alpha\,(x\cdot y)$

Lema. $x=y\quad\Leftrightarrow\quad\forall u \in V\quad x\cdot u=y\cdot u$

### Skalarni proizvod u koordinatama
Neka je $(e_{1},\,e_{2},\,\dots,\,e_{n})$ ortonormirana baza
$\Big($tj. važe $(\forall i \ne j=\overline{1,n}\quad e_{i}\cdot e_{j}=0)$ i $(\forall i =\overline{1,n}\quad||e_{i}||=1)$ $\Big)$

>Kronekerov simbol:
>$\delta_{ij}=\begin{cases}1,\quad i = j\\0,\quad i \ne j\end{cases}$
>$e_{i}\cdot e_{j}=\delta_{ij}$


$x = x_{1}\,e_{1}+x_{2}\,e_{2}+\dots+x_{n}\,e_{n}$
$y = y_{1}\,e_{1}+y_{2}\,e_{2}+\dots+y_{n}\,e_{n}$

tada $x\cdot y =\bigg(\sum\limits_{i=1}^{n}x_{i}\,e_{i}\bigg)\cdot\bigg(\sum\limits_{j=1}^{n}y_{j}\,e_{j}\bigg)=\sum\limits_{i,\,j=1}^{n}x_{i}\,y_{j}\,(e_{i}\cdot e_{j})=$
$=\sum\limits_{i,\,j=1}^{n}x_{i}\,y_{j}\,\delta_{ij}=\sum\limits_{i=1}^{n}x_{i}\,y_{i}$


### Primene skalarnog proizvoda

$x = x_{1}\,e_{1}+x_{2}\,e_{2}+\dots+x_{n}\,e_{n}$
$y = y_{1}\,e_{1}+y_{2}\,e_{2}+\dots+y_{n}\,e_{n}$

1. $||x||=\sqrt[]{x\cdot x}=\sqrt[]{\sum\limits_{i=1}^{n}x_{i}^{2}}$
2. $\begin{align}\cos\widehat{(x,\,y)}=\frac{x\cdot y}{||x||\,||y||}=\frac{\sum\limits_{i=1}^{n}x_{i}\,y_{i}}{\sqrt[]{\sum\limits_{i=1}^{n}x_{i}^{2}}\,\sqrt[]{\sum\limits_{i=1}^{n}y_{i}^{2}}}\end{align}$
3. $\begin{align}\frac{x}{||x||}=\frac{x_{1}}{||x||}\,e_{1}+\frac{x_{2}}{||x||}\,e_{2}+\dots+\frac{x_{n}}{||x||}\,e_{n}=\end{align}$
   $=\cos\widehat{(x,\,e_{1})}\,e_{1}+\cos\widehat{(x,\,e_{2})}\,e_{2}+\dots+\cos\widehat{(x,\,e_{n})}\,e_{n}$
   
   Odakle $\ \ \cos^{2}\widehat{(x,\,e_{1})}+\cos^{2}\widehat{(x,\,e_{2})}+\dots+\cos^{2}\widehat{(x,\,e_{n})}=1$
4. $\begin{align}\mathrm{pr}_{x}\ y=\frac{x\cdot y}{||x||}=\frac{\sum\limits_{i=1}^{n}x_{i}\,y_{i}}{\sqrt[]{\sum\limits_{i=1}^{n}x_{i}^{2}}}\end{align}$