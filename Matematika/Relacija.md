#fax #math #ds1[deo [[Matematika|matematike]]]
$\:$

**Def**. Neka su $A$ i $B$ skupovi.
**Relacija** $\rho$ sa skupa $A$ u skup $B$ je bilo koji podskup [dekartovog proizvoda](Dekartov%20proizvod) $A \times B$. $\quad\rho \subseteq A \times B$
Piše se $\: (x, \  y) \in \rho \:\:$ ili $\:\: x \ \rho \ y \:\:$ za $\:\: x \in A \:\:$ i $\:\: y \in B$
Relacija između tri i više skupova se definiše slično.

**Def**.
- **Domen** relacije $\rho$ je $Dom(\rho)=\{a\in A\ | \ \exists b \in B \ : \ (a, \ b)\in \rho\}$
- **Slika** relacije $\rho$ je $Im(\rho)=\{b\in B\ | \ \exists a \in A \ : \ (a, \ b)\in \rho\}$
- **Inverzna relacija** relacije $\rho$ je relacija $\rho^{-1} = \{(b, \ a)\in B \times A \ | \ (a, \ b) \in \rho\}$

[Primer](relacija%20primer%201.png)

Osobine inverzne relacije ([dokaz](inverzna%20relacija%20svojstva.png)): $\rho,\ \sigma \in A \times B$, tada važi
1. $\rho \subseteq \sigma \quad \Rightarrow \quad \rho^{-1} \subseteq \sigma^{-1}$
2. $(\rho^{-1})^{-1} = \rho$
3. $(\sigma \cup \rho)^{-1} = \sigma^{-1} \cup \rho^{-1}$
4. $(\sigma \cap \rho)^{-1} = \sigma^{-1} \cap \rho^{-1}$

### Kompozicija relacija

**Def**. Neka su $\:\rho\subseteq A \times B\:$ i $\ \sigma\subseteq B \times C\:$ relacije.
**Kompozicija relacija** $\rho$ i $\sigma$ je relacija $\sigma\! \circ \! \rho = \{ (a,\ c) \in A \times C\ | \ \exists b \in B \ : \ (a, \ b) \in \rho \:$ i $\: (b, \ c) \in \sigma\}$
[Primer](kompozicija%20relacija%20primer.png)

Osobine kompozicije relacija ([dokaz](kompozicija%20relacija%20svojstva.png)):
$\rho\subseteq A \times B\,$, $\ \sigma\subseteq B \times C\,$, $\ \tau \subseteq C \times D$
1. $\tau\!\circ\!(\sigma\!\circ\!\rho) = (\tau\!\circ\!\sigma)\!\circ\!\rho$
2. $(\sigma\!\circ\!\rho)^{-1} = \rho^{-1}\!\circ\,\sigma^{-1}$


### Binarna relacija
**Def**. Binarna relacija je relacija sa skupa $A$ u isti skup $A$:$\:$ $\rho \subseteq A \times A$

**Def**. Binarna relacija je
- **refleksivna** (R) ako $\ \forall a \in A \quad (a, \ a)\in \rho$
- **antirefleksivna** (AR) ako $\ \forall a \in A \quad (a, \ a)\notin \rho$
- **simetrična** (S) ako $\ \forall a, \ b \in A \quad (a, \ b)\in \rho \ \ \ \Rightarrow \ \ \ (b, \ a) \in \rho$
- **antisimetrična** (AS) ako 
$\ \forall a, \ b \in A \quad (a, \ b)\in \rho \:$ i $\: (b, \ a) \in \rho \ \ \ \Rightarrow \ \ \ a = b$
- **tranzitivna** (T) ako 
$\ \forall a, \ b, \ c \in A \quad (a, \ b)\in \rho \:$ i $\: (b, \ c) \in \rho \ \ \ \Rightarrow \ \ \ (a, \ c)\in \rho$

[Primer](binarna%20relacija%20primer.png)

**Def**. Dijagonala $\triangle_A = \{ (a, \ a) \ | \  a \in A\} \subset A \times A$
- (R)$\quad \Leftrightarrow \quad \triangle_A \in \rho$
- (AR)$\quad \Leftrightarrow \quad \triangle_A \cap \rho = \varnothing$
- (S)$\quad \Leftrightarrow \quad \rho^{-1} \subseteq \rho$
- (AS)$\quad \Leftrightarrow \quad \rho^{-1} \cap \rho \subseteq \triangle_A$
- (T)$\quad \Leftrightarrow \quad \rho \! \circ \! \rho \subseteq \rho$

**Def**. Binarna relacija je relacija [**ekvivalencije**](Relacija%20ekvivalencije.md) ako je (R), (S) i (T)
**Def**. Binarna relacija je relacija **strogog** (parcijalnog) [**poretka**](Relacija%20poretka.md) ako je (AR), (S) i (T)
**Def**. Binarna relacija je relacija **nestrogog** (parcijalnog) [**poretka**](Relacija%20poretka.md) ako je (R), (S) i (T)

### [[Matrica relacije]] 
### [[Funkcija]]