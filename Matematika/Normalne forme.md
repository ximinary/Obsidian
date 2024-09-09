#fax #math #ds1 #cs/ar [deo [[Iskazna logika|iskazne logike]] i [[Računarstvo|računarstva]]]
$\:$

[[Bulova algebra]]: $S(\,\cdot\,,\,+,\,\overline{\ },\,1,\,0)$
	Operacije su definisani sa [[Logičke operacije#^96b28f|∙]], [[Logičke operacije#^66b381|+]], [[Logičke operacije#^b24d81|‾]] i jesu u sledećem prioritetu $\overline{\ },\,\,\cdot\,,\,+.$

**Def**. **Literal**  je promenljiva ili negacija promenljivih. $(x,\, \overline{y},\,z)$

**Def**. **Elementarna konjunkcija** je konjunkcija literala. $(x\,\overline{y}\,z,\,\overline{u}\,\overline{v})$
**Def**. **Disjunktna normalna forma (DNF)** je disjunkcija elementarnih konjunkcija. $(x\,\overline{y}\,z+\overline{u}\,\overline{v}+x)$

**Def**. **Elementarna disjunkcija** je disjunkcija literala. $(x+\overline{y}+z,\,\overline{u}+\overline{v})$
**Def**. **Konjunktna normalna forma (KNF)** je konjunkcija elementarnih disjunkcija. $\big((x+\overline{y}+z)\,(\overline{u}+\overline{v})\,x\big)$

**Def**. **Savršena disjunkcija/konjunkcija** sadrži tačno po jedan literal za svaku promenljivu iz skup svih promenljivih.
**Def**. **Savršena DNF/KNF** — svi elementi disjunkcije/konjunkcije su savršeni.
$\:$

Za svaki izraz postoji ekvivalentni izraz u DNF/KNF.

Dobijanje DNF/KNF od nekog izraza:
1. Elemenisanje konstanti:
   $\overline 0=1\quad e\cdot0=0\quad e+0=e$
   $\overline 1=0\quad e\cdot1=e\quad e+1=1$
2. Negacije moraju da budu samo iznad promenljivih:
   $\overline{\overline x}=x\quad\begin{align}\overline{e_{1}+e_{2}}=\overline{e_{1}}\cdot\overline{e_{2}}\\\overline{e_{1}\cdot e_{2}}=\overline{e_{1}}+\overline{e_{2}}\end{align}$
3. DNF — izvlačenje disjunkcija: $e\cdot(e_{1}+e_{2})=e\cdot e_{1}+e\cdot e_{2}$
   DNF — izvlačenje konjunkcija: $e+e_{1}\cdot e_{2}=(e+e_{1})\,(e+e_{2})$
4. Uprošćavanje:
$\overline e \cdot e=0\quad\ \ e\cdot e=e$
$\overline e+e=1\quad e+e=e$
$e_{1}+e_{1}\cdot e_{2}=e_{1}\quad \Big(e_{1}\,(e_{1}+e_{2})=e_{1}\Big)$


### [[Logička funkcija|Logičke funkcije]] i DNF/KNF
![[LogičkeFjeIdnf_knf.png]]


---
[[Minimalizacija logičkih izraza]]

