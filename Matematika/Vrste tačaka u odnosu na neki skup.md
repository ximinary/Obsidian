#fax #math #a1 [deo [[Realni brojevi|poglavlja "realni brojevi"]]]
$\:$
[[Okolina tačke]]

**Def**. Neka je $A$ neki podskup $\mathbb{R}$. Tada
- $a\in \mathbb{R}$ je **unutrašnja** tačka skupa $A$ ako
   $\exists \varepsilon>0\ \ :\ \ \mathrm{O}_{\varepsilon}(a)\subseteq A$
  $\mathrm{int\ }A$ je skup svih unutrašnjih tačaka skupa $A.$
  $\:$
- $a\in \overline{\mathbb{R}}$ je **spoljašnja** tačka skupa $A$ ako
  $\exists \varepsilon>0\ \ :\ \ \mathrm{O}_{\varepsilon}(a)\subseteq \mathbb{R}\setminus A$
  $\mathrm{ext\ }A$ je skup svih spoljašnjih tačaka skupa $A.$
  $\:$
- $a\in\overline{\mathbb{R}}$ je **granična**  tačka skupa $A$ ako
  $\forall \varepsilon>0\quad \begin{cases}\mathrm{O}_{\varepsilon}(a)\cap A\ne\varnothing\\\mathrm{O}_{\varepsilon}(a)\cap (\mathbb{R}\setminus A)\ne\varnothing\end{cases}$
  $\partial\, A$ je skup svih graničnih tačaka skupa $A.$
  $\:$

$\mathrm{int\ }A,\ \mathrm{ext\ }A,\ \partial\, A$ su disjunktni i njihova unija daje $\overline{\mathbb{R}}$.
$\mathrm{int\ }A\subseteq A$
$\mathrm{ext\ }A\subseteq (\mathbb{R}\setminus A)$
$\partial\, A = \Big(A\setminus(\mathrm{int\ }A)\Big)\cup\Big((\mathbb{R}\setminus A)\setminus(\mathrm{ext\ }A)\Big)$
  ---
- $a\in \overline{\mathbb{R}}$ je **tačka nagomilavanja** skupa A ako $\forall\varepsilon>0\quad \mathring{\mathrm{O}}_{\varepsilon}(a)\cap A\ne \varnothing$
$A'$ je skup svih tačaka nagomilavanja skupa $A.$
  $\:$ ^3de7f2
-  $a\in \mathbb{R}$ je **izolovana** tačka skupa $A$ ako
  $a\in A\setminus A'\quad\Leftrightarrow\quad\exists\varepsilon>0\ \ :\ \ \mathrm{O}_{\varepsilon}(a)\cap A=\{ a \}$
  $\:$
  -  $a\in \mathbb{R}$ je **atherentna** tačaka skupa $A$ ako
  $a\in A\cup A'=A\cup\partial\, A\quad\Leftrightarrow\quad\forall\varepsilon>0\ \ :\ \ \mathrm{O}_{\varepsilon}(a)\cap A\ne\varnothing$
  $\overline{A}$ je skup svih atherentnih tačaka (**zatvorenje**) skupa $A.$

Atherentna tačka je ili tačka nagomilavanja ili granična tačka.

---
![[analiza1_0_tačke.png]]