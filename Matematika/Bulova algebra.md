#fax #math #ds1 [deo [[Logika|logike]]]
$\:$

$B \ne \varnothing\quad$ — neki skup
$\mathbb{0}, \mathbb{1} \in B\quad$ — istaknuti elementi

Definisani su fje na skupu $B$:
$': \quad B \to B\quad$ — unarna operacija - bulovski komplement. 
$\qquad x \mapsto x'$
$\land: \quad B \times B\to B\quad$ — binarna operacija - bulovska konjunkcija. 
$\qquad (x, y) \mapsto x \land y$
$\lor: \quad B \times B\to B\quad$ — binarna operacija - bulovska disjunkcija. 
$\qquad (x, y) \mapsto x \lor y$

Tada algebarska struktura $(B, \: \lor, \: \land, \: ', \: \mathbb{0}, \: \mathbb{1})$ zove se **bulovom algebrom** ako $\forall x,\,y,\,z \in B$ važi:
1. $x \lor y = y \lor x \qquad$ — komutativnost
$x \land y = y \land x \qquad$ 
2. $x \lor (y \land z) = (x \lor y) \land (x \lor z) \qquad$ — distrivutivnost
$x \land (y \lor z) = (x \land y) \lor (x \land z) \qquad$
3. $x \lor \mathbb{0} = x \qquad$ — neutral
$x \land \mathbb{1} = x \qquad$
4. $x \lor x' = \mathbb{1} \qquad$ — komplementarnost
$x \land x' = \mathbb{0} \qquad$
5. $\mathbb{0} \ne \mathbb{1} \qquad$ — nedegenerisanost

Is aksioma 1.-5. izvode se sledeći zakoni ([[dokazi zakona bulovih algebri.png|dokazi]]):

6. $\mathbb{0}' = \mathbb{1}$
$\mathbb{1}' = \mathbb{0}$
7. $x \lor x = x \qquad$ — zakon idempotencije
$x \land x = x \qquad$
8. $x \land \mathbb{0} = \mathbb{0}$
 $x \lor \mathbb{1} = \mathbb{1}$
9. $x \lor (x \land y) = x \qquad$ — zakon apsorpcije
$x \land (x \lor y) = x \qquad$
10. $x \lor (y \lor z) = (x \lor y) \lor z \qquad$ — zakon asocijativnosti
$x \land (y \land z) = (x \land y) \land z \qquad$
11. $(x \lor y)' = x' \land y' \qquad$ — De Morganovi zakoni
$(x \land y)' = x' \lor y' \qquad$
12. Ako $x \lor y = 1$ i $x \land y = \mathbb{0}$, tada je $y = x'\qquad$ — jedinstvenost komplementa

### [[Relacija poretka]] na bulovoj algebri
$x \leqslant y \quad$ akko $\quad x \land y = x$

(R) $\quad x \land x = x\quad \Rightarrow \quad x \leqslant x$ 
(AS) $\quad x \leqslant y \quad\quad$ i $\quad\quad y \leqslant x$
$\quad\quad\quad x \land y = x \quad\quad\quad  y \land x = y\quad$
$\quad\quad\quad\quad\quad\quad\quad  x = y$
(T) $\quad x \leqslant y \quad\quad$ i $\quad\quad y \leqslant z$
$\quad(1)\: x \land y = x \quad\quad (2) \:  y \land z = y\quad$

$\quad\quad x  \stackrel{(1)}{=} x \land y \stackrel{(2)}{=} x \land y \land z \stackrel{(1)}{=} x \land z \quad \Rightarrow \quad x \leqslant z$ 

[[stav. relacija poretka u bulovim algebrama.png|Stav]]

### Princip dualnosti
$\Phi(B, \: \lor, \: \land, \: ', \: \mathbb{0}, \: \mathbb{1})$ - iskaz u bulovoj algebri $B$.
Tada je $\Phi(B, \: \lor, \: \land, \: ', \: \mathbb{0}, \: \mathbb{1})$ tačno akko je $\Phi(B, \: \land, \: \lor, \: ', \: \mathbb{1}, \: \mathbb{0})$ tačno.
$\Phi(B, \: \land, \: \lor, \: ', \: \mathbb{1}, \: \mathbb{0})$ je **dualan** prvom iskazu.
### Primeri bulovih algebri
1. Algebra [[Iskazna logika|iskazne logike]]: $B = \{0,1 \}$,  $\lor$, $\land$, $\neg$
Bulova algebra — $(\{0, 1\},\lor,\land,\neg,0,1)$
2. Algebra [[Karakteristična funkcija|karakterističnih funkcija]] na skupu $X$:
$X \ne \varnothing$
$B = \{ \chi_{A} \:|\: A \subseteq X\}$
$\chi_{A} \lor \chi_{B} := \chi_{A \cup B}$
$\chi_{A} \land \chi_{B} := \chi_{A \cap B}$
$\chi_{A}\,' := \chi_{X \setminus A}$
$1 := \chi_{\varnothing}$
$0 := \chi_{X}$
Bulova algebra — $(B,\lor,\land,',\chi_{\varnothing},\chi_{X})$

[[primeri bulovih algebri.png|Drugi primeri bulovih algebri]]

