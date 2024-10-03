![[ds1_beleške-01.png]]
![[ds1_beleške-02.png]]
# 1 Teorija skupova

![[raselov paradoks.png]]
## 1.1 Aksiome teorije skupova
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
  Za svaki skup $X$ postoji skup čiji su elementi svi podskupovi skupa $X$. Partitivni skup skupa $X$ je $\mathcal{P}(X)$
  Ako $X$ sadrži n elemenata, onda $\mathcal{P}(X)$ sadrži $2^n$ elemenata.
  >Primeri:
  $X = \{a, b\}\quad$ tada $\quad \mathcal{P}(X) = \{\varnothing, \{a\}, \{b\}, \{a,b\}\}$
  $Y = \varnothing \quad$ tada $\quad \mathcal{P}(Y) = \{\varnothing\}$
  $Z = \{\varnothing\} \quad$ tada $\quad \mathcal{P}(Z) = \{\varnothing, \{\varnothing\} \}$
- Aksioma **razdvajanja**:
  Neka je $A$ neki skup i $\Phi$ je neko svojstvo,
  tada je $\{ x \in A \:|\: \Phi(x)\}$ skup.

## 1.2 Osnovno
**Def.** Operacije nad skupovima
Neka je $X$ univerzum (skup svih objekata i skupova), tada:
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

$\_\_\_\_\_\_\_\_$
- Podskup: $A \subseteq B\quad$ akko $\quad \forall x \in A \ \ \ x \in B$
- Pravi podskup: $A \subset B\quad$ akko $\quad A \subseteq B \ \ \land \ \  A \ne B$

Primeri zadataka:
![[skupovi primer 1.png]]
![[skupovi primer 2.png]]

Svojstva skupova:
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
7. $(A \cap B)^C = A^C \cup B^C \qquad$ — De Morganovi zakoni
$(A \cup B)^C = A^C \cap B^C$
8. $A \setminus B = A \cap B^C$
9. $A \setminus (B \cap C) = (A \setminus B) \cup (A \setminus C)$
$A \setminus (B \cup C) = (A \setminus B) \cap (A \setminus C)$
10. $A \cap X = A \qquad A \cap \varnothing =  \varnothing$
$A \cup \varnothing =  A \qquad A \cup X =  X$


Stav $\{a,\ b\} = \{c, \ d\}\quad$ akko $\quad \begin{cases} a = c\\ b = d \end{cases}\quad$ ili$\quad \begin{cases} a = d\\ b = c \end{cases}$
![[stav. jednakost skupova.png]]


**Def.** Uređeni par $\:(a,\ b)\:$ je $\:\{\{a\},\ \{a,\ b\}\}$
**Def.** Uređena trojka $\:(a,\ b,\ c)\:$ je $\:(a,\ (b,\ c))$
**Def.** Uređena $n$-torka se zada slično rekurentno.

Stav. $(a, \ b) = (c, \ d)\quad$ akko $\quad \begin{cases} a = c\\ b = d \end{cases}$
![[stav. jednakost uređenih parova.png]]
Stav. $(a_1,\: a_2,\:..., \: a_n) = (b_1,\: b_2,\:..., \: b_n)\quad$ akko $\quad \begin{cases} a_1 = b_1\\ a_1 = b_2 \\ ... \\ a_n = b_n\end{cases}$



## 1.3 Dekartov proizvod

**Def.** Dekartov proizvod skupova $A$ i $B$:
$A \times B = \{ (a,\: b) \: | \: a \in A, \ b \in B \}$

Dekartov proizvod skupova $A$, $B$ i $C$:
$A \times B \times C= \{ (a,\: b,\: c) \: | \: a \in A, \ b \in B, \ c \in C \}$

Dekartov proizvod skupova $A_1$, $A_2$, $...$, $A_n$:
$A_1 \times A_2 \ \times \ ... \times \ A_n= \{ (a_1,\: a_2,\:..., \: a_n) \: | \: a_1 \in A_1, \ a_2 \in A_2, \ ..., \ a_n \in A_n \}$

$A^n = \underbrace{A \times A \ \times \ ... \times \ A}_{n}$

$\lvert A \times B \rvert = \lvert A \rvert \cdot \lvert  B \rvert$

Svojstva:
- $(A \cup B) \times C = (A \times C)\cup(B \times C)$
- $(A \cap B) \times C = (A \times C)\cap(B \times C)$
- $(A \, \setminus \, B) \times C = (A \times C)\setminus (B \times C)$
- $(A \times B) \cup (C \times D) \subseteq (A \cup C) \times (B \cup D)$
- $(A \times B) \cap (C \times D) = (A \cap C) \times (B \cap D)$

# 2 Relacije
**Def**. Neka su $A$ i $B$ skupovi.
**Relacija** $\rho$ sa skupa $A$ u skup $B$ je bilo koji podskup dekartovog proizvoda $A \times B$. $\quad\rho \subseteq A \times B$
Piše se $\: (x, \  y) \in \rho \:\:$ ili $\:\: x \ \rho \ y \:\:$ za $\:\: x \in A \:\:$ i $\:\: y \in B$
Relacija između tri i više skupova se definiše slično.

**Def**.
- **Domen** relacije $\rho$ je $Dom(\rho)=\{a\in A\ | \ \exists b \in B \ : \ (a, \ b)\in \rho\}$
- **Slika** relacije $\rho$ je $Im(\rho)=\{b\in B\ | \ \exists a \in A \ : \ (a, \ b)\in \rho\}$
- **Inverzna relacija** relacije $\rho$ je relacija $\rho^{-1} = \{(b, \ a)\in B \times A \ | \ (a, \ b) \in \rho\}$

![[relacija primer 1.png]]

Osobine inverzne relacije: $\rho,\ \sigma \in A \times B$, tada važi
1. $\rho \subseteq \sigma \quad \Rightarrow \quad \rho^{-1} \subseteq \sigma^{-1}$
2. $(\rho^{-1})^{-1} = \rho$
3. $(\sigma \cup \rho)^{-1} = \sigma^{-1} \cup \rho^{-1}$
4. $(\sigma \cap \rho)^{-1} = \sigma^{-1} \cap \rho^{-1}$

![[inverzna relacija svojstva.png]]

**Def**. Neka su $\:\rho\subseteq A \times B\:$ i $\ \sigma\subseteq B \times C\:$ relacije.
**Kompozicija relacija** $\rho$ i $\sigma$ je relacija $\sigma\! \circ \! \rho = \{ (a,\ c) \in A \times C\ | \ \exists b \in B \ : \ (a, \ b) \in \rho \:$ i $\: (b, \ c) \in \sigma\}$

![[kompozicija relacija primer.png]]

Osobine kompozicije relacija:
$\rho\subseteq A \times B\,$, $\ \sigma\subseteq B \times C\,$, $\ \tau \subseteq C \times D$
1. $\tau\!\circ\!(\sigma\!\circ\!\rho) = (\tau\!\circ\!\sigma)\!\circ\!\rho$
2. $(\sigma\!\circ\!\rho)^{-1} = \rho^{-1}\!\circ\,\sigma^{-1}$

![[kompozicija relacija svojstva.png]]

## 2.1 Binarna relacija
**Def**. Binarna relacija je relacija sa skupa $A$ u isti skup $A$:$\:$ $\rho \subseteq A \times A$

**Def**. Binarna relacija je
- **refleksivna** (R) ako $\ \forall a \in A \quad (a, \ a)\in \rho$
- **antirefleksivna** (AR) ako $\ \forall a \in A \quad (a, \ a)\notin \rho$
- **simetrična** (S) ako $\ \forall a, \ b \in A \quad (a, \ b)\in \rho \ \ \ \Rightarrow \ \ \ (b, \ a) \in \rho$
- **antisimetrična** (AS) ako 
$\ \forall a, \ b \in A \quad (a, \ b)\in \rho \:$ i $\: (b, \ a) \in \rho \ \ \ \Rightarrow \ \ \ a = b$
- **tranzitivna** (T) ako 
$\ \forall a, \ b, \ c \in A \quad (a, \ b)\in \rho \:$ i $\: (b, \ c) \in \rho \ \ \ \Rightarrow \ \ \ (a, \ c)\in \rho$

![[binarna relacija primer.png]]
**Def**. Dijagonala $\triangle_A = \{ (a, \ a) \ | \  a \in A\} \subset A \times A$
- (R)$\quad \Leftrightarrow \quad \triangle_A \in \rho$
- (AR)$\quad \Leftrightarrow \quad \triangle_A \cap \rho = \varnothing$
- (S)$\quad \Leftrightarrow \quad \rho^{-1} \subseteq \rho$
- (AS)$\quad \Leftrightarrow \quad \rho^{-1} \cap \rho \subseteq \triangle_A$
- (T)$\quad \Leftrightarrow \quad \rho \! \circ \! \rho \subseteq \rho$

## 2.2 Matrica relacije
**Def**. $A = \{a_1,\ a_2,\ ...,\ a_n\}$, $B = \{b_1,\ b_2,\ ...,\ b_m\}$ su konačni skupovi, $\rho \subseteq A \times B$
**Matrica relacije** $\rho$ (oznaka $M_{\rho}\,$) je matrica sa komponentima $m_{ij} = \begin{cases} 1, \ \ (a_i,\ b_j) \in \rho \\ 0, \ \ (a_i,\ b_j) \notin \rho \end{cases}$
$M_{\rho} \in \mathbb{M}(\{ 0,\ 1\})$

![[matrica relacije primer.png]]

**Def**. Bulov proizvod matrica $R \in \mathbb{M}_{m\times n}(\{ 0,\ 1\})\:$ i $\: S \in \mathbb{M}_{n\times k}(\{ 0,\ 1\})$ je matrica $\: T \in \mathbb{M}_{m\times k}(\{ 0,\ 1\})$ ako važi $t_{ij} = (r_{i1}\land s_{1j}) \lor (r_{i2}\land s_{2j}) \ \lor \, ... \,\! \lor \ (r_{in}\land s_{nj})$,
gde su $\quad \land,\ \lor :\quad \{ 0,\ 1\}\times\{ 0,\ 1\}\to\{ 0,\ 1\}$
definisani slično kao logičke konjunkcija i disjunkcija.
Oznaka: $T = R \otimes S$

![[bulov proizvod primer.png]]

Teorema.
![[matrica relacije teorema.png]]

Matrica binarne relacije $\rho$ je kvadratna i važi:
- (R) $\:\Leftrightarrow\:$ matrica ima samo jedinici na glavnoj dijagonali
- (AR) $\:\Leftrightarrow\:$ matrica ima samo nule na glavnoj dijagonali
- (S)  $\:\Leftrightarrow\:$  matrica je simetrična u odnosu na glavnu dijagonalu
- (AS)  $\:\Leftrightarrow\:$ za $i\ne j$, $m_{ij}$ i $m_{ji}$ ne mogu oba biti 1 ($m_{ij} \land m_{ji} = 0$)
- (T)   $\:\Leftrightarrow\:$ za svako $i$ i $j$ ako je jedinica na mestu $ij$ u matrici $M_{\rho} \otimes M_{\rho}$, tada je jedinica na mesu $ij$ u matrici $M_{\rho}\,$.

## 2.3 Relacija ekvivalencije
**Def**. Binarna relacija je relacija **ekvivalencije** ako je (R), (S) i (T)

Primeri relacija ekvivalencije:
- = u skupu $\mathbb{R}$
- sličnost trouglova
- || - paralelnost pravih u $\mathbb{R}^2$, $\mathbb{R}^3$, ...
- $\equiv_m$ - kongruentnost u skupu $\mathbb{Z}$

**Def**. Neka je $\sim$ relacija ekvivalencije na skupu $A$.
**Klasa** elementa $a \in A$ je skup $C_a = \{ x \in A\ | \ a\sim x\}$
Oznaka: $[\,a\,]$

Stav. Neka je $\sim$ relacija ekvivalencije na skupu $A$, tada
1. Svaka klasa je neprazan skup
2. $a, \ b \in A$. $\ \ C_a\cap C_b \ne \varnothing \quad \Rightarrow \quad C_a = C_b$
3. $A$ je unija svih klasa ekvivalencije relacije $\sim$

![[klasa ekvivalencije stav.png]]
**Def**. Neka je $\sim$ relacija ekvivalencije na skupu $A$.
**Količnički skup** (faktor skup) je $A/\!\sim\:\: = \{ C_x\ | \ x \in A \}$

Svaka relacija ekvivalencije na skupu $A$ određuje jednu particiju tog skupa.
(Skupovi čine particiju skupa $A$ ako su disjunktni i njihova unija je jednaka $A$)

![[klasa ekvivalencije primer.png]]

## 2.4 Relacija poretka

(_**Def**. Binarna relacija je relacija **strogog** (parcijalnog) **poretka** ako je (AR), (S) i (T). Oznaka: $\prec$._)

**Def**. Binarna relacija je relacija **nestrogog** (parcijalnog) **poretka** ako je (R), (S) i (T).  Oznaka: $\preceq$.

**Def**. Ako je u skupu uvedena relacija parcijalnog poretka, tada je taj skup **uređen** ili se zove **poset**.

**Def**. $a,\ b \in A \:$ su uporedivi ako važi $a\preceq b\:$ ili $\:b\preceq a$

**Def**. Ako su u skupu svaka dva elementa uporediva, tada je taj skup **totalno uređen** i relacija je **totalnog** (umesto da bude parcijalnog) poretka.

**Def**. Podskup skupa $A$ je **lanac** ako su u njemu svaka dva elementa uporediva.
**Def**. Podskup skupa $A$ je **antilanac** ako u njemu svaka dva elementa nisu uporediva.
Neki podskup može biti ni lanac ni antilanac.

 >Primer
$X = \{ a, \ b, \ c\}$
$\mathcal{P}(X) = \{\varnothing, \ \{ a\},\ \{b\},\ \{c\}, \ \{a,\ b\}, \ \{a,\ c\}, \ \{b,\ c\},\ \{ a, \ b, \ c\}\}$
Relacija $\subseteq$ u skupu $\mathcal{P}(X)$
(R) $\forall A \in \mathcal{P}(X)\ \ \ A\subseteq A$
(AS) $\forall A, \ B \in \mathcal{P}(X)\ \ \ (A\subseteq B, \ B\subseteq A) \ \ \ \Rightarrow \ \ \ A=B$
(T) $\forall A, \ B, \ C \in \mathcal{P}(X)\ \ \ (A\subseteq B, \ B\subseteq C) \ \ \ \Rightarrow \ \ \ A\subseteq C$
jeste relacija nestrogog poretka.
— $\{a,\ b\}$ i $\{a,\ c\}$ nisu uporedivi $\ \ \ \Rightarrow \ \ \ \mathcal{P}(X)$  nije totalno uređen.
— Lanac: $\varnothing \subseteq \{ a\}\subseteq \{ a,\ b\}\subseteq \{ a,\ b, \ c\}$
— Antilanac: $\{\{ a\},\ \{b\}, \ \{c\}\}$ - svaka dva nisu uporediva
Haseov dijagram:
![[haseov dijagram primer 1.png]]
Svaka linija predstavlja relaciju između dva elementa tako da (donji element) $\!\preceq\!$ (gornji element). Ali relacije kao na primer $\{a\} \subseteq \{a,\ b,\ c\}$ se ne označavaju jer "prolaze" kroz drugi element $\{a\} \subseteq \{a,\ b\} \subseteq \{a,\ b,\ c\}$

$\:$

**Def**. Neka je $\preceq$ relacija nestrogog parcijalnog poretka u skupu $A$, $B \subseteq A$. Tada:
- $a\in B$ je **najmanji** element u $B$ ako $\forall x \in B \ \ \ a \preceq x$
- $a\in B$ je **najveći** element u $B$ ako $\forall x \in B \ \ \ x \preceq a$
- $a\in B$ je **minimalni** element u $B$ ako $\forall x \in B \ \ \ x \preceq a \ \ \Rightarrow \ \ a=x$
- $a\in B$ je **maksimalni** element u $B$ ako $\forall x \in B \ \ \ a \preceq x \ \ \Rightarrow \ \ a=x$

Na haseovom dijagramu:
- Najmanji — jedinstven donji element, koji je povezan sa svim ostalim elementima.
- Najveći — jedinstven gornji element, koji je povezan sa svim ostalim elementima.
- Minimalni — element koji nema veza sa elementima dole od sebe.
- Maksimalni — element koji nema veza sa elementima gore od sebe.
 
>Primer 1:
$A = \{x,\ y,\ z,\ t,\ f,\ g\}$
Relacija je zadata dijagramom
![[haseov dijagram primer 2.png]]
$x$ je najmanji i minimalni
$g$ i $t$ su maksimalni
najveći ne postoji

>Primer 2:
$A = \{2^n\ | \ n \geqslant 0\} \cup \{3\}$
Relacija je zadata dijagramom
![[haseov dijagram primer 3.png]]
$1$ je najmanji i minimalni
$3$ je maksimalni
najveći ne postoji

Teorema. Ako $\exists a \in B \:$ najmanji (najveći) element, tada
1. $a$ je jedinstven najmanji (najveći) element
2. $a$ je jedinstven minimalni (maksimalni) element

![[najminmaks teorema.png]]

![[najminmaks primer.png]]
$\:$
**Def**. Neka je $\preceq$ relacija nestrogog parcijalnog poretka u skupu $A$, $B \subseteq A$. Tada:
- $a \in A$ je donje ograničenje skupa $B$ ako $\ \forall x \in B \ \ \ a \preceq x$
- $a \in A$ je gornje ograničenje skupa $B$ ako $\ \forall x \in B \ \ \ x \preceq a$
- Najveće donje ograničenje skupa $B$ ako postoji zove se infinum: $\inf(B)$
- Najmanje gornje ograničenje skupa $B$ ako postoji zove se supremum: $\sup(B)$

>Primer:
$B = [0,\ 1) \in \mathbb{R}$
$(-\infty, \ 0]$ - skup donjih ograničenja; $\inf(B)=0$
$[1, \ +\infty)$ - skup gornjih ograničenja; $\sup(B)=1$

# 3 Funkcije
**Def**. Relacija $f \subseteq A\times B\:$ je funkcija ako $\forall x\in X = Dom(f)\ \ \ \exists! y \in Y = B\ \ : \ \ (x, \ y) \in f$
Oznaka: $f:\ \ X \to Y$
Umesto $(x, \ y) \in f$ piše se $f(x) = y$
Skup $X$ se zove domen funkcije, skup $Y$ se zove kodomen funkcije.

![[funkcija.png]]

Funkcije $f:\ \ X \to Y\:$ i $\:g:\ \ A \to B\:$ su **jednaki** ako 1)$\ X = A$; 2)$\ Y = B$; 3)$\ \forall x \in X \ \ \ f(x)=g(x)$

**Def**. Funkcija $f:\ \ X \to Y\:$ je **surjekcija ("na")**, ako $\forall y \in Y\ \ \ \exists x \in X \ \ :\ \ f(x)=y$
(Funkcija preslikava nešto u svaki element kodomena)

**Def**. Funkcija $f:\ \ X \to Y\:$ je **injekcija ("1-1")**, ako $\forall x_1,\ x_2 \in X\ \ \ f(x_1)=f(x_2) \ \ \ \Rightarrow \ \ \ x_1=x_2$
(Funkcija ne može da slika dva različitih elementa domena u jedan element kodomena)

**Def**. Funkcija je **bijekcija** ako je "na" i "1-1".

![[funkcija primer 1.png]]

**Def**. **Identičko preslikavanje** (identitet) na $X$ je funkcija $id_X : \ \ X \to X \ \:$ definisana sa $\forall x \in X \ \ \ id_X(x)=x$

## 3.1 Kompozicija funkcija
Teorema. Ako su $f \subseteq A \times B\:$ i $\:g \subseteq B \times C\:$ funkcije tada kompozicija relacija $g\,\!\circ\!f \subseteq A\times C$ je funkcija i važi $\forall x\in A\ \ \ (g\,\!\circ\!f)(x) = g(f(x))$
> Dokaz: pps $g\,\!\circ\!f$ nije funkcija tada važi $\exists a \in A, \ c_1,\ c_2\in C\ \ : \ \ (a,\ c_1), \ (a,\ c_2)\in g\,\!\circ\!f$.
$(a,\ c_1)\in g\,\!\circ\!f\ \ \Rightarrow \ \ \exists b_1\in B\ \ : \ \ (a,\ b_1) \in f\ \ \land \ \ (b_1,\ c_1)\in g$
$(a,\ c_2)\in g\,\!\circ\!f\ \ \Rightarrow \ \ \exists b_2\in B\ \ : \ \ (a,\ b_2) \in f\ \ \land \ \ (b_2,\ c_2)\in g$
$f$ je funkcija, $a\in Dom(f)\ \ \Rightarrow\ \ b_1 = f(a) = b_2$ 
$g$ je funkcija, $b_1=b_2$ $\ \ \Rightarrow\ \ c_1 = c_2$ 
Kontradikcija $\ \ \Rightarrow\ \ g\,\!\circ\!f$ je funkcija

**Def**. Ako su $f:\ \ X \to Y\:$ i $\:g:\ \ Y \to Z\:$  funkcije tada se funkcija $g\,\!\circ\!f:\ \ X \to Z\:$ zove **kompozicija** funkcija $f$ i $g$ i važi $\forall x\in A\ \ \ (g\,\!\circ\!f)(x) = g(f(x))$

![[funkcija primer 2.png]]

Stav. Ako su $f:\ \ A \to B$ , $\:g:\ \ B \to C\:$ i $\:h:\ \ C \to D\:$ funkcije tada važi $h\,\!\circ\!(g\,\!\circ\!f) = (h\,\!\circ\!g)\,\!\circ\!f$

Stav. Neka su $f:\ \ A \to B\:$ i $\:g:\ \ B \to C\:$ funkcije tada
1. Ako je $g\,\!\circ\!f$ "1-1" onda je $f$ "1-1"
2. Ako je $g\,\!\circ\!f$ "na" onda je $g$ "na"
3. Ako su $f$ i $g$ "1-1" onda je $g\,\!\circ\!f$ "1-1"
4. Ako su $f$ i $g$ "na" onda je $g\,\!\circ\!f$ "na"

![[kompozicija funkcija stav.png]]

![[kompozicija funkcija primer.png]]

## 3.2 Inverzna funkcija
Ako je relacija $f \subseteq X\times Y\:$ funkcija tada joj inverzna relacija $f^{-1}$ ne mora da bude funkcija.

**Def**. Funkcija $g:\ \ Y \to X\:$ je **levi inverz** funkcije $f:\ \ X \to Y\:$ ako $\forall x \in X \ \ \ (g\,\!\circ\!f)(x) = x\:\:$ (tj. $g\,\!\circ\!f\equiv id_X$)
Stav. $f$ ima levi inverz $\:\ \Leftrightarrow \ \:$ $f$ je "1-1"
![[inverzna fja stav levi.png]]

**Def**. Funkcija $g:\ \ Y \to X\:$ je **desni inverz** funkcije $f:\ \ X \to Y\:$ ako $\forall y \in Y \ \ \ (f\!\circ\!g)(y) = y\:\:$ (tj. $f\!\circ\!g\equiv id_Y$)
Stav. $f$ ima desni inverz $\:\ \Leftrightarrow \ \:$ $f$ je "na"
![[inverzna fja stav desni.png]]

**Def**. Funkcija $g:\ \ Y \to X\:$ je **inverz** funkcije $f:\ \ X \to Y\:$ ako je ona levi i desni inverz. Važi $g \equiv f^{-1}$
Teorema. $f$ ima  inverz $\:\ \Leftrightarrow \ \:$ $f$ je bijekcija
(Dokaz: kombinacija prethodna dva stava)

- $f$ je bijekcija $\:\ \Leftrightarrow \ \:$ $f$ ima inverz $f^{-1}$ $\:\ \Leftrightarrow \ \:$
 $\Leftrightarrow \ \:$$f^{-1}$ ima inverz $f$ $\:\ \Leftrightarrow \ \:$ $f^{-1}$ je bijekcija
- $(f^{-1})^{-1} \equiv f$

## 3.3 Direktna i inverzna slika skupa
Neka je $f:\ \ X \to Y$ funkcija
**Def**. $A \subseteq X$. **Direktna slika** skupa $A$ je skup $f[A]=\{ f(x)\ | \ x\in A\}$
**Def**. $B \subseteq Y$. **Inverzna slika** skupa $B$ je skup $f^{-1}[B]=\{ x \in X\ | \ f(x)\in B\}$
*($f^{-1}[B]$ je samo oznaka $f$ ne mora da ima inverz)*

$y \in f[A] \ \ \Leftrightarrow \ \ \exists x\in A \ : \ f(x) =y$
$x \in f^{-1}[B] \ \ \Leftrightarrow \ \ f(x)\in B$

![[direktna i inverzna slika primer 1.png]]

Stav. Neka je $f:\ \ X \to Y$ funkcija. $A, \, B\subseteq X;\ \ C,\, D\subseteq Y$. Tada
1. $f[\varnothing] = \varnothing ,\ \ f^{-1}[\varnothing] = \varnothing$
2. $A \subseteq B \ \ \Rightarrow\ \ f[A]\subseteq f[B]$
3. $C \subseteq D \ \ \Rightarrow\ \ f^{-1}[C]\subseteq f^{-1}[D]$

> Dokaz:
> 1. pps $\exists y \in f[\varnothing]\ \ \ \ \exists x\in \varnothing \ : \ f(x) =y \ \:$ — kontradikcija
> 2. $y \in f[A] \ \ \Rightarrow\ \ \exists x\in A \subseteq B \ : \ f(x) = y$
>    $\exists x\in B\ : \ f(x) = y\ \ \Rightarrow\ \ y \in f[B]$
> 3. $x \in f^{-1}[C] \ \ \Rightarrow\ \ f(x) \in C \subseteq D$
>    $f(x) \in D\ \ \Rightarrow\ \ x \in f^{-1}[D]$


Stav. Neka je $f:\ \ X \to Y$ funkcija. $A, \, B\subseteq X;\ \ C,\, D\subseteq Y$. Tada
1. $A \subseteq f^{-1}[f(A)]$ $\quad\quad\quad\quad\quad$(jednakost ako je $f$ "1-1")
2. $f[f^{-1}(C)] \subseteq C$ $\quad\quad\quad\quad\quad$(jednakost ako je $f$ "na")
3. $f[A\cup B] = f[A] \cup f[B]$
4. $f[A\cap B] \subseteq f[A] \cap f[B]$ $\ \ \ \ \ \,$(jednakost ako je $f$ "1-1")
5. $f[A\,\setminus\,\!B] \supseteq f[A] \,\setminus\,\! f[B]$ $\ \ \ \ \ \,$(jednakost ako je $f$ "1-1")
6. $f^{-1}[C\cup D] = f^{-1}[C] \cup f^{-1}[D]$
7. $f^{-1}[C\cap D] = f^{-1}[C] \cap f^{-1}[D]$
8. $f^{-1}[C\,\setminus\,\!D] = f^{-1}[C]\,\setminus\,\!f^{-1}[D]$

 ![[direktna i inverzna slika primer 2.png]]
 
## 3.4 Karakteristična funkcija
**Def**. Neka je $X$ univerzum i $A\subseteq X$.
**Karakteristična funkcija** skupa $A$ je funkcija $\chi_A:\ \ X\to \{0,\ 1\}$ definisana sa $\chi_A(x) = \begin{cases} 1, \ \ x\in A\\ 0, \ \ x\notin A \end{cases}$

![[karakt fja primer 1.png]]

Stav. $A = B\quad\Leftrightarrow\quad\chi_A=\chi_B$
> Dokaz: $[\Rightarrow]$ iz definicije
> $[\Leftarrow]\ \ \ \chi_A=\chi_B$
> $\begin{aligned} x \in A \ \ \Rightarrow \ \ \chi_A = 1  \ \ \Rightarrow \ \  \chi_B = 1 \ \ \Rightarrow \ \  x \in B \\ x \in B \ \ \Rightarrow \ \ \chi_B = 1  \ \ \Rightarrow \ \  \chi_A = 1 \ \ \Rightarrow \ \  x \in A \end{aligned}  \ \ \Rightarrow A = B$

$\:$
![[karakt fja.png]]

![[karakt fja primer 2.png]]

# 4 Prirodni brojevi

## 4.1 Peanove aksiome
- P1. $\:\:$$0$ je prirodan broj.
- P2. $\:\:$Ako je $x$ prirodan broj tada je i njegov sledbenik $x'$ prirodan broj.
- P3. $\:\:$Ako su $x$ i $y$ prirodni brojevi takvi da je $x' = y'$ onda $x=y$.
- P4. $\:\:$Za svaki  prirodni broj $x$ važi $x'\ne0$.
- P5.  $\:\:$Neka je $\Phi$ svojstvo prirodnih brojeva takvo da
  1. važi $\Phi(0)$
  2. za svaki prirodni broj $x$ ako važi $\Phi(x)$ onda važi i $\Phi(x')$

	 tada $\Phi(x)$ važi za svaki prirodni broj $x$.

$\mathbb{N}=\{ 0,\, 1,\, 2,\, 3,\, \dots \}$
## 4.2 Fon Nojmanov model
- $0=\varnothing$
- $n' = n \cup\{ n \}$

Tada:
$1 = \{ 0 \} = \{ \varnothing \}$
$2 = \{ 0,\, 1 \}=\{ \varnothing,\, \{ \varnothing \} \}$
$3 = \{ 0,\, 1,\, 2 \} = \{ \varnothing,\, \{ \varnothing \},\, \{ \varnothing,\, \{ \varnothing \} \} \}$
$4= \{ 0,\, 1,\, 2,\, 3 \} = \{ \varnothing,\, \{ \varnothing \},\, \{ \varnothing,\, \{ \varnothing \} \},\, \{ \varnothing,\, \{ \varnothing \},\, \{ \varnothing,\, \{ \varnothing \} \} \} \}$
$\dots$

Teorema. Fon Nojmanov model zadovoljava Peanove aksiome.
![[FNM teorema.png]]

## 4.3 Matematička indukcija

### 4.3.1 Princip matematičke indukcije

Neka je $\Phi$ svojstvo prirodnih brojeva takvo da
  - važi $\Phi(0)$
  - za svaki prirodni broj $n$ $\Big[$ ako važi $\Phi(n)$ onda važi i $\Phi(n')$ $\Big]$

tada $\Phi(n)$ važi za svaki prirodni broj $n$.

### 4.3.2 Princip potpune indukcije
Neka je $\Phi$ svojstvo prirodnih brojeva takvo da 
-  za svaki prirodni broj $n$  $\Big[$ ako važi $\forall k<n \ \ \Phi(k)$ onda važi i $\Phi(n)$ $\Big]$

tada $\Phi(n)$ važi za svaki prirodni broj $n$.

Teorema. PMI $\quad \Rightarrow \quad$ PPI
![[PPI teorema.png]]

### 4.3.3 Princip najmanjih elemenata
- Relacija poretka: $\forall n\in \mathbb{N} \ \ \ n< n'$

Neka je $A \ne \varnothing,\ \ A \subseteq \mathbb{N} \ \:$ tada u $A$ postoji najmanji element.

Teorema. PPI $\quad \Rightarrow \quad$ PNE
![[PNE teorema.png]]

### 4.3.4 Još varijacije matematičke indukcije
1. Neka je $\Phi$ svojstvo prirodnih brojeva takvo da
	  - važi $\Phi(k)$ za neko $k\in \mathbb{N}$
	  - za svaki prirodni broj $n\geqslant k$ $\Big[$ ako važi $\Phi(n)$ onda važi i $\Phi(n')$ $\Big]$

	tada $\Phi(n)$ važi za svaki prirodni broj $n\geqslant k$.
2.  Neka je $\Phi$ svojstvo prirodnih brojeva takvo da
	  - važe $\Phi(0),\,\Phi(1),\, \dots,\, \Phi(k-1)$ za neko $k\in \mathbb{N}$
	  - za svaki prirodni broj $n\geqslant k$ $\Big[$ ako važe $\Phi(n-k),\,\Phi(n-k+1),\, \dots,\, \Phi(n-1)$ onda važi i $\Phi(n)$ $\Big]$

	tada $\Phi(n)$ važi za svaki prirodni broj $n$.

## 4.4 Operacije $+$ i $\,\cdot\,$ u prirodnim brojevima
**Def**. **Sabiranje** prirodnih brojeva:
- $x + 0 = x$
- $x+y\,' = (x+y)'$

Osobine: $\forall x,\,y,\,z \in \mathbb{N}$
1. $x + (y + z) =(x + y) + z$
2. $x + 0 = 0 + x = x$
3. $x + 1 = 1 + x$
4. $x + y = y + x$
5. $x + y = 0 \quad \Rightarrow \quad x = 0 \ \ \mathrm{i}\ \ y = 0$
6. $x + z =y + z \quad \Rightarrow \quad x = y$

![[prirodni br osbine sabiranja.png]]

**Def**. **Množenje** prirodnih brojeva:
- $x \cdot 0 = 0$
- $x\cdot y\,' = x\cdot y + x$

Osobine: $\forall x,\,y,\,z \in \mathbb{N}$
1. $x \cdot (y + z) = x\cdot y + x\cdot z$
2. $x \cdot (y \cdot z) =(x \cdot y) \cdot z$
3. $(x + y) \cdot z = x\cdot z + y\cdot z$
4. $0 \cdot x = 0$
5. $1 \cdot x = x$
6. $x\cdot y = y\cdot x$
7. $x \cdot y = 0 \quad \Rightarrow \quad x = 0 \ \ \mathrm{ili}\ \ y = 0$

![[prirodni br osbine množenja.png]]

# 5 Teorija brojeva
## 5.1 Deljivost i Euklidsko deljenje

**Def**. $a,\, b\in \mathbb{N}$
$a\,|\,b\:$ ($a$ deli $b$) ako $\exists c \in \mathbb{N}\ \ : \ \ b = a\cdot c$

Stav. U skupu $\mathbb{N}\setminus\{ 0 \}$ relacija deljivosti je relacija nestrogog parcijalnog poretka.
![[deljivost stav.png]]

Osobine: $\: \forall a,\,b,\,c \in \mathbb{N}$
1. $a\,|\,0\:$
2. $a\,|\,b\ \ \mathrm{i}\ \ a\,|\, c\ \ \ \Rightarrow \ \ \ a\,|\, (b+c)$
3. $a\,|\,b\ \ \mathrm{ili}\ \ a\,|\, c\ \ \ \Rightarrow \ \ \ a\,|\, (b\cdot c)$
4. $a\,|\,b\ \ \ \Rightarrow \ \ \ a\,|\, b^{n},\ \:$ za $\ \forall n\in \mathbb{N}\setminus\{ 0 \}$ 

![[deljivost osobine.png]]

Teorema (o Euklidskom deljenju). Neka su $a,\, b \in \mathbb{N},\ \ b=0$
Tada postoji jedinstven par $q,\,r\in \mathbb{N}\:$ takav da $a = b\cdot q + r \quad 0\leqslant r<b$
![[euklidsko deljenje teorema 1.png]]

**Def**. $a,\, b\in \mathbb{Z}$
$a\,|\,b\:$ ($a$ deli $b$) ako $\exists c \in \mathbb{Z}\ \ : \ \ b = a\cdot c$

Deljivost nije relacija poretka u skupu $\mathbb{Z}\setminus\{ 0 \}$, jer ne važi (AS).

Teorema. Neka su $a,\, b \in \mathbb{Z},\ \ b=0$
Tada postoji jedinstven par $q,\,r\in \mathbb{Z}\:$ takav da $a = b\cdot q + r \quad 0\leqslant r<|b|$
![[euklidsko deljenje teorema 2.png]]

**Def**. Neka su $a,\,b \in \mathbb{N}\, (\mathbb{Z})$. $d\in \mathbb{N}$ je **zajednički delilac** $a$  i $b$ ako $d\,|\,a$ i $d\,|\,b$.
$d$ je najveći zajednički delilac (**NZD**) ako za svako $d'\in \mathbb{N}$ takvo da $d'\,|\,a$ i $d'\,|\,b$ važi $d'\,|\,d$.

**Def**. Neka su $a,\,b \in \mathbb{N}\, (\mathbb{Z})$. $s\in \mathbb{N}$ je **zajednički sadržalac** $a$  i $b$ ako $a\,|\,s$ i $b\,|\,s$.
$s$ je najmanji zajednički delilac (**NZS**) ako za svako $s'\in \mathbb{N}$ takvo da $a\,|\,s'$ i $b\,|\,s'$ važi $s\,|\,s'$.

## 5.2 Euklidov algoritam

Teorema. Ako je $a = b\cdot q + r\:$, tada važi $\mathrm{NZD}(a,\,b) = \mathrm{NZD}(b,\,r)$
![[eukl alg t1.png]]

### 5.2.1 Algoritam:
$a, b \in \mathbb{N}, \ \ b \ne 0$
Primena teoreme odogo više puta dok ostatak neće postati 0:
$a = b\cdot q_{1} + r_{1}\quad\quad\quad\quad\quad\quad 0< r_{1}<b$
$b = r_{1}\cdot q_{2} + r_{2}\quad\quad\quad\quad\quad\ \ \, 0< r_{2}<r_{1}$
$r_{1} = r_{2}\cdot q_{3} + r_{3}\quad\quad\quad\quad\quad\ 0< r_{3}<r_{2}$
$\dots$
$r_{n-3} = r_{n-2}\cdot q_{n-1} +r_{n-1}\quad\ 0< r_{n-1}<r_{r-2}$
$r_{n-2} = r_{n-1}\cdot q_{n} +r_{n}\quad\quad\quad\!\ 0< r_{n}<r_{r-1}$
$r_{n-1} = r_{n}\cdot q_{n+1} \quad\quad\quad\quad\quad\ r_{n+1}=0$

Teorema. Poslednji nenula ostatak u Euklidovom algoritmu $r_{n}$ je jednak $\mathrm{NZD}(a,\,b)$.
> Dokaz:
> Iz teoreme:
> $\mathrm{NZD}(a,\,b) = \mathrm{NZD}(b,\,r_1) = \mathrm{NZD}(r_1,\,r_2) = \dots = \mathrm{NZD}(r_{n-2},\,r_{n-1}) = \mathrm{NZD}(r_{n-1},\,r_{n})$
> Poslednja jednčina: $r_{n-1} = r_{n}\cdot q_{n+1} \ \ \Rightarrow\ \ r_{n}\,|\,r_{n-1}\ \ \Rightarrow\ \ \mathrm{NZD}(r_{n-1},\,r_{n}) = r_{n}$

$\:$
Posledica.$\ \forall a,\,b\in \mathbb{N}\ \ \ \exists p,\,q \in \mathbb{Z}\ \ : \ \ a\cdot p + b\cdot q = \mathrm{NZD}(a,\,b)$ 
![[eukl alg posl.png]]

![[eukl alg primer.png]]

### 5.2.2 Matrična metoda:
$M_0=\left[\begin{array}{c|c c} 
	a & 1 & 0\\ 
	b & 0 & 1 
\end{array}\right]$

Operacije
- T1: zamena mesta vrsta
- T2: množenje vrsta sa -1
- T3: dodavanje jedne vrste pomnožene celim brojem drugoj vrsti.

Matrica $M_n=\left[\begin{array}{c|c c} 
	x & p & q\\ 
	y & r & s 
\end{array}\right]$ se dobija primenom T1, T2, T3

Teorema. Za $M_{n}$ važi $\begin{cases} x = a\cdot p + b \cdot q\\ y = a\cdot r + b \cdot s \end{cases}$
![[eukl alg matr 1.png]]

Teorema. Za $M_{n}$ važi $\mathrm{NZD}(a,\, b) = \mathrm{NZD}(x,\,y)$
![[eukl alg matr 2.png]]

$\:$
Primenom T1, T2, T3 iz matrice $\left[\begin{array}{c|c c} 
	a & 1 & 0\\ 
	b & 0 & 1 
\end{array}\right]$ treba dobiti matricu oblika $
\left[\begin{array}{c|c c} 
	d & p & q\\ 
	0 & p' & q' 
\end{array}\right]$, tada je $d=\mathrm{NZD}(a,\,b)$ i $d=a\cdot p + b\cdot q$

![[eukl alg matr primer.png]]

---
Teorema. $a\,|\,b\, c\ \:$ i $\ \: \mathrm{NZD}(a,\, b)= 1$. $\:$ Tada $a\,|\,c$ ^015ce1
>Dokaz: Iz posledice Euklidovog algoritma:
>$\exists p,\,q\in \mathbb{Z}\ \ : \ \ a\,p + b\,q = 1$, pomnožimo jednačinu sa $c$: $\:$ $a\,c\,p + b\,c\,q = c$
>$\begin{aligned} a\,|\,a\,c\,p \\ a\,|\,b\,c \ \ \Rightarrow \ \ a\,|\, b\,c\,q\end{aligned} \ \ \Rightarrow \ \ a\,|\,(a\,c\,p + b\,c\,q) \ \ \Rightarrow \ \ a\,|\,c$

Posledica. $a\,|\,c\:$ i $\:b\,|\,c$; $\:\mathrm{NZD}(a,\,b) = 1$. $\:$ Tada $a\,b\,|\,c$  
> Dokaz: $c = b\,b_{1},\quad b_{1}\in \mathbb{Z}$
> $\begin{align}a\,|\,c\ \ \Rightarrow\ \ a\,|\,b\,b_{1}\\ \mathrm{NZD}(a,\,b) = 1\end{align}\ \  \stackrel{\mathrm{iz\ teoreme}}{\Longrightarrow} \ \ a\,|\,b_{1}\ \ \Rightarrow \ \ \exists t \in \mathbb{Z} \ :\ b_{1}=a\,t$
> $c = b\,b_{1}=a\,b\,t \ \ \Rightarrow\ \ a\,b\,|\,c$

$\:$
## 5.3 Prosti brojevi

**Def**. Prirodan broj $p>1$ je **prost** ako su njegovi jedini delioci $1$ i $p$. U suprotnom je **složen**.

Stav. $p$ je prost broj i $p\,|\, a\,b$ $\:$ ($a,\,b\in \mathbb{Z}$)
Tada $p\,|\,a\:$ ili $\:p\,|\,b$
>Dokaz: $p\nmid a\ \ \ \Rightarrow\ \ \ \mathrm{NZD}(p,\,a) = 1$
>Iz prethodne teoreme sledi $p\,|\,b$

Stav. Za prirodni broj $n>1$ važi da je prost ili proizvod prostih brojeva.
![[prost stav.png]]

Teorema. Postoji beskonačno mnogo prostih brojeva.
>Dokaz: pps ima  ih konačno mnogo
>Neka su to $p_{1}<p_{2}<\dots<p_{n}$
>Tada $m = p_{1}\,p_{2}\,\dots p_{n} +1$ mora biti složen (jer $m>p_{n}$)
>nijedan od brojeva $p_{1},\,p_{2},\,\dots,\,p_{n}$ ne deli $m$ $\ \:\Rightarrow\ \:$ $m$ je prost (kontradikcija).

Teorema (osnovna teorema aritmetike). Svaki prirodni broj $n>1$ može se napisati u obliku proizvoda stepena prostih brojeva na jedinstven način (do na redosled faktora).
$n = p_{1}^{\alpha_{1}}\,p_{2}^{\alpha_{2}}\,\dots\,p_{k}^{\alpha_{k}}$, $\quad$ $p_{1},\, p_{2},\,\dots,\,p_{n}$ su prosti; $\:$ $\alpha_{1},\, \alpha_{2},\,\dots,\,\alpha_{n} \geqslant 1$

![[prost teorema.png]]

## 5.4 Diofantove jednačine

**Def**. **Diofantova** je jednačina sa celobrojnim koeficijentima, u kojoj treba naći sva rešenja u $\mathbb{Z}$

- $a\,x = b\quad a,\,b\in \mathbb{Z},\ a\ne 0$
Ima jedinstveno rešenje $x = \frac{b}{a}$, ako $a\,|\,b$ (inače nema rešenja)
- $a\,x+b\,y=c\quad  a,\,b,\,c\in \mathbb{Z},\ a\ne 0,\ b\ne 0$
Treba naći sve parove $(x,\,y)$ da bi važila jednačina:

>$d := \mathrm{NZD}(a,\,b)$ tada (iz posledice Euklidovog algoritma)
$\exists u,\,v\in \mathbb{Z}\ \ :\ \ a\,u + b\,v = d$
>
>Stav. $a\,x+b\,y=c$ ima rešenja akko $\mathrm{NZD}(a,\,b)\,|\,c$
> > [$\Leftarrow$] 
> > Ako $d\,|\,c$, tada $c':= \frac{c}{d}$ 
> > Pomnožimo jednačinu $a\,u + b\,v = d$ sa $c'$:
> > $a\,u\,c' + b\,v\,c' = c$
> > Odakle imamo jedno rešenje: $(u\,c',\,v\,c')$
> > 
> > [$\Rightarrow$] 
> > Ako $\exists$ rešenje $a\,x+b\,y=c$
> > $\mathrm{NZD}(a,\,b) = d$, tada $d\,|\,a$ i $d\,|\,b$
> > $\Rightarrow \ \ d\,|\,(a\,x+b\,y)\ \ \Rightarrow \ \ d\,|\,c$
> > 
>
>Potražimo sva rešenja jednačine:
>imamo jedno rešenje $(x_{0},\,y_{0}):=(u\,c',\,v\,c')$ 
>važi $a\,x_{0}+b\,y_{0}=c$ 
>
>Tada je $a\,x+b\,y=c$ isto što i $a\,x+b\,y=a\,x_{0}+b\,y_{0}$
>$a\,(x-x_{0}) = -b\,(y-y_{0})$
>
>$\mathrm{NZD}(a,\,b)=d$
>$\begin{aligned} a = a'\,d \\ b = b'\,d\end{aligned} \ \ \Rightarrow\ \ \mathrm{NZD}(a',\,b') = 1$
>
>Vratimo to u jednačinu:
>$a'\,d\,(x-x_{0}) = -b'\,d\,(y-y_{0})$
>$a'\,(x-x_{0}) = -b'\,(y-y_{0})$
>
>$\begin{aligned} b'\,|\,a'\,(x-x_{0}) \\ \mathrm{NZD}(a',\,b') = 1\end{aligned} \ \ \Rightarrow\ \ b'\,|\,(x-x_{0})\ \ \Rightarrow\ \ \exists t\in \mathbb{Z}\ :\ x-x_{0}=b'\,t$
>
>$x = x_{0} + b'\,t$
>$a'\,b'\,t=-b'(y-y_{0})\ \ \Rightarrow\ \ y = y_{0}-a'\,t$
>
>Opšte rešenje jednačine:
>$\begin{aligned} x= u\,c' + b'\,t\quad\quad\quad x = \frac{c\,u+b\,t}{d}\\ y=v\,c' - a'\, t\quad\quad\quad y = \frac{c\,v-a\,t}{d}\end{aligned}\quad\quad\quad\forall t\in \mathbb{Z},$
>gde su $u$, $v$ brojevi iz posledice Euklidovog algoritma za $a$ i $b$ $\:$ (tj važi $a\,u+b\,v=d$)

![[diofantova jednačina primer.png]]

## 5.5 Kongruencije

**Def**. Neka su $a,\,b\in \mathbb{Z}$ i $m> 1$ je prirodan broj. Tada $a$ je kongruentno sa $b$ po modulu $m$ ($a\equiv_{m} b$) ako $m\,|\,(a-b)$

($a$ i $b$ daju isti ostatak pri deljenju na $m$)

Stav. $\equiv_{m}$ je relacija ekvivalencije na $\mathbb{Z}$
![[kongr stav 1.png]]

Stav. Ako $a\equiv_{m}a_{1}$ i $b\equiv_{m}b_{1}$, onda važi
1) $a+b\equiv_{m}a_{1}+b_{1}$
2) $a\cdot b \equiv_{m} a_{1}\cdot b_{1}$
3) $a^{k} \equiv_{m} a_{1}^{k}$, $\:$ za svako $k\in \mathbb{Z}$

![[kongr stav 2.png]]

Stav. Broj je deljiv sa 3 akko zbir njegovih cifara je deljiv sa 3.
> $a = a_{k}\cdot10^{k} + a_{k-1}\cdot10^{k-1} +\dots+a_{1}\cdot10 +a_{0}$,
> $a_{k},\,a_{k-1},\,\dots,\,a_{1},\,a_{0}$ su cifre broja $a$
> 
> $10\equiv_{3}1$
> $10^{2}\equiv_{3}10\equiv_{3}1$
> $10^{3}\equiv_{3}10\equiv_{3}1$
> $\dots$
> $10^{k}\equiv_{3}10\equiv_{3}1$
> 
> Tada: $a\equiv_{3}a_{k}\cdot10^{k} + a_{k-1}\cdot10^{k-1} +\dots+a_{1}\cdot10 +a_{0}\equiv_{3}$
> $\equiv_{3}a_{k} + a_{k-1} +\dots+a_{1} +a_{0}$

Oznaka. $\mathbb{Z}_{n} = \{ 0,\,1,\,\dots,\,n \}$

> Primer. Odrediti ostatak pri deljenju $2^{30}$ sa $13$.
> Treba naći $x\in\mathbb{Z}_{13}$ tako da $2^{30}\equiv_{13}x$ *
> 
> $2^{30} = \big(2^{6}\big)^{5} = \big(2^{2}\cdot2^{4}\big)^{5}$
> 
> $2^4 = 16 \equiv_{13}3$
> $2^6 = 2^{2}\cdot2^{4} \equiv_{13}4\cdot3\equiv_{13}12\equiv_{13}-1$ **
> 
> $2^{30}= \big(2^{6}\big)^{5} \equiv_{13} (-1)^{5}\equiv_{13}-1\equiv_{13}12$ 
> 
> \* U zadacima nikada ne morate računati veće stepene. Uvek je moguće faktorisati i napraviti ugneždeni stepeni (na primer $12^{21} = 3^{21}\cdot\big(2^{2}\big)^{21}=\big(3^{7}\big)^{3} \cdot\bigg(\big(2^{7}\big)^{3}\bigg)^{2} =\dots$; $7^{26} = 7\cdot\big(7^{5}\big)^{5}=7\cdot\Big(7\cdot\big(7^{2}\big)^{2}\Big)^{5}=\dots$ )
> \** Obično je cilj imati najmanji broj po modulu (u ovom slučaju u intervalu $[-6,\, 6]$), onda je lakše množiti.

Stav. $a\cdot b\equiv_{m}a \cdot c\:$ i $\:\mathrm{NZD}(m,\,a)= 1$. $\:$ Tada $b\equiv_{m}c$
>Dokaz:
>$a\cdot b\equiv_{m}a \cdot c\ \ \Rightarrow\ \ m\,|\,(a\cdot b-a\cdot c)\ \ \Rightarrow$
>$\begin{align}\Rightarrow m\,|\,a\cdot(b-c) \\ \mathrm{NZD}(m,\,a) = 1\end{align}\ \ \Rightarrow\ \ m\,|\,(b-c) \ \ \Rightarrow \ \ b\equiv_{m}c$

$\:$
### 5.5.1 Jednačina oblika $a\,x\equiv_{m}b$
$a\,x\equiv_{m}b\ \ \Leftrightarrow\ \ m\,|\,(a\,x-b) \ \ \Leftrightarrow\ \ \exists y\in \mathbb{Z}\ : \ a\,x-b=m\,(-y)$
$a\,x+m\,y=b\:$ — Diofantova jednačina, koja ima rešenja ako $\mathrm{NZD}(a,\,m)\,|\,b$

$d:=\mathrm{NZD}(a,\, m);\ a'=\frac{a}{d};\ b'=\frac{b}{d};\ m'=\frac{m}{d}$
Možemo podeliti diofantovu jednačinu sa $d$:
$a'\,x+m'\,y=b'\ \ \Leftrightarrow\ \ a'\,x\equiv_{m'}b'\:$ (ima isti skup rešenja kao i polazna jednačina)
>I metoda:
>Rešavanjem diofantove jednačine $a'\,x+m'\,y=b'$ dobijamo rešenje u obliku $x = x_{0}+m'\,t,\quad \forall t\in \mathbb{Z}$
>
> II metoda:
> U $\mathbb{Z}_{m'}$ prebrojavanjem treba naći $x_0$ koji zadovoljava jednačinu $a'\,x_{0}\equiv_{m'}b'$
> Tada rešenje je $x = x_{0}+m'\,t,\quad\forall t\in \mathbb{Z}$

>Rešenja iz $\mathbb{Z}_{m}$: $\ \ d$ rešenja
>(Ako je $x_0$  rešenje iz $\mathbb{Z}_{m'}$ onda rešenja iz $\mathbb{Z}_{m}$ su
>$x_{0},\,x_{0}+m',\,x_{0}+2m',\,\dots,\,x_{0}+(d-1)m'$)

![[kongr primer 1.png]]

### 5.5.2 Kineska teorema o ostacima
Teorema. Ako $\forall i\ne j\quad a_{i} \equiv_{\mathrm{NZD}(m_{i},\,m_{j})}a_{j}$ onda sistem jednačina 
$$
\begin{cases} x\equiv_{m_{1}}a_{1}\\
x\equiv_{m_{2}}a_{2} \\
\dots \\
x\equiv_{m_{k}}a_{k}\\ \end{cases}
$$ 
ima rešenja.
Ako je $\overline x$ je jedno rešenje sistema onda su sva rešenja oblika $x = \overline x+\mathrm{NZS}(m_{1},\,m_{2},\,\dots,\,m_{k})\,t,\quad t\in \mathbb{Z}$

![[kineska teorema.png]]

>Rešavanje sistema:
>Rešavamo prvu jednačinu dobijamo $x = x_{0}+m_{1}\,t$
>Ubacujemo to u drugu jednačinu, rešavamo po $t$ dobijamo: $t = t_0+m_{2}'\,s$, gde je $m_2'=\frac{\mathrm{NZS}(m_{1},\, m_{2})}{m_{1}}$ \*
>Zatim vračamo: $x = x_{0}+m_{1}\,t = x_{0}+m_{1}\,(t_0+m_{2}'\,s)=\dots$
>Ubacujemo to u treću jednačinu, rešavamo po $s$ dobijamo: $s = s_0+m_{3}'\,u$, gde je $m_3'=\frac{\mathrm{NZS}(m_{1},\, m_{2},\,m_{3})}{\mathrm{NZS}(m_{1},\,m_{2})}$ \*
>Zatim vračamo: $x = x_{0}+m_{1}\,(t_0+m_{2}'\,(s_0+m_{3}'\,u))=\dots$
>i tako dalje, dok nećemo dobiti
>$x=\overline x+\mathrm{NZS}(m_{1},\,m_{2},\,\dots,\,m_{k})\,v$
>
>(\* ne morate da učite ove razlomke, te brojevi $m'_{k}$ se dobijaju sami, rešavanjem kongruencija)

![[kongr primer 2.png]]
![[kongr primer 3.png]] 

### 5.5.3 Ojlerova teorema
**Def**. Neka je $n>1$ prirodan broj, tada skup $\Phi(n)=\{ k\in \mathbb{N}\ | \ 1\leqslant k< n \ \ \mathrm{i}\ \ \mathrm{NZD}(k,\,n)=1\}$ je **Ojlerov skup**.
$\varphi (n) = |\Phi(n)|$ je **Ojlerova funkcija**.
>Primer:
>$\Phi(3) = \{ 1,\,2 \}\quad\quad\quad\ \ \varphi(3)=2$
>$\Phi(4) = \{ 1,\,3 \}\quad\quad\quad\ \ \varphi(4)=2$
>$\Phi(5) = \{ 1,\,2\,3\,4 \}\quad\quad\,\varphi(5)=4$
>$\Phi(6) = \{ 1,\,5 \}\quad\quad\quad\ \ \varphi(6)=2$

Teorema. $m,\,n>1,\ \ \mathrm{NZD}(m,\,n)=1\ \ \Rightarrow\ \ \varphi(m\,n)=\varphi(m)\,\varphi(n)$


Stav. $p$ je prost, tada $\varphi(p^{k})=p^{k}-p^{k-1}$
![[ojlerova fja prostog broja.png]]

Iz osnovne teoreme aritmetike: $n = p_{1}^{\alpha_{1}}\,p_{2}^{\alpha_{2}}\,\dots\,p_{k}^{\alpha_{k}}$
Tada $\varphi(n)=\varphi(p_{1}^{\alpha_{1}})\,\varphi(p_{2}^{\alpha_{2}})\,\dots\,\varphi(p_{k}^{\alpha_{k}})=$
$= (p_{1}^{\alpha_{1}}-p_{1}^{\alpha_{1}-1})\,(p_{2}^{\alpha_{2}}-p_{2}^{\alpha_{2}-1})\,\dots\,(p_{k}^{\alpha_{k}}-p_{k}^{\alpha_{k}-1})=$
$\begin{align}=n\,\bigg(1-\frac{1}{p_{1}}\bigg)\,\bigg(1-\frac{1}{p_{2}}\bigg)\,\dots\,\bigg(1-\frac{1}{p_{k}}\bigg)\end{align}$

Teorema (Ojlerova). $n > 1\:$ i $\:a$ su prirodni brojevi i $\mathrm{NZD}(a,\,n)=1$.
Tada $a^{\varphi(n)}\equiv_{n}1$
![[ojlevova teorema.png]]

Posledica (mala Fermaova teorema). $a\in \mathbb{N}$,$\ p$ je prost, $p\nmid a$. 
Tada $a^{p-1}\equiv_{p}1$

![[kongr primer 4.png]]

### 5.5.4 Vilsonova teorema
Teorema. $p$ je prost akko $(p-1)!\equiv_{p}-1$

# 1 Teorija skupova (nastavak)
## 1.4 Prebrojivost. Kardinalnost
$\lvert A \rvert$ — kardinalnost skupa $A$.

$\lvert A \rvert \in \mathbb{N}\quad \Leftrightarrow \quad A$ je konačan skup,
inače je beskonačan

**Teorema**. Skup $X$ je beskonačan ako postoji pravi podskup $Y$ $\ (Y \subset X)$, takav da su $X$ i $Y$ u bijekciji.

Teorema. Skup prirodnih brojeva je beskonačan.
![[teorema. N je beskonačan.png]]

**Def**.
- Skup je **prebrojiv** ako je u bijekciji sa $\mathbb{N}$.
- Skup je **najviše prebrojiv** ako je konačan ili prebrojiv.
- Skup je **neprebrojiv** ako nije najviše prebrojiv.

Teorema.  $\mathbb{N}$,  $\mathbb{Z}$, svaki njihov beskonačan podskup, $\mathbb{N}^n$, $\ \mathbb{Z}^n$, $\:$ $\mathbb{Q} \subseteq \mathbb{Z} \times \mathbb{N}$ su prebrojivi skupovi.

Stav. $\exists f: \ \ X \stackrel{_{na}}{\to} \mathbb{N} \quad \Rightarrow \quad X$ je najviše prebrojiv.
$\quad \quad \ \exists f: \ \ \mathbb{N} \stackrel{_{1-1}}{\to} X \quad \Rightarrow \quad X$ je najviše prebrojiv.

![[prebrojivost primer.png]]

Teorema.  $\mathbb{R}$ je neprebrojiv.
![[teorema. R je neprebrojiv.png]]

**Def**. $\lvert A \rvert \leq \lvert B \rvert \;$ ($A$ je je kardinalnosti manje ili jednako od $B$) ako $\ \exists f: \ \ A \stackrel{_{1-1}}{\to} B$

**Def**. $\lvert A \rvert = \lvert B \rvert \;$ ($A$ i $B$ su iste kardinalnosti) ako postoji bijekcija između $A$ i $B$.

**Def**. $\lvert A \rvert < \lvert B \rvert \;$ ($A$ je je kardinalnosti strogo manje od $B$) ako $\lvert A \rvert \leq \lvert B \rvert \;$ i $\; \lvert A \rvert \ne \lvert B \rvert$

Važi:
- $\lvert A \rvert = \lvert B \rvert \quad \Rightarrow \quad \lvert A \rvert \leq \lvert B \rvert \;$ i $\; \lvert B \rvert \leq \lvert A \rvert \;$
- $\lvert A \rvert \leq \lvert B \rvert \;$ i $\; \lvert B \rvert \leq \lvert C \rvert \quad \Rightarrow \quad \lvert A \rvert \leq \lvert C \rvert$
- $\lvert A \rvert = \lvert B \rvert \;$ i $\; \lvert B \rvert = \lvert C \rvert \quad \Rightarrow \quad \lvert A \rvert = \lvert C \rvert$

**Teorema (Kantor-Bernštajn)**. 
$\lvert A \rvert \leq \lvert B \rvert \;$ i $\; \lvert B \rvert \leq \lvert A \rvert \quad \Rightarrow \quad \lvert A \rvert = \lvert B \rvert$

| Skup                           | Kardinalnost           |
| ------------------------------ | ---------------------- |
| Konačan                        | Broj elemenata         |
| Prebrojiv                      | $\aleph_0$ — alef nula |
| $\mathbb{R}$,  $\mathcal{P}(\mathbb{N})$ | $c$ — moć kontinuuma   |

Ako je $n \in \mathbb{N}$, tada važi $\ \ n < \aleph_0 < c$

# 6 Logika
## 6.1 Iskazna logika
Iskazi - $p, q$ 
Tačno - 1 ili $\top$
Netačno - 0 ili $\bot$

$\mathcal{P}$ - skup iskaznih slova.
**Iskazna slova** menjaju vrednost u zavisnosti od valuacije.
**Konstante** uvek imaju istu vrednost.

**Def.** Logičke operacije
1. **Negacija** iskaza $p$ je
   $\neg p$ :

| $p$ | $\neg p$ |
| :-: | :------: |
|  0  |    1     |
|  1  |    0     |

2. **Konjunkcija** iskaza $p$ i $q$ je
   $p \land q$ :

| $p$ | $q$ | $p \land q$ |
| :-: | :-: | :---------: |
|  0  |  0  |      0      |
|  0  |  1  |      0      |
|  1  |  0  |      0      |
|  1  |  1  |      1      |
3. **Disjunkcija** iskaza $p$ i $q$ je
   $p \lor q$ :

| $p$ | $q$ | $p \lor q$ |
| :-: | :-: | :--------: |
|  0  |  0  |     0      |
|  0  |  1  |     1      |
|  1  |  0  |     1      |
|  1  |  1  |     1      |
4. **Eksluzivna disjunkcija** iskaza $p$ i $q$ je
   $p \underline{\vee} q$ :

| $p$ | $q$ | $p \underline{\vee} q$ |
| :-: | :-: | :--------------------: |
|  0  |  0  |           0            |
|  0  |  1  |           1            |
|  1  |  0  |           1            |
|  1  |  1  |           0            |
5. **Implikacija** iskaza $p$ i $q$ je
   $p \Rightarrow q$ :

| $p$ | $q$ | $p \Rightarrow q$ |
| :-: | :-: | :---------------: |
|  0  |  0  |         1         |
|  0  |  1  |         1         |
|  1  |  0  |         0         |
|  1  |  1  |         1         |
6. **Ekvivalencija** iskaza $p$ i $q$ je
   $p \Leftrightarrow q$ :

| $p$ | $q$ | $p \Leftrightarrow q$ |
| :-: | :-: | :-------------------: |
|  0  |  0  |           1           |
|  0  |  1  |           0           |
|  1  |  0  |           0           |
|  1  |  1  |           1           |



Prioritet logičkih operacija: $\neg$, $\lor$ i $\land$, $\Rightarrow$ i $\Leftrightarrow$ i $\underline{\vee}$;

**Def.** Iskazna formula:
1. Logičke konstante i iskazna slova su skazne formule
2. Ako su $A$ i $B$  iskazne formule, tada su $\neg A$, $A \lor B$, $A \land B$, $A \Rightarrow B$, $A \Leftrightarrow B$, $A \underline{\vee} B$ iskazne formule.
3. Iskazne formule se mogu dobiti jedino konačnim primenom 1. i 2.

$For$ - skup svih formula

### 6.1.1 Valuacija
**Def**. Valuacija je funkcija iz $\mathcal{P}$ u {0, 1}: $\quad v: \quad \mathcal{P} \to \{0, 1\}$
Preslikava svako iskazno slovo u 0 ili 1.

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
### 6.1.2 Formule
**Def.** Formula $A$ je 
1. **tautologija** ako važi $v(A) = 1$ za svaku valuaciju $v$.
2. **kontradikcija** ako važi $v(A) = 0$ za svaku valuaciju $v$.
1. **zadovoljiva** ako važi $v(A) = 1$ za neku valuaciju $v$. 
2. **poreciva** ako važi $v(A) = 0$ za neku valuaciju $v$.

**Def**. Iskazne formule $A$ i $B$ su **logički ekvivalentne** ($A \equiv B$) ako za svaku valuaciju važi $v(A)=v(B)$ 
(tj. $A \Leftrightarrow B$ je tautologija).

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

## 6.2 Bulove algebre
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

Is aksioma 1.-5. izvode se sledeći zakoni:

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

Dokazi:
![[dokazi zakona bulovih algebri.png]]
### 6.2.1 Relacija poretka na bulovoj algebri
$x \leqslant y \quad$ akko $\quad x \land y = x$

(R) $\quad x \land x = x\quad \Rightarrow \quad x \leqslant x$ 
(AS) $\quad x \leqslant y \quad\quad$ i $\quad\quad y \leqslant x$
$\quad\quad\quad x \land y = x \quad\quad\quad  y \land x = y\quad$
$\quad\quad\quad\quad\quad\quad\quad  x = y$
(T) $\quad x \leqslant y \quad\quad$ i $\quad\quad y \leqslant z$
$\quad(1)\: x \land y = x \quad\quad (2) \:  y \land z = y\quad$

$\quad\quad x  \stackrel{(1)}{=} x \land y \stackrel{(2)}{=} x \land y \land z \stackrel{(1)}{=} x \land z \quad \Rightarrow \quad x \leqslant z$ 

![[stav. relacija poretka u bulovim algebrama.png]]

### 6.2.2 Princip dualnosti
$\Phi(B, \: \lor, \: \land, \: ', \: \mathbb{0}, \: \mathbb{1})$ - iskaz u bulovoj algebri $B$.
Tada je $\Phi(B, \: \lor, \: \land, \: ', \: \mathbb{0}, \: \mathbb{1})$ tačno akko je $\Phi(B, \: \land, \: \lor, \: ', \: \mathbb{1}, \: \mathbb{0})$ tačno.
$\Phi(B, \: \land, \: \lor, \: ', \: \mathbb{1}, \: \mathbb{0})$ je **dualan** prvom iskazu.
### 6.2.3 Primeri bulovih algebri
1. Algebra iskazne logike: $B = \{0,1 \}$,  $\lor$, $\land$, $\neg$
Bulova algebra — $(\{0, 1\},\lor,\land,\neg,0,1)$
2. Algebra karakterističnih funkcija na skupu $X$:
$X \ne \varnothing$
$B = \{ \chi_{A} \:|\: A \subseteq X\}$
$\chi_{A} \lor \chi_{B} := \chi_{A \cup B}$
$\chi_{A} \land \chi_{B} := \chi_{A \cap B}$
$\chi_{A}\,' := \chi_{X \setminus A}$
$1 := \chi_{\varnothing}$
$0 := \chi_{X}$
Bulova algebra — $(B,\lor,\land,',\chi_{\varnothing},\chi_{X})$


![[primeri bulovih algebri.png]]

## 6.3 Predikatska logika
![[predik1.png]]![[predik2.png]]![[predik3.png]]![[predik4.png]]![[predik5.png]]![[predik6.png]]