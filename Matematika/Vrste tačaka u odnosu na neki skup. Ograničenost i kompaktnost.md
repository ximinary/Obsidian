#fax #math #a1 #a3 [deo [[Metrika|poglavlja "metrika"]]]
$\:$
[[Okolina tačke#Okolina u proizvoljnom Metrika metričkom prostoru|Okolina tačke]]

**Def**. Neka je $(X,\,\mathrm{d})$ [[Metrika|metrički]] prostor i neka $A\subseteq X$. Tada
- $a\in X$ je **unutrašnja** tačka skupa $A$ ako
   $\exists \mathrm{O}(a)\ \ :\ \ \mathrm{O}(a)\subseteq A$
  $\mathrm{int\ }A$ je skup svih unutrašnjih tačaka skupa $A.$
  $\:$
- $a\in X$ je **spoljašnja** tačka skupa $A$ ako
  $\exists \mathrm{O}(a)\ \ :\ \ \mathrm{O}(a)\subseteq X\setminus A$
  $\mathrm{ext\ }A$ je skup svih spoljašnjih tačaka skupa $A.$
  $\:$
- $a\in X$ je **granična** (rubna)  tačka skupa $A$ ako
  $\forall \mathrm{O}(a)\quad \begin{cases}\mathrm{O}(a)\cap A\ne\varnothing\\\mathrm{O}(a)\cap (X\setminus A)\ne\varnothing\end{cases}$
  $\partial\, A$ je skup svih graničnih tačaka (**rub**) skupa $A.$
  $\:$ ^1ecb22


$\mathrm{int\ }A,\ \mathrm{ext\ }A,\ \partial\, A$ su disjunktni i njihova unija daje $X$.
$\mathrm{int\ }A\subseteq A$
$\mathrm{ext\ }A\subseteq (X\setminus A)$
$\partial\, A = \Big(A\setminus(\mathrm{int\ }A)\Big)\cup\Big((X\setminus A)\setminus(\mathrm{ext\ }A)\Big)$

$\:$
**Def**. Ako $\partial\,A\subseteq A$ onda je $A$ **zatvoren** skup.
**Def**. Ako $\partial\,A\subseteq X\setminus A$ onda je $A$ **otvoren** skup. ^0ce91a

  ---
- $a\in\overline{X}$ je **tačka nagomilavanja** skupa $A$ ako $\forall\mathring{\mathrm{O}}(a)\quad \mathring{\mathrm{O}}(a)\cap A\ne \varnothing$
$A'$ je skup svih tačaka nagomilavanja skupa $A.$
  $\:$ ^3de7f2
-  $a\in X$ je **izolovana** tačka skupa $A$ ako
  $a\in A\setminus A'\quad\Leftrightarrow\quad\exists\mathrm{O}(a)\ \ :\ \ \mathrm{O}(a)\cap A=\{ a \}$
  $\:$
  -  $a\in\overline{X}$ je **atherentna** tačaka skupa $A$ ako $a\in A\cup A'=\partial\, A\cup A'\quad\Leftrightarrow\quad\forall\varepsilon>0\ \ :\ \ \mathrm{O}_{\varepsilon}(a)\cap A\ne\varnothing$
  $\overline{A}$ je skup svih atherentnih tačaka (**zatvorenje**) skupa $A$


> Napomena:
> za $X=\mathbb{R}$ definišimo $\overline{X}=\overline{\mathbb{R}}=\mathbb{R\cup\{-\infty,\,+\infty\}}$
> za ostale prostore radi jednostavnosti uzimamo $\overline{X}=X$

---
![[analiza1_0_vrste_tacaka.png]]

### Ograničenost i kompaktnost
**Def**. Skup $A\subseteq X$ je **ograničen** ako $\exists\varepsilon>0\ \ :\ \ A\subseteq\mathrm{O}_{\varepsilon}(0)$

**Def**. Skup $A\subseteq X$ je **kompaktan** ako je zatvoren i ograničen. ^3969f8