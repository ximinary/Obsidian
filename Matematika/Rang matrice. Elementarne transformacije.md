#fax #math #laag [deo poglavlja [[Matrica|"matrica"]]]

### Rang matrice
Napomena: [[Matrica linearnog operatora|matrica linearnog operatora]]

Pojam ranga matrice se prenosi sa [[Slika i jezgro, rang i defekt linearnog operatora. Regularni operator|linearnih operatora]], pomoću izomorfizma $\varphi_{e,\,f}\:$:
$e=(e_{1},\,e_{2},\,\dots,\,e_{n})$ je baza $U$, $f=(f_{̌1},\,f_{2},\,\dots,\,f_{m})$ je baza $V$,
$A\in\mathrm{Hom}(U,\,V),\quad\mathcal{A}\in\mathbb{M}_{mn}(\mathbb{F})\ \ :\ \ \varphi_{e,\,f}(A)=\mathcal{A}$

$g_{1}=A(e_{1}),\ \ g_{2}=A(e_{2}),\ \ \dots, \ \ g_{m}=A(e_{m})$ 
$\{g_{1},\,g_{2},\,\dots,\,g_{m}\}$ je skup generatora od $\mathrm{Im}\,A$.
$\kappa_{f}(g_{1}),\,\kappa_{f}(g_{2}),\,\dots,\,\kappa_{f}(g_{m})$ — kolone $\mathcal{A}$.

$\mathrm{rang}\,A=\dim(\mathrm{Im}\,A)$, tj. broj linearno nezavisnih od $g_{1},\,g_{2},\,\dots,\,g_{m}$.
$\mathrm{rang}\,\mathcal{A}$ je broj linearno nezavisnih kolona $\mathcal{A}$.

$\mathrm{rang}\,A=\mathrm{rang}\,\mathcal{A}$

**Def**. Kanonska matrica ranga $r$ tipa $m\times n$ je matrica:

$\mathbb{D}^{r}_{m\times n}=\left(\begin{array}{c c c c c | c c c c}1&0&\dots&0&0&0&\dots&0\\0&1&\dots&0&0&0&\dots&0\\\dots&\dots&\dots&\dots&\dots&\dots&\dots&\dots\\0&0&\dots&1&0&0&\dots&0\\0&0&\dots&0&1&0&\dots&0\\\hline0&0&\dots&0&0&0&\dots&0\\\dots&\dots&\dots&\dots&\dots&\dots&\dots&\dots\\0&0&\dots&0&0&0&\dots&0\end{array}\right)=\left(\begin{array}{c|c}\mathbb{I}_{r}&\mathcal{O}_{r\times(n-r)}\\\hline \mathcal{O}_{(m-r)\times r}&\mathcal{O}_{(m-r)\times(n-r)}\end{array}\right)$

$\mathrm{rang}\,\mathbb{D}^{r}_{m\times n}=r$

Teorema ([[Slika i jezgro, rang i defekt linearnog operatora. Regularni operator#^6367f1|analogna za LO]]). $\mathcal{A},\,\mathcal{B}\in\mathbb{M}_{mn}(\mathbb{F})$.
1. $\mathcal{A}\sim\mathcal{B}\ \ \begin{align}&\Leftrightarrow\ \ \mathrm{rang}\,\mathcal{A}=\mathrm{rang}\,\mathcal{B}\\&\Leftrightarrow\ \ \exists\mathcal{S}\in\mathbb{M}_{m},(\mathbb{F}),\ \mathcal{T}\in\mathbb{M}_{n}(\mathbb{F})\text{ — invertibilni}\ \ :\ \ \mathcal{A}=\mathcal{S}\cdot\mathcal{B}\cdot\mathcal{T}\end{align}$ ^4f9e63
2. $\sim$ je relacija ekvivalencije na $\mathbb{M}_{mn}(\mathbb{F})$
### Elementarne transformacije
**Def**. Elementarne transformacije su:
- (el1) Množenje vrste (kolone) sa skalarom ^4c59da
- (el2) Zamena mesta dve vrste (kolone) ^ce1e01
- (el3) Dodavanje $j$-te vrste (kolone) $i$-toj vrsti (koloni). ^e52b75

$\mathbb{E}_{ij}= \left(\begin{array}{}0&\dots&0&\overset{j\text{-ta}}{\overset{\text{kolona}}{0}}&0&\dots&0\\\dots&\dots&\dots&\dots&\dots&\dots&\dots\\0&\dots&0&0&0&\dots&0\\0&\dots&0&1&0&\dots&0\\0&\dots&0&0&0&\dots&0\\\dots&\dots&\dots&\dots&\dots&\dots&\dots\\0&\dots&0&\underset{}{\underset{}{0}}&0&\dots&0\end{array}\right){}\small{i\text{-ta vrsta}}$

(el1):
>$\mathbb{F}_{i,\,\lambda}=\mathrm{diag}[1,\,\dots,\,1,\,\overset{i}{\lambda},\,1\,\dots,\,1]$
>
>$\mathbb{F}_{i,\,\lambda}\cdot\mathcal{A}$ — množi $i$-tu vrstu $\mathcal{A}$ sa $\lambda$
>$\mathcal{A}\cdot\mathbb{F}_{i,\,\lambda}$ — množi $i$-tu kolonu $\mathcal{A}$ sa $\lambda$
>
>$(\mathbb{F}_{i,\,\lambda})^{-1}=\mathbb{F}_{i,\,\frac{1}{\lambda}}$


(el2):
>$\mathbb{G}_{ij}=\mathbb{I}_{n}+\mathbb{E}_{ij}+\mathbb{E}_{ji}-\mathbb{E}_{ii}-\mathbb{E}_{jj}$
>
>$\mathbb{G}_{ij}\cdot\mathcal{A}$ — menja $i$-tu i $j$-tu vrstu $\mathcal{A}$ mestima
>$\mathcal{A}\cdot\mathbb{G}_{ij}$ — menja $i$-tu i $j$-tu kolonu $\mathcal{A}$ mestima
>
>$(\mathbb{G}_{ij})^{2}=\mathbb{I}_{n}\quad \Rightarrow\quad (\mathbb{G}_{ij})^{-1}=\mathbb{G}_{ij}$

(el3):
>$\mathbb{E}'_{ij}=\mathbb{I}_{n}+\mathbb{E}_{ij}$ ,$\ \:$ $i\ne j$
>
>$\mathbb{E}'_{ij}\cdot\mathcal{A}$ — doda $j$-tu vrstu $i$-toj vrsti $\mathcal{A}$
>$\mathcal{A}\cdot\mathbb{E}'_{ij}$ — doda $j$-tu kolonu $i$-toj koloni $\mathcal{A}$
>
>$(\mathbb{E}'_{ij})^{-1}=\mathbb{I}_{n}-\mathbb{E}_{ij}$

Stav. Elementarne transformacije ne menjaju rang matrice. (Posledica iz prethodne teoreme)
 
Stav. $\mathcal{A}\in\mathbb{M}_{mn}(\mathbb{F})$. Postoji konačan broj elementarnih transformacija $\mathrm{E}_{1},\,\mathrm{E}_{2},\,\dots,\,\mathrm{E}_{k}$ i $\overline{\rm E}_{1},\,\overline{\rm E}_{2},\,\dots,\,\overline{\rm E}_{k'}$ tako da $\mathrm{E}_{k}\cdot\!\cdot\!\cdot\mathrm{E}_{2}\,\mathrm{E}_{1}\,\mathcal{A}\,\overline{\rm E}_{1}\,\overline{\rm E}_{2}\cdot\!\cdot\!\cdot\overline{\rm E}_{k'}=\mathbb{D}^{r}_{m\times n}\:$. Odakle $\mathrm{rang}\, \mathcal{A}=r$

Specijalno: ako je $\mathcal{A}$ invertibilna, primenom konačnog broja elementarnih transformacija samo nad vrstama (kolonama) može da se dobija $\mathbb{I}_{n}$.
$\:$

[[Inverzna matrica#Traženje pomoću elementarnih transformacija|Traženje inverzne matrice pomoću elementarnih transformacija]].
