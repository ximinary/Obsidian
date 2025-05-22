#fax #math #alg #laag [deo [[Grupa|poglavlja "grupa"]]]
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

**Def**. Permutacija, u kojoj $a_{1}\mapsto a_{2}\mapsto\dots\mapsto a_{k-1}\mapsto a_{k}\mapsto a_{1}$, gde su svi $a_{i}$ različiti, a svi ostali $a_{i}, \ i>k$ se slikaju sami u sebe, zovemo **ciklus** dužine $k$, a skup $\{a_{1},\,a_{2},\,\dots,\,a_{k}\}$ je **nosač** tog ciklusa.
Oznaka: $(a_{1}\,a_{2}\,\cdots\,a_{k})$

**Stav**. [[Grupa#Red grupe i elementa|Red]] ciklusa dužine $k$ je $k$.

**Def**. Ciklus dužine dva zove se **transpozicija**.

**Def**. Ciklusi su **disjunktni** ako su njima nosači disjunktni.

**Stav**. Ako su svi $a_{1},\,a_{2},\,\dots,\,a_{k},\,a_{k+1},\,\dots,\,a_{m}$ različiti onda
$(a_{1}\ a_{2}\ \cdots\ a_{k})(a_{k}\ a_{k+1}\ \cdots\ a_{m})=(a_{1}\ a_{2}\ \cdots\ a_{k}\ a_{k+1}\ \cdots\ a_{m})$

**Teorema**. Svaka permutacija iz $\mathbb{S}_{n}$ može se predstaviti na jedinstven način (do na redosled) kao kombinacija disjunktnih ciklusa.

**Stav**. Svaka permutacija iz $\mathbb{S}_{n}$ može se predstaviti kao kombinacija transpozicija. ^76ab79

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

> Ciklus dužine $k$ je parna/neparna permutacija ako je $k$ neparan/paran broj.

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

$\:$
### Svojstva $\mathbb{S}_{n}$ i $\mathbb{A}_{n}$
**Stav**. Grupa $\mathbb{S}_{n}$ je generisana:
1. transpozicijama $(1\,2),\ (1\,3),\ \dots,\ (1\,n)$
2. transpozicijama $(1\,2),\ (2\,3),\ \dots,\ (n-1\,n)$
3. permutacijama $(1\,2)$ i $(1\,2\,3\,\cdots\,n)$
   
> Dokaz:
> 1. Pokažemo da $(a\, b)=(1\,a)(1\,b)(1\,a)$
>    $1\mapsto a\mapsto a \mapsto 1$
>    $a\mapsto 1\mapsto b \mapsto b$
>    $b\mapsto b\mapsto 1 \mapsto a$
>    Tako možemo dobiti svaku transpoziciju, a iz [[Grupa permutacija#^76ab79|stava]] svaku permutaciju je moguće predstaviti kao kombinaciju transpozicija.
>   2. Treba pokazati da je moguće izraziti svaku od transpozicija iz $1.$ kao kombinaciju transpozicija iz $2.$ 
>    Indukcijom:
>    baza: $(1\ 2)$ već je izražena. 
>    hipoteza: neka je izražena $(1\ k)$.
>    korak: pokazati da možemo izraziti i $(1\ k\!+\!1)$.
>    $(1\ k\!+\!1)=(1\ k)(k\ \ k\!+\!1)(1\ k)$
>    $\quad$ $\ \ \ 1\ \ \ \mapsto\ \ \ k\ \ \ \mapsto k\!+\!1\, \mapsto k\!+\!1$
>    $\quad$ $\ \ \  k\ \ \ \mapsto \ \ \ 1\ \ \ \mapsto \ \ \ 1\ \ \ \,  \mapsto \ \ \ k$
>    $\quad$ $k\!+\!1\mapsto k\!+\!1\,\mapsto \ \ \ k\ \ \  \mapsto \ \ \ 1$
>    Svaku permutaciju možemo izraziti kao kombinaciju transpozicija iz $1.$, a svaku od njih možemo izraziti transpozicijama iz $2.$
>    3. Treba pokazati da je moguće izraziti svaku od transpozicija iz $2.$ kao kombinaciju $(1\ 2)$ i $(1\ 2\ 3\ \cdots\ n)$.
>    Indukcijom:
>    baza: $(1\ 2)$ već je izražena. 
>    hipoteza: neka je izražena $(k\!-\!1\ \ k)$.
>    korak: pokazati da možemo izraziti i $(k\ k\!+\!1)$.
>    $(k\ k\!+\!1)=(1\ 2\ 3\ \cdots\ n)(k\!-\!1\ k)(1\ 2\ 3\ \cdots\ n)^{n-1}$
>    $\quad$ $\cdots$
>    $\quad$ $k\!-\!1 \mapsto k\!-\!2\mapsto k\!-\!2\, \mapsto k\!-\!1$
>    $\quad$ $\ \ \  k\ \ \, \mapsto k\!-\!1 \mapsto \ \ \ k\ \ \  \mapsto k\!+\!1$
>    $\quad$ $k\!+\!1\mapsto\ \ \ k\ \ \,\mapsto k\!-\!1\,  \mapsto \ \ \ k$
>    $\quad$ $\cdots$
>    Izražavanje permutacije: kombinacija proizvoljnih transpozicija -> $1.$ -> $2.$ -> $3.$ 

$\:$
**Stav**. Za $n\geqslant3$ grupa $\mathbb{A}_{n}$ je generisana ciklusima dužine 3.
> Dokaz: $\mathbb{A}_{3}=\{\mathrm{id,\ (123), (132)}\}$ jeste generisan ciklusima dužine 3.
> Iz dela $1.$ prethodnog stava svaki element $\mathbb{S}_{n}$ možemo dobiti kombinacijom navedenih transpozicija.
> Jer $\mathbb{A}_{n}\leqslant\mathbb{S}_{n}$, svaki element $\mathbb{A}_{n}$ možemo razviti na paran broj transpozicija oblika $(1\ a)$.
> Primenom $(1\ a)(1\ b)=(a\ 1\ b)$ na svaki uzastopni par, dobijamo tvrđenje. 

$\:$
**[[Grupa#^5f96ab|Posledica]]**. Ako su $\sigma$ i $\tau$ disjunktni ciklusi iz $\mathbb{S}_{n}$, onda $\omega(\sigma\,\tau)=\mathrm{NZS}\Big(\omega(\sigma),\ \omega(\tau)\Big)$