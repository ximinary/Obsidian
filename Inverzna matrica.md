#fax #math #laag [deo poglavlja [[Matrica|"matrica"]]]
$\:$

**Def**. **Inverzna matrica** (inverz) matrici $\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})$ je matrica $\mathcal{A}^{-1}\in\mathbb{M}_{n}(\mathbb{F})$ ako važi $\mathcal{A}\cdot \mathcal{A}^{-1}=\mathbb{I}_{n}=\mathcal{A}^{-1}\cdot\mathcal{A}$

Tada su $\mathcal{A}$ i $\mathcal{A}^{-1}$ **invertibilni**/**regularni**.

Teorema (svojstva invertibilnih matrica).
- $\big(\mathcal{A}^{-1}\big)^{-1}=\mathcal{A}$
- $\big(\mathcal{A}^{\mathrm{T}}\big)^{-1}=\big(\mathcal{A}^{-1}\big)^{\mathrm{T}}$
- $\big(\mathcal{A}\cdot\mathcal{B}\big)^{-1}=\mathcal{B}^{-1}\cdot\mathcal{A}^{-1}$
- $\big(\lambda\,\mathcal{A}\big)^{-1}=\lambda^{-1}\,\mathcal{A}^{-1}$
- $\begin{align}\det\mathcal{A}^{-1}=\frac{1}{\det\mathcal{A}}\end{align}$ $\:$ (Posledica [[Determinanta#^47b633|Bine-Košijeve teoreme]])

Teorema. $\mathcal{A}\in \mathbb{M}_{n}(\mathbb{F})$.
$\mathcal{A}$ je invertibilna $\quad\Leftrightarrow\quad \det \mathcal{A}\ne 0$
### Traženje pomoću elementarnih transformacija
Elementarne transformacije: [[Rang matrice. Elementarne transformacije#^4c59da|(el1)]], [[Rang matrice. Elementarne transformacije#^ce1e01|(el2)]], [[Rang matrice. Elementarne transformacije#^e52b75|(el3)]].

$\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})$ — invertibilna
Primenimo elementarne transformacije $\mathrm{E}_{1},\,\mathrm{E}_{2},\,\dots,\,\mathrm{E}_{k}$ samo nad vrstama tako da $\underbrace{\mathrm{E}_{k}\cdot\!\cdot\!\cdot\mathrm{E}_{2}\,\mathrm{E}_{1}}_{\mathbf{E}}\,\mathcal{A}=\mathbb{I}_{n}$ $\ \ \:\Rightarrow\ \ \:$  $\mathcal{A}^{-1}=\mathbf{E}=\underbrace{\mathrm{E}_{k}\cdot\!\cdot\!\cdot\mathrm{E}_{2}\,\mathrm{E}_{1}}_{\mathbf{E}}\,\mathbb{I}_{n}$
tj $\mathcal{A}^{-1}$ dobijamo primenom istih transformacija na $\mathbb{I}_{n}$.

Odakle važi: $\boxed{\Big(\ \mathcal{A}\ \,\Big|\,\ \mathbb{I}_{n\ }\Big)\overset{\text{elementarne transformacije}}{\overset{\text{samo nad vrstama}}{\sim}}\Big(\ \,\mathbb{I}_{n\ }\ \Big|\ \mathcal{A}^{-1}\ \Big)}$
$\:$

Primedba: ako $\mathcal{A}$ nije invertibilna dobićemo $\mathbb{D}^{r}_{n\times n}$ umesto $\mathbb{I}_{n}$

### [[Determinanta#Laplasov razvoj|Traženje pomoću adjungovane matrice]]

$\begin{align}\mathcal{A}^{-1}=\frac{1}{\det \mathcal{A}}\,\mathrm{adj}\,\mathcal{A} \end{align}$
### Traženje pomoću minimalnog polinoma