#fax #math #geom  [deo [[Geometrija|geometrije]] i poglavlja [[Brojevi|"brojevi"]]]
$\:$

$\mathbb{H}=\{ ai +bj+ck+d\ \big|\ a,\,b,\,c,\,d\in\mathbb{R} \}$
$\boxed{i^{2}=j^{2}=k^{2}=ijk=-1}$

Konjugovanje: $\overline{ai+bj+ck+d}=-ai-bj-ck+d$
Apsolutna vrednost: $|ai+bj+ck+d|=\sqrt[]{a^{2}+b^{2}+c^{2}+d^{2}}$

$\forall q,\,q_{1},\,q_{2},\,q_{3} \in \mathbb{H}$
Abelova grupa $(\mathbb{H},\, +)$:
$(a_{1}i+b_{1}j+c_{1}k+d_{1})+(a_{2}i+b_{2}j+c_{2}k+d_{2}):=(a_{1}+a_{2})i+(b_{1}+b_{2})j+(c_{1}+c_{2})k+(d_{1}+d_{2})$
1. $q_{1} + (q_{2} + q_{3}) =(q_{1} + q_{2}) + q_{3}$
2. $\exists !0\in \mathbb{R}\ :\ q + 0 = 0 + q = q$
3. $\exists(-q)\in\mathbb{R}\ : \ q + (-q) = (-q)+q = 0$
   za $q=ai+bj+ck+d$, $\quad$ $-q=(-a)i+(-b)j+(-c)k+(-d)$
4. $q_{1} + q_{2} = q_{2} + q_{1}$

Grupa $(\mathbb{H}\setminus\{0\},\, \cdot)$:
$(a_{1}i+b_{1}j+c_{1}k+d_{1})\cdot(a_{2}i+b_{2}j+c_{2}k+d_{2})$ definisano sa:

$\begin{array}{}ij=k&&ji=-k&&k^{2}=-1\\jk=i&&kj=-i&&i^{2}=-1\\ki=j&&ik=-j&&j^{2}=-1\end{array}$

5. $q_{1}\cdot (q_{2}\cdot q_{3}) =(q_{1}\cdot q_{2})\cdot q_{3}$
6. $\exists !1\in \mathbb{H}\ :\ q \cdot 1 = 1 \cdot q = q$
7. $\begin{align}\exists(q^{-1}):=\frac{\overline{q}}{|q|^{2}}\ \ :\ \ q\cdot (q^{-1}) = (q^{-1})\cdot q = 1\end{align}$

Važi $x\cdot y \ne y\cdot x$
$\:$


Neka je $q = ai+bj+ck+d$
Realni deo $\mathfrak{R}(q)=d$
Imaginarni deo $\mathfrak{I}(q)=ai+bj+ck\quad\longleftrightarrow\quad \overrightarrow{v}=(a,\,b,\,c)\in\mathbb{R}^{3}$
Tada $q=[(a,\,b,\,c),\,d]=[\overrightarrow{v},\,d]$

### Konjugacija
**Def**. Svaki $q\in\mathbb{H},\ q\ne 0$ određuje **konjugaciju** — preslikavanje $C_{q}:\mathbb{H}\to\mathbb{H}$ def. sa $C_{q}(p)=q\,p\,q^{-1}$.

Lema. $q,\,h\in\mathbb{H}$. $C_{q}$ i $C_{h}$ su isti $\quad\Leftrightarrow\quad$ $\exists\lambda\in\mathbb{R}\ \ :\ \ q= \lambda\,h$

$C_{h}\circ C_{q}=C_{h\cdot q}$

$C_{q}$ je izometrija prostora $\mathfrak{I}(\mathbb{H})$ i $\mathbb{R}^{3}$

**Stav**. Ako važi $q = [\,\overrightarrow{v}\, \sin \varphi,\, \cos \varphi]$ i $|\,\overrightarrow{v}\,| = 1$, preslikavanje $C_{q}$
je rotacija za ugao $2\varphi$ oko vektora $\overrightarrow{v}$ u pozitivnom smeru.