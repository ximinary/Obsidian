#fax #math #alg #laag [deo poglavlja [[Grupa|"grupa"]] i [[Determinanta|"determinanta"]]]
$\:$

**Def**. $S_{X}$ je skup svih [[Izbor elemenata#(5) Permutacije|permutacija]] skupa $X$, tj. skup svih bijekcija $\sigma:\ X\to X$.
Ako je $X=\{ 1,\,2,\,\dots,\,n \}$ označavamo sa $S_{n}$.

Ako je $\circ$ kompozicija funkcija, onda je $\mathbb{S}_{X}=(S_{X},\,\circ)$ [[Grupa|grupa]]:
- važi asocijativnost
- neutral je funkcija $\mathrm{id}$, takva da $\forall x\in X\ \ \ \mathrm{id}(x)=x$
- za svaku permutaciju $\sigma$, postoji obratna $\sigma^{-1}$

$\:$
**Stav**. Ako postoji bijekcija među skupovima $X$ i $Y$, onda $\mathbb{S}_{X}\cong \mathbb{S}_{Y}$

$\sigma\in S_{n},$ tada označavamo $\sigma=\left(\begin{array}{} 1&2&\dots&n\\\sigma(1)&\sigma(2)&\dots&\sigma(n)\end{array}\right)$

**Def**. Permutacija, u kojoj $a_{1}\mapsto a_{2}\mapsto\dots\mapsto a_{k-1}\mapsto a_{k}\mapsto a_{1}$, gde su svi $a_{i}$ različiti, a svi ostali $a_{i}, \ i>k$ se slikaju sami u sebe, zovemo **ciklus** dužine (odnosno [[Grupa#Red grupe i elementa|reda]]) $k$, a skup $\{a_{1},\,a_{2},\,\dots,\,a_{k}\}$ je **nosač** tog ciklusa.
Oznaka: $(a_{1}\,a_{2}\,\cdots\,a_{k})$

**Def**. Ciklus dužine dva zove se **transpozicija**.

**Def**. Ciklusi su **disjunktni** ako su njima nosači disjunktni.

**Stav**. Ako su svi $a_{1},\,a_{2},\,\dots,\,a_{k},\,a_{k+1},\,\dots,\,a_{m}$ različiti onda
$(a_{1}\ a_{2}\ \cdots\ a_{k})(a_{k}\ a_{k+1}\ \cdots\ a_{m})=(a_{1}\ a_{2}\ \cdots\ a_{k}\ a_{k+1}\ \cdots\ a_{m})$

**Teorema**. Svaka permutacija iz $\mathbb{S}_{n}$ može se predstaviti na jedinstven način (do na redosled) kao kombinacija disjunktnih ciklusa.

**Stav**. Svaka permutacija iz $\mathbb{S}_{n}$ može se predstaviti kao kombinacija transpozicija.

Primeri: 
- $(12)(23)=(123)\quad\quad(23)(12)=(132)$
- Permutaciju $\sigma=\left(\begin{array}{}1&2&3&4&5&6&7&8&9\\2&3&1&5&4&7&8&9&7\end{array}\right)$ predstavimo kao
— kombinaciju disjunktnih ciklusa: $\sigma =(123)(45)(6789)$ 
— kombinaciju transpozicija: $\sigma =(12)(23)(45)(67)(78)(89)$ 
- Svi predstavnici ciklusa dužine 4 u $\mathbb{S}_{4}$:
  $(1234)=(2341)=(3412)=(4123)$


### Parnost permutacije
**Def**. **Inverzija** permutacije je par $\:(i,\,j)\:$ za koji važi $\:i<j\:$ i $\:\sigma(i)>\sigma(j)$, $\ \:$ $\forall i,\,j=\overline{1,n}$

$I(\sigma)$ — broj inverzija permutacije.

$\sigma$ je parna permutacija ako je $I(\sigma)$ paran broj,
$\sigma$ je neparna permutacija ako je $I(\sigma)$ neparan broj.

**Stav**. Ako je permutacija predstavljena kombinacijom parnog/neparnog broja transpozicija, onda je ona parna/neparna.

$\:$
Skup svih parnih permutacija u $\mathbb{S}_{n}$ je grupa $\mathbb{A}_{n}$

**Stav**. $\begin{align}\forall n\geqslant2\quad \mathbb{A}_{n}\leqslant \mathbb{S}_{n}\ \ \text{i}\ \ |\mathbb{A}_{n}|=\frac{n!}{2}\end{align}$
> Dokaz:
> Skup parnih permutacija je podskup skupa permutacija.
> $\forall \sigma,\,\pi\in\mathbb{A}_{n}$ mogu biti predstavljeni kao kompozicija parnog broja transpozicija.
> Stoga i $\sigma\pi$ se predstavlja kompozicijom parnog broja transpozicija, tj. $\sigma\pi\in\mathbb{A}_{n}$.
> Imamo da je $\mathbb{A}_{n}$ [[Grupa#Podgrupa|podgrupa]] od $\mathbb{S}_{n}$.
> 
> Neka je $\tau$ proizvoljna transpozicija, definišemo funkciju $\Phi:\ \mathbb{A}_{n}\to \mathbb{S}_{n}\!\setminus\!\mathbb{A}_{n}$ $\ \:$ sa $\ \:$ $\Phi(\pi)=\tau\pi$, koja jeste bijekcija, tada $|\mathbb{A}_{n}|=|\mathbb{S}_{n}|-|\mathbb{S}_{n}\!\setminus\!\mathbb{A}_{n}|=|\mathbb{S}_{n}|-|\mathbb{A}_{n}|$
> Imamo da $\begin{align}|\mathbb{A}_{n}|=\frac{|\mathbb{S}_{n}|}{2}=\frac{n!}{2}\end{align}$