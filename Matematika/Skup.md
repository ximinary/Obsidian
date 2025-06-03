#fax #math #ds1 [deo [[Matematika|matematike]]]
$\:$

[Raselov paradoks](raselov%20paradoks.png)
### Aksiome teorije skupova
- Aksioma **egzistencije**:
Dva skupa su jednaki ako imaju iste elemente
- Aksioma **para**:
Za svaka dva skupa $X$ i $Y$ postoji skup $Z$ čiji su elemente $X$ i $Y$.
$Z=\{X,\:Y\}$
- Aksioma **praznog skupa**:
  Postoji jedinstven skup $\varnothing$ koji ne sadrži nijedan element. 
- Aksioma **unije**:
  Za svaki skup $X$ postoji skup $Z$ tako da je
  $u \in Z$ akko $u \in Y$ za neki $Y \in X\quad$  ($Z$ sadrži samo elementi nekog elemenata $X$)
- Aksioma **partitivnog skupa**:
  Za svaki skup $X$ postoji skup čiji su elementi svi podskupovi skupa $X$.
  $\mathcal{P}(X)$
  Ako $X$ sadrži n elemenata, onda $\mathcal{P}(X)$ sadrži $2^n$ elemenata.
  >Primeri:
  $X = \{a, b\}\quad$ tada $\quad \mathcal{P}(X) = \{\varnothing, \{a\}, \{b\}, \{a,b\}\}$
  $Y = \varnothing \quad$ tada $\quad \mathcal{P}(Y) = \{\varnothing\}$
  $Z = \{\varnothing\} \quad$ tada $\quad \mathcal{P}(Z) = \{\varnothing, \{\varnothing\} \}$
- Aksioma **razdvajanja**:
  Neka je $A$ neki skup i $\Phi$ je neko svojstvo,
  tada je $\{ x \in A \:|\: \Phi(x)\}$ skup.

### Operacije nad skupovima i njihova svojstva
**Def**.
Neka je $X$ univerzum ([skup](Skup.md) svih objekata i skupova), tada:
- Presek:
$\qquad A \cap B = \{x \in X\:|\:x \in A \ \ \land \ \ x \in B\}$
- Unija: 
$\qquad A \cup B = \{x \in X\:|\:x \in A \ \ \lor \ \ x \in B\}$
- Razlika: 
$\qquad A \setminus B = \{x \in X\:|\:x \in A \ \ \land \ \ x \notin B\}$
- Komplement: 
$\qquad A^C = \{x \in X\:|\: x \notin A\}$
- Simetrična razlika:
$\qquad A \, \triangle \, B = (A \setminus B) \cup (B \setminus A)$

**Stav** (svojstva).
1. $A \cap (B \cap C) = (A \cap B) \cap C \qquad$ — asocijativnost
$A \cup (B \cup C) = (A \cup B) \cup C \qquad$ 
$A \, \triangle \, (B \, \triangle \, C) = (A \, \triangle \, B) \, \triangle \, C \qquad$ 
2. $A \cap B = B \cap A \qquad$ — komutativnost
$A \cup B = B \cup A \qquad$
$A \, \triangle \, B = B \, \triangle \, A \qquad$
3. $A \cap (B \cup C) = (A \cap B) \cup (A \cap C) \qquad$ — distributivnost
$A \cup (B \cap C) = (A \cup B) \cap (A \cup C) \qquad$ 
4. $A \cap A = A \qquad$ — idempotentnost
$A \cup A = A \qquad$
5. $A \cap (A \cup B) = A \qquad$ — zakon apsorpcije
$A \cup (A \cap B) = A \qquad$ 
6. $(A^C)^C = A$
7. $(A \cap B)^C = A^C \cup B^C\qquad$ — De Morganovi zakoni
$(A \cup B)^C = A^C \cap B^C$
8. $A \setminus B = A \cap B^C$
9. $A \setminus (B \cap C) = (A \setminus B) \cup (A \setminus C)$
$A \setminus (B \cup C) = (A \setminus B) \cap (A \setminus C)$
10. $A \cap X = A \qquad A \cap \varnothing =  \varnothing$
$A \cup \varnothing =  A \qquad A \cup X =  X$

$\:$
[Relacije poretka](Relacija%20poretka.md):
- Podskup: $A \subseteq B\quad$ akko $\quad \forall x \in A \ \ \ x \in B$
- Pravi podskup: $A \subset B\quad$ akko $\quad A \subseteq B \ \ \land \ \  A \ne B$

[[skupovi primer 1.png|Primer 1]]
[[skupovi primer 2.png|Primer 2]]


[Stav](stav.%20jednakost%20skupova.png). $\{a,\ b\} = \{c, \ d\}\quad$ akko $\quad \begin{cases} a = c\\ b = d \end{cases}\quad$ ili$\quad \begin{cases} a = d\\ b = c \end{cases}$

**Def.** Uređeni par $\:(a,\ b)\:$ je $\:\{\{a\},\ \{a,\ b\}\}$
**Def.** Uređena trojka $\:(a,\ b,\ c)\:$ je $\:(a,\ (b,\ c))$
**Def.** Uređena $n$-torka se zada slično rekurentno. ^e21aa8

[Stav](stav.%20jednakost%20uredenih%20parova.png). $(a, \ b) = (c, \ d)\quad$ akko $\quad \begin{cases} a = c\\ b = d \end{cases}$

Stav. $(a_1,\: a_2,\:..., \: a_n) = (b_1,\: b_2,\:..., \: b_n)\quad$ akko $\quad \begin{cases} a_1 = b_1\\ a_1 = b_2 \\ ... \\ a_n = b_n\end{cases}$

### Dekartov proizvod
**Def**. Dekartov proizvod [[Skup|skupova]] $A$ i $B$:
$A \times B = \{ (a,\: b) \: | \: a \in A, \ b \in B \}$

Dekartov proizvod [[Skup|skupova]] $A$, $B$ i $C$:
$A \times B \times C= \{ (a,\: b,\: c) \: | \: a \in A, \ b \in B, \ c \in C \}$

Dekartov proizvod [[Skup|skupova]] $A_1$, $A_2$, $...$, $A_n$:
$A_1 \times A_2 \ \times \ ... \times \ A_n= \{ (a_1,\: a_2,\:..., \: a_n) \: | \: a_1 \in A_1, \ a_2 \in A_2, \ ..., \ a_n \in A_n \}$

$A^n = \underbrace{A \times A \ \times \ ... \times \ A}_{n}$

$\lvert A \times B \rvert = \lvert A \rvert \cdot \lvert  B \rvert$

Svojstva:
- $(A \cup B) \times C = (A \times C)\cup(B \times C)$
- $(A \cap B) \times C = (A \times C)\cap(B \times C)$
- $(A \, \setminus \, B) \times C = (A \times C)\setminus (B \times C)$
- $(A \times B) \cup (C \times D) \subseteq (A \cup C) \times (B \cup D)$
- $(A \times B) \cap (C \times D) = (A \cap C) \times (B \cap D)$
### [[Kardinalnost. Prebrojivost]]
