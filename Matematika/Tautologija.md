#fax #math #ds1 [deo [[Iskazna logika|iskazne logike]]]
$\:$

 **Def**. Formula $A$ je **tautologija** ako važi $v(A) = 1$ za svaku valuaciju $v$.
 Važne tautologije: [[Ekvivalentne formule]]
> Primer 1:  Pomoću istinosne tablice dokazati da je formula $A = (p \land q) \land r \Rightarrow p \land (q \land r)$ tautologija.
Rešenje: 

|  p  |  q  |  r  | $p \land q$ | $q \land r$ | $(p \land q) \land r$ | $p \land (q \land r)$ | $A$ |
| :-: | :-: | :-: | :--------: | :-------: | :-----------------: | :----------------: | :-: |
|  0  |  0  |  0  |      0     |     0     |          0          |          0         |  1  |
|  0  |  0  |  1  |      0     |     0     |          0          |          0         |  1  |
|  0  |  1  |  0  |      0     |     0     |          0          |          0         |  1  |
|  0  |  1  |  1  |      0     |     1     |          0          |          0         |  1  |
|  1  |  0  |  0  |      0     |     0     |          0          |          0         |  1  |
|  1  |  0  |  1  |      0     |     0     |          0          |          0         |  1  |
|  1  |  1  |  0  |      1     |     0     |          0          |          0         |  1  |
|  1  |  1  |  1  |      1     |     1     |          1          |          1         |  1  |


> Primer 2:  Metodom svođenja na apsurd dokazati da je formula $A = (p \Rightarrow (q \Rightarrow r)) \Rightarrow (p \Rightarrow q) \Rightarrow (p \Rightarrow r)$ tautologija.
Rešenje: 
![[tautologija primer 2.png]]

> Primer 3:  Pomoću diskusije po iskaznom slovu dokazati da je formula $A = (p \Rightarrow (q \lor r)) \Rightarrow (p \Rightarrow q) \Rightarrow (p \Rightarrow r)$ tautologija.
Rešenje: 
![[tautologija primer 3.png]]