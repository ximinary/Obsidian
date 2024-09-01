#fax #math #ds1 [deo [[Relacija|poglavlja "relacija"]]]
$\:$

**Def**. $A = \{a_1,\ a_2,\ ...,\ a_n\}$, $B = \{b_1,\ b_2,\ ...,\ b_m\}$ su konačni skupovi, $\rho \subseteq A \times B$
**Matrica relacije** $\rho$ (oznaka $M_{\rho}\,$) je matrica sa komponentima $m_{ij} = \begin{cases} 1, \ \ (a_i,\ b_j) \in \rho \\ 0, \ \ (a_i,\ b_j) \notin \rho \end{cases}$
$M_{\rho} \in \mathbb{M}(\{ 0,\ 1\})$

[Primer](matrica%20relacije%20primer.png)

**Def**. Bulov proizvod matrica $R \in \mathbb{M}_{m\times n}(\{ 0,\ 1\})\:$ i $\: S \in \mathbb{M}_{n\times k}(\{ 0,\ 1\})$ je matrica $\: T \in \mathbb{M}_{m\times k}(\{ 0,\ 1\})$ ako važi $t_{ij} = (r_{i1}\land s_{1j}) \lor (r_{i2}\land s_{2j}) \ \lor \, ... \,\! \lor \ (r_{in}\land s_{nj})$,
gde su $\quad \land,\ \lor :\quad \{ 0,\ 1\}\times\{ 0,\ 1\}\to\{ 0,\ 1\}$
definisani slično kao [logičke konjunkcija i disjunkcija](Logi%C4%8Dke%20operacije).
Oznaka: $T = R \otimes S$

[Primer](bulov%20proizvod%20primer.png)

[Teorema](matrica%20relacije%20teorema.png). $M_{\rho} \otimes M_{\sigma} = M_{\sigma \ \circ \ \rho}$

Matrica binarne relacije $\rho$ je kvadratna i važi:
- (R) $\:\Leftrightarrow\:$ matrica ima samo jedinici na glavnoj dijagonali
- (AR) $\:\Leftrightarrow\:$ matrica ima samo nule na glavoj dijagonali
- (S)  $\:\Leftrightarrow\:$  matrica je simetrična u odnosu na glavnu dijagonalu
- (AS)  $\:\Leftrightarrow\:$ za $i\ne j$, $m_{ij}$ i $m_{ij}$ ne mogu oba biti 1 ($m_{ij} \land m_{ij} = 0$)
- (T)   $\:\Leftrightarrow\:$ za svako $i$ i $j$ ako je jedinica na mestu $ij$ u matrici $M_{\rho} \otimes M_{\rho}$, tada je jedinica na mesu $ij$ u matrici $M_{\rho}\,$.