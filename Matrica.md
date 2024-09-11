#fax #math #laag [deo [[Linearna algebra|linearne algebre]]]
$\:$

$\mathbb{M}_{mn}(\mathbb{F})=\left\{\left(\begin{array}{c}a_{11}&a_{12}&\dots&a_{1n}\\a_{21}&a_{22}&\dots&a_{2n}\\\dots&\dots&\dots&\dots\\a_{m1}&a_{m2}&\dots&a_{mn}\end{array}\right)=(a_{ij})=\mathcal{A}\ \ \Bigg|\ \ a_{ij}\in \mathbb{F}\right\}$
— skup svih matrica $m\times n$ ($m$ vrsta, $n$ kolona).

**Stav**. $\mathbb{M}_{mn}(\mathbb{F})$ je [[Vektorski prostor|VP]] uz operacije:
- (s) $\forall \mathcal{A}=(a_{ij}),\,\mathcal{B}=(b_{ij})\in \mathbb{M}_{mn}(\mathbb{F})$
  $\quad\quad \mathcal{A}+\mathcal{B}=(a_{ij})+(b_{ij})=(a_{ij}+b_{ij})$
- (ms) $\forall \mathcal{A}=(a_{ij})\in \mathbb{M}_{mn}(\mathbb{F}),\ \ \forall \lambda\in\mathbb{F}$
  $\quad\quad \lambda\,\mathcal{A}=\lambda\,(a_{ij})=(\lambda\,a_{ij})$
$\:$

Nula matrica je neurtal za sabiranje:
$\mathcal{O}_{m\times n}=\left(\begin{array}{c}0&0&\dots&0\\0&0&\dots&0\\\dots&\dots&\dots&\dots\\0&0&\dots&0\end{array}\right)$
$\forall \mathcal{A}\in\mathbb{M}_{mn}(\mathbb{F})\quad\mathcal{A}+\mathcal{O}=\mathcal{O}+\mathcal{A}=\mathcal{A}$
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
Tada $\mathcal{A}\cdot(\mathcal{B}\cdot\mathcal{C})=(\mathcal{A}\cdot\mathcal{B})\cdot\mathcal{C}$ ^9c7738
> Dokaz:
> $\Big(\big(\mathcal{A\cdot\mathcal{B}}\big)\cdot\mathcal{C}\Big)^{i}_{j}=\big(\mathcal{A\cdot\mathcal{B}}\big)^{i}\cdot\mathcal{C}_{j}=\sum\limits_{p=1}^{k}\big(\mathcal{A}\cdot\mathcal{B}\big)^{i}_{p}\cdot\big(\mathcal{C}\big)^{p}_{j}=$
> $=\sum\limits_{p=1}^{k}\Big(\big(\mathcal{A}\big)^{i}\cdot\big(\mathcal{B}\big)_{p}\Big)\cdot\big(\mathcal{C}\big)^{p}_{j}=\sum\limits_{p=1}^{k}\Big( \sum\limits_{s=1}^{n}\big(\mathcal{A}\big)^{i}_{s}\cdot\big(\mathcal{B}\big)^{s}_{p}\Big)\cdot\big(\mathcal{C}\big)^{p}_{j}=$
> $=\sum\limits_{p=1}^{k}\sum\limits_{s=1}^{n}\big(\mathcal{A}\big)^{i}_{s}\cdot\big(\mathcal{B}\big)^{s}_{p}\cdot\big(\mathcal{C}\big)^{p}_{j}=\sum\limits_{s=1}^{n} \big(\mathcal{A}\big)^{i}_{s}\cdot\Big(\sum\limits_{p=1}^{k}\big(\mathcal{B}\big)^{s}_{p}\cdot\big(\mathcal{C}\big)^{p}_{j}\Big)=$
> $=\sum\limits_{s=1}^{n} \big(\mathcal{A}\big)^{i}_{s}\cdot\Big(\big(\mathcal{B}\big)^{s}\cdot\big(\mathcal{C}\big)_{j}\Big)=\sum\limits_{s=1}^{n} \big(\mathcal{A}\big)^{i}_{s}\cdot\big(\mathcal{B}\cdot\mathcal{C}\big)^{s}_{j}=$
> $=\big(\mathcal{A}\big)^{i}\cdot\big(\mathcal{B}\cdot\mathcal{C}\big)_{j}=\Big(\mathcal{A\cdot\big(\mathcal{B}}\cdot\mathcal{C}\big)\Big)^{i}_{j}$

$\:$

Stav (svojstva množenja matrica). ^f65329
1. $\forall \mathcal{A}\in\mathbb{M}_{mn}(\mathbb{F})\quad\forall\mathcal{B},\,\mathcal{C}\in\mathbb{M}_{nk}(\mathbb{F})\quad$
   $\mathcal{A}\cdot(\mathcal{B}+\mathcal{C}) = \mathcal{A}\cdot\mathcal{B}+\mathcal{A}\cdot\mathcal{C}$
   $\:$ ^66baee
2. $\forall \mathcal{A},\,\mathcal{B}\in\mathbb{M}_{mn}(\mathbb{F})\quad\forall\mathcal{C}\in\mathbb{M}_{nk}(\mathbb{F})\quad$
   $(\mathcal{A}+\mathcal{B})\cdot\mathcal{C} = \mathcal{A}\cdot\mathcal{C}+\mathcal{B}\cdot\mathcal{C}$
   $\:$ ^43f815
3.  $\forall \mathcal{A}\in\mathbb{M}_{mn}(\mathbb{F})\quad\forall\mathcal{B}\in\mathbb{M}_{nk}(\mathbb{F})\quad\forall\lambda \in \mathbb{F}\quad$
   $\lambda(\mathcal{A}\cdot\mathcal{B})=(\lambda\,\mathcal{A})\cdot\mathcal{B}=\mathcal{A}\cdot(\lambda\mathcal{B})$ ^fda602

> Dokaz 1.
> $\mathcal{A}\cdot(\mathcal{B}+\mathcal{C}) = \big[a^{1},\ a^{2},\ \dots,\ a^{m}\big]\!\cdot\!\big[b_{1}+c_{1},\ b_{2}+c_{2},\ \dots,\ b_{k}+c_{k}\big]=$
> 
> $=\left(\begin{array}{c}a^{1}\cdot (b_{1}+c_{1})&a^{1}\cdot (b_{2}+c_{2})&\dots&a^{1}\cdot (b_{k}+c_{k})\\a^{2}\cdot (b_{1}+c_{1})&a^{2}\cdot (b_{2}+c_{2})&\dots&a^{2}\cdot (b_{k}+c_{k})\\\dots&\dots&\dots&\dots \\a^{m}\cdot (b_{1}+c_{1})&a^{m}\cdot (b_{2}+c_{2})&\dots&a^{m}\cdot (b_{k}+c_{k})\end{array}\right)=$
> 
>  $=\left(\begin{array}{c}a^{1}\cdot b_{1}&a^{1}\cdot b_{2}&\dots&a^{1}\cdot b_{k}\\a^{2}\cdot b_{1}&a^{2}\cdot b_{2}&\dots&a^{2}\cdot b_{k}\\\dots&\dots&\dots&\dots \\a^{m}\cdot b_{1}&a^{m}\cdot b_{2}&\dots&a^{m}\cdot b_{k}\end{array}\right)+\left(\begin{array}{c}a^{1}\cdot c_{1}&a^{1}\cdot c_{2}&\dots&a^{1}\cdot c_{k}\\a^{2}\cdot c_{1}&a^{2}\cdot c_{2}&\dots&a^{2}\cdot c_{k}\\\dots&\dots&\dots&\dots \\a^{m}\cdot c_{1}&a^{m}\cdot c_{2}&\dots&a^{m}\cdot c_{k}\end{array}\right)=$
>  
>$=\mathcal{A}\cdot\mathcal{B}+\mathcal{A}\cdot\mathcal{C}$

$\:$

### Transponovanje
**Def**. **Transponovanje matrice** je funkcija $\ ^{\mathrm{T}}:\ \mathbb{M}_{mn}(\mathbb{F})\to\mathbb{M}_{nm}(\mathbb{F})$, takva da $\forall \mathcal{A}=(a_{ij})\in\mathbb{M}_{mn}(\mathbb{F})\quad\exists \mathcal{A}^{\mathrm{T}}=(a_{ji})\in\mathbb{M}_{nm}(\mathbb{F})$

Stav (svojstva transponovanja). 
- $\forall\mathcal{A},\,\mathcal{B}\in\mathbb{M}_{mn}(\mathbb{F})\quad(\mathcal{A}+\mathcal{B})^{\mathrm{T}}=\mathcal{A}^{\mathrm{T}}+\mathcal{B}^{\mathrm{T}}$
- $\forall\mathcal{A}\in\mathbb{M}_{mn}(\mathbb{F})\quad\forall\lambda\in\mathbb{F}\quad(\lambda\,\mathcal{A})^{\mathrm{T}}=\lambda\,\mathcal{A}^{\mathrm{T}}$
- $\forall\mathcal{A}\in\mathbb{M}_{mn}(\mathbb{F})\quad\forall\mathcal{B}\in\mathbb{M}_{nk}(\mathbb{F})\quad(\mathcal{A}\cdot\mathcal{B})^{\mathrm{T}}=\mathcal{B}^{\mathrm{T}}\cdot\mathcal{A}^{\mathrm{T}}$

> Dokaz poslednjeg tvrđenja:
> $\Big(\big(\mathcal{A}\cdot\mathcal{B}\big)^{\mathrm{T}}  \Big)^{i}_{j}=\big(\mathcal{A}\cdot\mathcal{B} \big) ^{j}_{i}=\sum\limits_{l=1}^{n}\big( \mathcal{A}\big)^{j}_{l}\big(\mathcal{B}\big)^{l}_{i} = \sum\limits_{l=1}^{n}\big(\mathcal{B}^{\mathrm{T}}\big)^{i}_{l}\big( \mathcal{A}^{\mathrm{T}}\big)^{l}_{j}=$
> $=\Big(\mathcal{B}^{\mathrm{T}}\cdot\mathcal{A}^{\mathrm{T}}\Big)^{i}_{j}$

$\:$
### [[Kvadratna matrica]]
- ### [[Determinanta]]
- ### [[Inverzna matrica]]
