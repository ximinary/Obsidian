#fax #math #ds1 #a1 [deo [[Relacija|poglavlja "relacija"]]]
$\:$

**Def**. [Binarna relacija](Relacija#Binarna%20relacija) je relacija **strogog** (parcijalnog) **poretka** ako je (AR), (S) i (T). Oznaka: $\prec$.
**Def**. [Binarna relacija](Relacija#Binarna%20relacija) je relacija **nestrogog** (parcijalnog) **poretka** ako je (R), (S) i (T).  Oznaka: $\preceq$.

**Def**. Ako je u [[Teorija skupova|skupu]] uvedena relacija parcijalnog poretka, tada je taj skup **uređen** ili se zove **poset**.

**Def**. $a,\ b \in A \:$ su uporedivi ako važi $a\preceq b\:$ ili $\:b\preceq a$

**Def**. Ako su u skupu svaka dva elementa uporediva, tada je taj skup **totalno uređen** i relacija je **totalnog** (umesto da bude parcijalnog) poretka.

**Def**. Podskup skupa $A$ je **lanac** ako su u njemu svaka dva elementa uporediva.
**Def**. Podskup skupa $A$ je **antilanac** ako u njemu svaka dva elementa nisu uporediva.
Neki podskup može biti ni lanac ni antilanac.
### Primer
$X = \{ a, \ b, \ c\}$
$\mathcal{P}(X) = \{\varnothing, \ \{ a\},\ \{b\},\ \{c\}, \ \{a,\ b\}, \ \{a,\ c\}, \ \{b,\ c\},\ \{ a, \ b, \ c\}\}$
Relacija $\subseteq$ u skupu $\mathcal{P}(X)$
- (R) $\forall A \in \mathcal{P}(X)\ \ \ A\subseteq A$
(AS) $\forall A, \ B \in \mathcal{P}(X)\ \ \ (A\subseteq B, \ B\subseteq A) \ \ \ \Rightarrow \ \ \ A=B$
(T) $\forall A, \ B, \ C \in \mathcal{P}(X)\ \ \ (A\subseteq B, \ B\subseteq C) \ \ \ \Rightarrow \ \ \ A\subseteq C$
jeste relacija nestrogog poretka.
- $\{a,\ b\}$ i $\{a,\ c\}$ nisu uporedivi $\ \ \ \Rightarrow \ \ \ \mathcal{P}(X)$  nije totalno uređen.
- Lanac: $\varnothing \subseteq \{ a\}\subseteq \{ a,\ b\}\subseteq \{ a,\ b, \ c\}$
- Antilanac: $\{\{ a\},\ \{b\}, \ \{c\}\}$ - svaka dva nisu uporediva

Haseov dijagram:
![[haseov dijagram primer 1.png]]
Svaka linija predstavlja relaciju između dva elementa tako da (donji element) $\!\preceq\!$ (gornji element). Ali relacije kao na primer $\{a\} \subseteq \{a,\ b,\ c\}$ se ne označavaju jer "prolaze" kroz drugi element $\{a\} \subseteq \{a,\ b\} \subseteq \{a,\ b,\ c\}$

### Najmanji, najveći, minimalni, maksimalni
**Def**. Neka je $\preceq$ relacija nestrogog parcijalnog poretka u [[Teorija skupova|skupu]] $A$, $B \subseteq A$. Tada:
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

[Teorema](najminmaks%20teorema.png). Ako $\exists a \in B \:$ najmanji (najveći) element, tada
1. $a$ je jedinstven najmanji (najveći) element
2. $a$ je jedinstven minimalni (maksimalni) element

Napomena: U totalno uređenom skupu pojmove najmanji i minimalni, najveći i maksimalni se poklapaju.

### Donje i gornje ograničenje. Infinum i supremum
**Def**. Neka je $\preceq$ relacija nestrogog parcijalnog poretka u [[Teorija skupova|skupu]] $A$, $B \subseteq A$. Tada:
- $a \in A$ je **donje ograničenje** (minoranta) skupa $B$ ako $\ \forall x \in B \ \ \ a \preceq x$
- $B$ je **ograničen odozdo** ako takvo $a$ postoji
- Skup donjih ograničenja je $B^{\succeq} = \{a \in A\ | \ a\ \textrm{je donje ograničenje skupa }B\}$
- Najveće donje ograničenje skupa $B$ ako postoji zove se **infinum**: $\inf(B)$
$\:$
- $a \in A$ je **gornje ograničenje** (majoranta) skupa $B$ ako $\ \forall x \in B \ \ \ x \preceq a$
- $B$ je **ograničen odozgo** ako takvo $a$ postoji
- Skup gornjih ograničenja je $B^{\preceq} = \{a \in A\ | \ a\ \textrm{je gornje ograničenje skupa } B\}$
- Najmanje gornje ograničenje skupa $B$ ako postoji zove se **supremum**: $\sup(B)$
$\:$
- $B$ je **ograničen** ako je ograničen odozdo i odozgo.

>Primer:
$B = [0,\ 1) \in \mathbb{R}$
$(-\infty, \ 0]$ - skup donjih ograničenja; $\inf(B)=0$
$[1, \ +\infty)$ - skup gornjih ograničenja; $\sup(B)=1$

---
### Relacija $\leqslant$ u skupu $\mathbb{R}$
Stav.
- $a$ je minimum (najmanji el) skupa $B$ akko je $a \in A \cap A^{\leqslant}$
- $a$ je maksimum (najveći el) skupa $B$ akko je $a \in A \cap A^{\geqslant}$

Stav.
- $\exists \min B  =a\ \ \Rightarrow\ \ \exists \inf B = a$
- $\exists \max B  =a\ \ \Rightarrow\ \ \exists \sup B = a$

> Dokaz za $\sup$, za $\inf$ analagno
> 1. $a=\max B \ \ \Rightarrow\  \ a\in B\cap B^{\leqslant}\ \ \Rightarrow\ \ a\in B^{\leqslant}\ \ \Rightarrow\ \ a$ je majoranta
> 2. pps $a$ nije najmanja majoranta
> $\exists a_0 < a$, gde je $a_0$ majoranta (tj. $\forall x \in B \ \ a_0\geqslant x$)
> $a \in B\ \ \Rightarrow\ \ a\leqslant a_0 < a\ \:$ kontradikcija $\ \ \Rightarrow\ \ a = \sup B$

Stav.
- $\inf B \in B\ \ \Rightarrow\ \ \exists\min B=\inf B$
- $\inf B \notin B\ \ \Rightarrow\ \ \nexists\min B$
- $\sup B \in B\ \ \Rightarrow\ \ \exists\max B=\sup B$
- $\sup B \notin B\ \ \Rightarrow\ \ \nexists\max B$

Dokazivanje da je $a$ supremum (infinum) skupa $B$:
1) $a$ je majoranta: $\ \forall x \in B \ \ \ x \leqslant a$
2)  $\:$
	- Ako $a \in B\ \ \Rightarrow\ \ a = \max B\ \ \Rightarrow\ \ a = \sup B$ 
	- Ako $a \notin B$, treba pokazati
	  $\forall\varepsilon>0 \ \ \exists x\in B\ : \ a - \varepsilon < x$
	  (Za proizvoljno $\varepsilon$ naći $x$ koristeći *[[Realni brojevi#Arhimedovo svojstvo ($ mathbb{R}$)|(ARH)]]*)
 