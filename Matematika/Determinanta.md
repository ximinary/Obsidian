#fax #math #laag [deo poglavlja [[Matrica|"matrica"]]]
$\:$

[[Grupa permutacija]]

**Def**. Determinanta je funkcija $\det:\ \mathbb{M}_{n}(\mathbb{F})\to\mathbb{F}$ def. sa $\forall \mathcal{A}=(a_{ij})\in\mathbb{M}_{n}(\mathbb{F})\quad \det\mathcal{A}=\sum\limits_{\sigma\,\in\,\mathbb{S}_{n}}(-1)^{I(\sigma)}\,a_{1\sigma(1)}\,a_{2\sigma(2)}\,\cdot\!\cdot\!\cdot\,a_{n\sigma(n)}$

Oznaka: $\det\mathcal{A}=|a_{ij}|=\left|\begin{array}{}a_{11}&a_{12}&\dots&a_{1n}\\a_{21}&a_{22}&\dots&a_{2n}\\\dots&\dots&\dots&\dots\\a_{n1}&a_{n2}&\dots&a_{nn}\end{array}\right|$
___
Stav. $\mathcal{A}=(a_{ij})\in \mathbb{M}_{n}(\mathbb{F})$
1. Vrsta/kolona matrice sastoji od nula $\ \ \Rightarrow\ \ \det \mathcal{A}=0$
2. Dve vrste/kolone matrice su proporcijalne $\ \ \Rightarrow\ \ \det \mathcal{A}=0$
3. $\det\mathcal{A}=\det\mathcal{A^{\rm T}}$
4. $\mathcal{A}$ je trougaona $\Big(\forall i \underset{(>)}{<} j \quad a_{ij}=0\Big)$ $\ \ \Rightarrow\ \ \det \mathcal{A}=a_{11}\,a_{22}\,\cdot\!\cdot\!\cdot\,a_{nn}$
___
Lema. $\mathcal{A,\,B,\,D}$ su kvadratne matrice takve da $\mathcal{A}=\left(\begin{array}{}\mathcal{B}&\mathcal{C}\\\mathcal{O}&\mathcal{D}\end{array}\right)$. Tada $\det \mathcal{A}=\det \mathcal{B}\cdot\det\mathcal{D}$
___
Teorema. $\mathcal{A}=(a_{ij})=\underbrace{\big[a^{1},\ a^{2},\ \dots,\ a^{n}\big]}_{\text{vrste}}=\underbrace{\big[a_{1},\ a_{2},\ \dots,\ a_{n}\big]}_{\text{kolone}}\in \mathbb{M}_{n}(\mathbb{F})$
svojstva za vrste (za kolone su analogne):
1. $\det\big[a^{1},\ a^{2},\ \dots,\ \lambda\,a^{i},\ \dots,\ a^{n}\big]=\lambda\,\det\mathcal{A},\ \:$ $\forall i=\overline{1,n}\ \ \ \forall \lambda \in \mathbb{F}$
   — množenje vrste skalarom
   $\:$
2. $\det\big[a^{1},\ a^{2},\ \dots,\ a^{i}+b,\ \dots,\ a^{n}\big]=$ 
   $=\big[a^{1},\ a^{2},\ \dots,\ a^{i},\ \dots,\ a^{n}\big]+\big[a^{1},\ a^{2},\ \dots,\ b,\ \dots,\ a^{n}\big],\ \:$ $\forall i=\overline{1,n}\ \ \ \forall b \in \mathbb{F}^{n}$
   $\:$
3. $\det\big[a^{1},\ a^{2},\ \dots,\ a^{i},\ a^{i+1},\ \dots,\ a^{n}\big]=$ 
   $=-\big[a^{1},\ a^{2},\ \dots,\ a^{i+1},\ a^{i},\ \dots,\ a^{n}\big],\ \:$ $\forall i=\overline{1,n\!\!-\!\!1}$
   — zamena dve susedne vrste

Posledica.
1. Zamena mesta dve vrste se svodi na neparan broj zamena susednih vrsta, tj. zamena mesta dve vrste menja znak determinante.
2. $\det\big[a^{1},\ a^{2},\ \dots,\ a^{i}+\sum\limits_{j\ne i}\lambda_{j}\,a^{j},\ \dots,\ a^{n}\big]=\det\mathcal{A},\ \:$ $\forall i=\overline{1,n}\ \ \ \forall \lambda_{j} \in \mathbb{F}$

### [[Rang matrice. Elementarne transformacije#Elementarne transformacije|Elementarne transformacije]] i determinanta
Svojstva 1. i 3. iz teorema i 2. iz posledice se mogu realizovati množenjem sa elementarnim matricama sa leva (vrste) i sa desna (kolone).

Stav. $\mathcal{A}\in \mathbb{M}_{n}(\mathbb{F}),\ \ \ \mathrm{E}\in\mathbb{M}_{n}(\mathbb{F})$ — elementarna matrica. Tada $\det(\mathrm{E}\cdot\mathcal{A})=\det(\mathcal{A}\cdot\mathrm{E})=\det\mathcal{A}$

Teorema (Bine-Košijeva).
$\forall\mathcal{A},\,\mathcal{B}\in \mathbb{M}_{n}(\mathbb{F})\quad\det(\mathcal{A}\cdot\mathcal{B})=\det\mathcal{A}\cdot\det\mathcal{B}$ ^47b633

Teorema. $\mathcal{A}\in \mathbb{M}_{n}(\mathbb{F})$.
$\mathcal{A}$ je [[Inverzna matrica|invertibilna]] $\quad\Leftrightarrow\quad \det \mathcal{A}\ne 0$

### Laplasov razvoj
$\mathcal{A}=(a_{ij})\in\mathbb{M}_{n}(\mathbb{F})$

$$
\mathcal{A}=\left(\begin{array}{cccc|c|cccc}
a_{11}&a_{12}&\dots&a_{1(j-1)}&a_{1j}&a_{1(j+1)}&\dots&a_{1(n-1)}&a_{1n}\\
a_{21}&a_{22}&\dots&a_{2(j-1)}&a_{1j}&a_{2(j+1)}&\dots&a_{2(n-1)}&a_{2n}\\ 
\dots&\dots&\dots&\dots&\dots&\dots&\dots&\dots&\dots\\
a_{(i-1)1}&a_{(i-1)2}&\dots&a_{(i-1)(j-1)}&a_{(i-1)j}&a_{(i-1)(j+1)}&\dots&a_{(i-1)(n-1)}&a_{(i-1)n}\\\hline
a_{i1}&a_{i2}&\dots&a_{i(j-1)}&a_{ij}&a_{i(j+1)}&\dots&a_{i(n-1)}&a_{in} \\\hline
a_{(i+1)1}&a_{(i+1)2}&\dots&a_{(i+1)(j-1)}&a_{(i+1)j}&a_{(i+1)(j+1)}&\dots&a_{(i+1)(n-1)}&a_{(i+1)n}\\
\dots&\dots&\dots&\dots&\dots&\dots&\dots&\dots&\dots\\
a_{(n-1)1}&a_{(n-1)2}&\dots&a_{(n-1)(j-1)}&a_{(n-1)j}&a_{(n-1)(j+1)}&\dots&a_{(n-1)(n-1)}&a_{(n-1)n} \\
a_{n1}&a_{n2}&\dots&a_{n(j-1)}&a_{nj}&a_{n(j+1)}&\dots&a_{n(n-1)}&a_{nn}\end{array}\right)
$$

**Def**. **Minora** $\Delta_{ij}(\mathcal{A})$  je determinanta matrice, koja se dobija izbacivanjem $i$-te vrste i $j$-te kolone iz matrice $\mathcal{A}$.

 $$
\Delta_{ij}(\mathcal{A})=
\left|\begin{array}{}
a_{11}&a_{12}&\dots&a_{1(j-1)}&a_{1(j+1)}&\dots&a_{1(n-1)}&a_{1n}\\
a_{21}&a_{22}&\dots&a_{2(j-1)}&a_{2(j+1)}&\dots&a_{2(n-1)}&a_{2n}\\ 
\dots&\dots&\dots&\dots&\dots&\dots&\dots&\dots\\
a_{(i-1)1}&a_{(i-1)2}&\dots&a_{(i-1)(j-1)}&a_{(i-1)(j+1)}&\dots&a_{(i-1)(n-1)}&a_{(i-1)n}\\
a_{(i+1)1}&a_{(i+1)2}&\dots&a_{(i+1)(j-1)}&a_{(i+1)(j+1)}&\dots&a_{(i+1)(n-1)}&a_{(i+1)n}\\
\dots&\dots&\dots&\dots&\dots&\dots&\dots&\dots\\
a_{(n-1)1}&a_{(n-1)2}&\dots&a_{(n-1)(j-1)}&a_{(n-1)(j+1)}&\dots&a_{(n-1)(n-1)}&a_{(n-1)n} \\
a_{n1}&a_{n2}&\dots&a_{n(j-1)}&a_{n(j+1)}&\dots&a_{n(n-1)}&a_{nn}\end{array}\right|
 $$
$\:$

**Def**. **Kofaktor** elementa $a_{ij}$ matrice $\mathcal{A}$ je broj $\mathbf{A}_{ij}=(-1)^{i+j}\,\Delta_{ij}(\mathcal{A})$

$\widetilde{\mathcal{A}}=(\mathbf{A}_{ij})\in\mathbb{M}_{n}(\mathbb{F})$ je **matrica kofaktora** matrice $\mathcal{A}$.

$\mathrm{adj}\,\mathcal{A} = (\widetilde{\mathrm{\cal A}})^{\rm T}\in\mathbb{M}_{n}(\mathbb{F})$ je **adjungovana matrica** matrice $\mathcal{A}$.
$\:$

Teorema (Laplasov razvoj).
- Razvoj po $i$-toj vrsti:
  $\det \mathcal{A}=\sum\limits_{j=1}^{n}a_{ij}\,\mathbf{A}_{ij},\quad \forall i=\overline{1,n}$
  $\:$
- Razvoj po $j$-toj koloni:
$\det\mathcal{A}=\sum\limits_{i=1}^{n}a_{ij}\,\mathbf{A}_{ij},\quad \forall j=\overline{1,n}$
$\:$

Lema.
- $\sum\limits_{j=1}^{n}a_{ij}\,\mathbf{A}_{kj}=0,\quad \forall i\ne k=\overline{1,n}$
  $\:$
- $\sum\limits_{i=1}^{n}a_{ij}\,\mathbf{A}_{ik}=0,\quad \forall j\ne k=\overline{1,n}$
$\:$

Posledica. $\boxed{\begin{align}\mathcal{A}^{-1}=\frac{1}{\det \mathcal{A}}\,\mathrm{adj}\,\mathcal{A} \end{align}}$
> Iz teoreme i leme: $\ \:$ $\forall i,\,k=\overline{1,n}$
> $\sum\limits_{j=1}^{n}a_{ij}\,\mathbf{A}_{kj}=\delta_{ik}\,\det \mathcal{A}$
> $\sum\limits_{j=1}^{n}a_{ij}(\widetilde{\cal A})_{kj}=\delta_{ik}\,\det \mathcal{A}$
> $\sum\limits_{j=1}^{n}a_{ij}\Big((\widetilde{\cal A})^{\rm T}\Big)_{jk}=\delta_{ik}\,\det \mathcal{A}$
> $\mathcal{A}\cdot(\widetilde{\cal A})^{\rm T}=(\det\mathcal{A})\,\mathbb{I}_{n}$
> $\mathcal{A}\cdot\left(\frac{1}{\det\mathcal{A}}\,\mathrm{adj}\,\mathcal{A}\right)=\mathbb{I}_{n}$
### Determinanta Vandermonda
$\mathrm{V}(a_{1},\,a_{2},\,\dots,\,a_{n})=\left|\begin{array}{c} 1&1&\dots&1\\a_{1}&a_{2}&\dots&a_{n}\\a_{1}^{2}&a_{2}^{2}&\dots&a_{n}^{2}\\a_{1}^{3}&a_{2}^{3}&\dots&a_{n}^{3}\\ \dots&\dots&\dots&\dots\\ a_{1}^{n-1}&a_{2}^{n-1}&\dots&a_{n}^{n-1}\end{array}\right|=\prod\limits_{i<j}(a_{j}-a_{i})$