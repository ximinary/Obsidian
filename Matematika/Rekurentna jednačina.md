#fax #math #ds2 [deo [[Kombinatorika|kombinatorike]]]
$\:$

Opšti oblik rekurentne jednačine $k$-tog reda:
$a_{n+k}=\Phi(n,\,a_{n},\,a_{n+1},\,\dots,\,a_{n+k-1})$

**Def**. 
- **Rešenje** rj je bilo koji niz $(a_{n})$, takav da
$\forall n\in\mathbb{N}_{0}$ članovi niza $a_{n},\,a_{n+1},\,\dots,\,a_{n+k}$ zadovoljavaju rj.
- **Opšte rešenje** $a_{n}=(n,\,c_{1},\,c_{2},\dots,\,c_{k}),\ \ \forall n\in \mathbb{N}_{0}$ obuhvata sva rešenja rj, tako da $\forall c_{1},\,c_{2},\,\dots,\,c_{n}\in \mathbb{F}\,(\mathbb{R})\quad a_{n}$ je rešenje.
- **Partikularno rešenje** je rešenje koje je određeno vrednostima prvih $k$ članova niza.

### Linearna rekurentna jednačina
Linearna rekurentna jednačina $k$-tog reda:
$f_{0}(n)\,a_{n} + f_{1}(n)\,a_{n+1}+\dots+f_{k}(n)\,a_{n+k}=f(n)$

Vrste:
- sa konstantnim koeficijentima ($f_{i}\equiv \mathrm{const}$)
- sa funkcionalnim koeficijentima
$\:$
- **homogena** ako $f(n)\equiv 0$; **nehomogena** inače
- **normalizovana** ako $f_{k}(n)\equiv1$

Stav. Opšte rešenje homogene linearne rj je linearna kombinacija svih nezavisnih rešenja.

Stav. Opšte rešenje nehomogene linearne rj je $a_{n}= h_{n}+p_{n}$, gde je $h_{n}$ opšte rešenje odgovarajuće homogene linearne rj, $p_{n}$ je neko partikularno rešenje nehomogene linearne rj.

### Rešavanje linearne rekurentne jednačine sa konstantnim koeficijentima

- HOMOGENA

$f_{0}\,a_{n}+f_{1}\,a_{n+1}+\dots+f_{k}\,a_{n+k}=0,\quad f_{i}\in \mathbb{R}$

1\) Tražimo opšte rešenje $a_{n}$:

Pravimo odgovarajuću karakterističnu jednačinu:
$f_{0}+f_{1}\,x+f_{2}\,x^{2}+\dots+f_{k}\,x^{k}=0$
koja ima nule $x_{1},\,x_{2},\,\dots,\,x_{k}$ između kojih može biti višestrukih.
Tada opšte rešenje $a_{n}$ je zbir članova, svakom od kojih odgovara jedna nula. Članovi su oblika $c_{i}\,n^{p-1}\,x_{i}^{n}$, gde je to $p$-to pojavljivanje nule $x_{i}$, idući redom po nulama i $c_{i}\in \mathbb{R}$

> Ako su sve nule karakteristične jednačine različite,
> opšte rešenje je $a_{n}=c_{1}\,x_{1}^{n}+c_{2}\,x_{2}^{n}+\dots+c_{k}x_{k}^{n}$
> 
> Ako $x_{1}=x_{2}=x_{3}$
> opšte rešenje je $a_{n}=c_{1}\,x_{1}^{n}+c_{2}\,n\,x_{1}^{n}+c_{3}\,n^{2}\,x_{1}^{n}+c_{4}\,x_{4}^{n}\dots+c_{k}x_{k}^{n}$

2\) Tražimo partikularno rešenje u zavisnosti od $k$ prvih članova niza (tj određujemo $c_{1},\,c_{2},\,\dots,\,c_{k}$) tako što ubacujemo redom $a_{1},\,a_{2},\,\dots,\,a_{k}$ u opšte rešenje i rešavamo dobijen sistem.

[[RJprimer1.png|Primer]]

- NEHOMOGENA

$f_{0}\,a_{n}+f_{1}\,a_{n+1}+\dots+f_{k}\,a_{n+k}=f(n),\quad f_{i}\in \mathbb{R}$

1\) Tražimo opšte rešenje odgovarajuće homogene $h_{n}$

2\) Tražimo partikularno rešenje nehomogene $p_{n}$:

Ako $f(n)=P_{d}(n)\cdot b^{n}$, gde je $P_{d}$ polinom stepena $d$ i  
$b\in \mathbb{R}$ je $m$-struka nula ($m:=0$ ako nije nula) karakteristične jednačine odgovarajuće homogene rj.
Tada $p_{n}=(A_{0}+A_{1}n+\dots+A_{d}n^{d})\cdot n^{m}\cdot b^{n}$, 
brojevi $A_{i}$ se dobijaju ubacivanjem $p_{n}$ u polaznu rj.

3\) Opšte rešenje $a_{n}=h_{n}+p_{n}$

4\) Tražimo partikularno rešenje u zavisnosti od $k$ prvih članova niza (tj određujemo $c_{1},\,c_{2},\,\dots,\,c_{k}$) tako što ubacujemo redom $a_{1},\,a_{2},\,\dots,\,a_{k}$ u opšte rešenje i rešavamo dobijen sistem.

[[RJprimer2.png|Primer]]

- Rešavanje homogene normalizovane pomoću [[Funkcija generatrisa|funkcija generatrisa]]

[[RJprimer3.png|Primer 1]]
[[RJprimer4.png|Primer 2]]