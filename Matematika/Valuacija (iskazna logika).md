#fax #math #ds1 [deo [[Iskazna logika|iskazne logike]]]
$\:$

**Def**. Valuacija je [funkcija](Funkcija.md) iz $\mathcal{P}$ u {0, 1}: $\quad v: \quad \mathcal{P} \to \{0, 1\}$
Preslikava svako [[Iskazna logika|iskazno]] slovo u 0 ili 1.

$v: \quad For \to \{0, 1\}$
Slično ista funkcija preslikava i svaku iskaznu formulu u 0 ili 1, pomoću sledećih jednakosti:
- $v(\neg A) = \neg v(A)$
- $v(A \lor B) = v(A) \lor v(B)$
- $v(A \land B) = v(A) \land v(B)$
- $v(A \Rightarrow B) = v(A) \Rightarrow v(B)$
- $v(A \Leftrightarrow B) = v(A) \Leftrightarrow v(B)$
- $v(A \underline{\vee} B) = v(A) \underline{\vee} v(B)$
- Ako je $c \in \{0, 1 \}$ konsranta tada $v(c)=c$

> Primer:
 Za datu valuaciju $v: v(p) = 0, v(q) = 1, v(r) = 0$ odrediti istinonosnuju vrednost formule $(p \lor q) \Rightarrow (p \lor r)$;
Rešenje:
$v((p \lor q) \Rightarrow (p \lor r)) = v(p \lor q) \Rightarrow v(p \lor r) =$
$= (v(p) \lor v(q)) \Rightarrow (v(p) \lor v(r)) =(0 \lor 1) \Rightarrow (0 \lor 0) =$
$= 1 \Rightarrow 0=0$