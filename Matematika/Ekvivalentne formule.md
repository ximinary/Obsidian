#fax #math #ds1 [deo [[Iskazna logika|iskazne logike]]]
$\:$

**Def**. Iskazne formule $A$ i $B$ su **logički ekvivalentne** ($A \equiv B$) ako za svaku valuaciju važi $v(A)=v(B)$ 
(tj. $A \Leftrightarrow B$ je [[tautologija]]).

Važni primeri:
1. $p \lor 0 \equiv p \qquad p \land 0 \equiv 0$
 $p \land 1 \equiv p \qquad p \lor 1 \equiv 1$
2. $p \lor p \equiv p \qquad$ — zakon idempotentnosti
$p \land p \equiv p$ 
3. $p \lor \neg p \equiv 1 \qquad$ — zakon isključenja trećeg
$p \land \neg p \equiv 0 \qquad$
4. $\neg (\neg p) \equiv p \qquad$ — zakon dvojne negacije
5. $p \lor (q \lor r) \equiv (p \lor q) \lor r \qquad$ — zakon asocijativnosti
$p \land (q \land r) \equiv (p \land q) \land r \qquad$
6. $p \lor q \equiv q \lor p \qquad$ — zakon komutativnosti
$p \land q \equiv q \land p \qquad$
7. $p \lor (q \land r) \equiv (p \lor q) \land (p \lor r) \qquad$ — zakon distrivutivnosti
$p \land (q \lor r) \equiv (p \land q) \lor (p \land r) \qquad$
8. $1 \Rightarrow p \equiv p$
$0 \Rightarrow p \equiv 1$
$p \Rightarrow 1 \equiv 1$
$p \Rightarrow 0 \equiv \neg p$
9. $\neg (p \lor q) \equiv \neg p \land \neg q\qquad$ — De Morganovi zakoni
$\neg (p \land q) \equiv \neg p \lor \neg q\qquad$
10. $p \lor (p \land q) \equiv p \qquad$ — zakon apsorpcije
$p \land (p \lor q) \equiv p \qquad$
11. $p \Rightarrow p \equiv p \equiv p \Leftrightarrow p \qquad$ — refleksivnost impl./ekviv.
12. $(p \Leftrightarrow q) \land (q \Leftrightarrow r) \equiv (p \Leftrightarrow r) \qquad$ — tranzitivnost ekviv.
13. $p \Rightarrow q \equiv \neg q \Rightarrow \neg p \qquad$ — kontrapozicija
14. $p \Rightarrow q \equiv \neg p \lor q \qquad$
15. $p \Leftrightarrow q \equiv (p \Rightarrow q) \land  (q \Rightarrow p)$
16. $p \underline{\vee} q \equiv \neg(p \Leftrightarrow q)$
17. $(p \lor q) \land (p \lor r)  \land (q \lor r) \equiv (p \land q) \lor (p \land r)\lor (q \land r)$

Važne tautologije ($\equiv 1$):

18. $(p \land (p \Rightarrow q)) \Rightarrow q\qquad$ — modus ponens
19. $(\neg p \Rightarrow 0) \Rightarrow p\qquad$ — svođenje na apsurd
20. $(p \land q) \Rightarrow p$
$p \Rightarrow (p \lor q)$