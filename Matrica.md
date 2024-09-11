#fax #math #laag [deo [[Linearna algebra|linearne algebre]]]
$\:$

$\mathbb{M}_{mn}(\mathbb{F})=\left\{\left(\begin{array}{c}a_{11}&a_{12}&\dots&a_{1n}\\a_{21}&a_{22}&\dots&a_{2n}\\\dots&\dots&\dots&\dots\\a_{m1}&a_{m2}&\dots&a_{mn}\end{array}\right)=(a_{ij})=\mathcal{A}\ \ \Bigg|\ \ a_{ij}\in \mathbb{F}\right\}$
— skup svih matrica $m\times n$ ($m$ vrsta, $n$ kolona).

**Stav**. $\mathbb{M}_{mn}(\mathbb{F})$ je VP uz operacije:
- (s) $\forall \mathcal{A}=(a_{ij}),\,\mathcal{B}=(b_{ij})\in \mathbb{M}_{mn}(\mathbb{F})$
  $\quad\quad \mathcal{A}+\mathcal{B}=(a_{ij})+(b_{ij})=(a_{ij}+b_{ij})$
- (ms) $\forall \mathcal{A}=(a_{ij})\in \mathbb{M}_{mn}(\mathbb{F}),\ \ \forall \lambda\in\mathbb{F}$
  $\quad\quad \lambda\,\mathcal{A}=\lambda\,(a_{ij})=(\lambda\,a_{ij})$
___
$\mathcal{A}_{m\times n}=(a_{ij})=\underbrace{\big[a^{1},\ a^{2},\ \dots,\ a^{m}\big]}_{\text{vrste}}=\underbrace{\big[a_{1},\ a_{2},\ \dots,\ a_{n}\big]}_{\text{kolone}}$

$a^{i}\in \mathbb{F}^{n},\ \ a_{j}\in\mathbb{F}^{m}\quad$ su vektori.

Sledeće oznake vrsta matrice su ekvivalentni: $\quad$$a^{i}\ \ \mathrm{i}\ \ (\mathcal{A})^{i}$
Sledeće oznake kolona matrice su ekvivalentni: $\quad$$a_{j}\ \ \mathrm{i}\ \ (\mathcal{A})_{j}$
___

Sledeće oznake elementa matrice su ekvivalentni:
$a_{ij}\quad\quad a^{i}_{j}\quad \quad(\mathcal{A})_{ij}\quad\quad(\mathcal{A})^{i}_{j}$

### Množenje matrica
**Def**. **Množenje matrica** je funkcija $\ \cdot:\ \mathbb{M}_{mn}(\mathbb{F})\times\mathbb{M}_{nk}(\mathbb{F})\to\mathbb{M}_{mk}(\mathbb{F})$.
takva da $\forall\mathcal{A}=(a_{ij})\in\mathbb{M}_{mn}(\mathbb{F})\quad\forall\mathcal{B}=(b_{ij})\in\mathbb{M}_{nk}(\mathbb{F})$$\quad$$\exists\mathcal{C}=(c_{ij})\in\mathbb{M}_{mk}(\mathbb{F})\ \ :\ \ \mathcal{C}=\mathcal{A}\cdot\mathcal{B},\quad$ gde $c_{ij}=\sum\limits_{l=1}^{n}a_{il}\,b_{lj}=a^{i}$ [[Projektovanje vektora i skalarni proizvod vektora#Skalarni proizvod u koordinatama|∙]] $b_{j}$

$\mathcal{A}\cdot\mathcal{B}=\big[a^{1},\ a^{2},\ \dots,\ a^{m}\big]\!\cdot\!\big[b_{1},\ b_{2},\ \dots,\ b_{k}\big]=\left(\begin{array}{c}a^{1}\cdot b_{1}&a^{1}\cdot b_{2}&\dots&a^{1}\cdot b_{k}\\a^{2}\cdot b_{1}&a^{2}\cdot b_{2}&\dots&a^{2}\cdot b_{k}\\\dots&\dots&\dots&\dots \\a^{m}\cdot b_{1}&a^{m}\cdot b_{2}&\dots&a^{m}\cdot b_{k}\end{array}\right)$

**Teorema** (asocijativnost množenja). $\mathcal{A}\in\mathbb{M}_{mn}(\mathbb{F}),\ \ \mathcal{B}\in\mathbb{M}_{nk}(\mathbb{F}),\ \ \mathcal{C}\in\mathbb{M}_{kl}(\mathbb{F}).$
Tada $\mathcal{A}\cdot(\mathcal{B}\cdot\mathcal{C})=(\mathcal{A}\cdot\mathcal{B})\cdot\mathcal{C}$
### Transponovanje

