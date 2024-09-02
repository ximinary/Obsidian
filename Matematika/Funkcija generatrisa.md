#fax #math #ds2 [deo [[Kombinatorika|kombinatorike]]]
$\:$

$(a_{n})=(a_{0},\,a_{1},\,a_{2},\,\dots,\,a_{k},\,\dots)$ — [[Niz brojeva|niz]]
$\begin{align}\sum\limits_{i=0}^{\infty}a_{i}\,x^{i}=a_{0}+a_{1}\,x+a_{2}\,x^{2}+\dots+a_{k}\,x^{k}+\dots\end{align}$ — [[Red|red]]
Ako red konvergira, $\exists$ funkcija generatrisa $A(x)=\begin{align}\sum\limits_{i=0}^{\infty}a_{i}\end{align}$ niza $(a_{n})$
$(a_{n})\overset{\mathrm{jednoznačna}}{\overset{\mathrm{veza}}\longleftrightarrow} A(x)$
$\:$ 

Za $|x|<1$ važi
$(1,\,1,\,\dots,\,1,\,\dots)\ \longleftrightarrow\ 1+x+\dots+x^{k}+\dots=\begin{align}\frac{1}{1-x}\end{align}\quad$ ([[Aritmetička i geometrijska progresija#^adeab1|*]])

### Određivanje funkcija generatrisa
Neka 
$(a_{n})=(a_{0},\,a_{1},\,\dots,\,a_{k},\,\dots)\ \longleftrightarrow\ A(x)$
$(b_{n})=(b_{0},\,b_{1},\,\dots,\,b_{k},\,\dots)\ \longleftrightarrow\ B(x)$
Tada važi:
- sabiranje:
  $(a_{n})+(b_{n})=(a_{0}+b_{0},\,a_{1}+b_{1},\,\dots,\,a_{k}+b_{k},\, \dots) \ \longleftrightarrow$
  $\longleftrightarrow\ (a_{0}+b_{0})+(a_{1}+b_{1})x+\dots+(a_{k}+b_{k})x^{k}+\dots=$
  $= (a_{0}+a_{1}\,x+\dots+a_{k}\,x^{k}+\dots)+(b_{0}+b_{1}\,x+\dots+b_{k}\,b^{k}+\dots) =$
  $= A(x)+B(x)$
  $\:$
- množenje skalarom:
  $c\cdot(a_{n})=(c\,a_{0},\,c\,a_{1},\,\dots,\,c\,a_{k},\,\dots)\ \longleftrightarrow$
  $\longleftrightarrow\ c\,a_{0}+c\,a_{1}\,x+\dots+c\,a_{k}\,x^{k}+\dots=c\cdot A(x)$
  $\:$
- pomeranje za $k$ mesta ulevo:
  $\begin{align}(a_{k},\,a_{k+1},\,a_{k+2},\,\dots)\ \longleftrightarrow\ \frac{A(x)- (a_{0}+a_{1}\,x+\dots+a_{k}\,x^{k})}{x^{k}}\end{align}$
  $\:$
- pomeranje za $k$ mesta udesno: 
  $(\underbrace{0,\,0,\,\dots,\,0}_{k},\,a_{0},\,a_{1},\,\dots,\,a_{k},\,\dots)\ \longleftrightarrow\ x^{k}A(x)$
  $\:$
- zamena $x$ sa $c\,x$ u FG:
  $A(c\,x)\ \longleftrightarrow\ (a_{0},\, c\,a_{1},\,c^{2}\,a_{2},\,\dots,\,c^{k}\,a_{k},\,\dots)$
  - specijalno: $A(-x)\ \longleftrightarrow\ (a_{0},\,-a_{1},\,a_{2},\,-a_{3},\,\dots)$
  $\:$
- zamena $x$ sa $x^{n}$ u FG:
   $A(x^{k})=a_{0}+a_{1}\,x^{k}+a_{2}\,x^{2k}+\dots+a_{k}\,x^{kk}+\dots\ \longleftrightarrow$$\longleftrightarrow\ (a_{0},\,\underbrace{0,\,0,\,\dots,\,0}_{k-1},\,a_{1},\,\underbrace{0,\,0,\,\dots,\,0}_{k-1},\,a_{2},\,\dots)$
  $\:$
- diferenciranje FG:  
  $A'(x)=a_{1}+2a_{2}\,x+3a_{3}\,x^{2}+\dots+ka_{k}\,x^{k-1}+\dots\ \longleftrightarrow$
 $\longleftrightarrow\ (a_{1},\,2a_{2},\,3a_{3},\,\dots,\, ka^{k},\dots)$
  $\:$
- integracija FG:
 $\begin{align}\int A(x) \, dx=a_{0}\,x+\frac{a_{1}\,x^{2}}{2}+\frac{a_{2}\,x^{3}}{3}+\dots+\frac{a_{k}\,x^{k+1}}{k+1}+\dots\ \longleftrightarrow\end{align}$
 $\begin{align}\longleftrightarrow\ \bigg(0,\,a_{0},\,\frac{a_{1}}{2},\,\frac{a_{2}}{3},\,\dots,\,\frac{a_{k}}{k+1},\,\dots\bigg)\end{align}$

[[FGprimer1.png|Primer 1]]
[[FGprimer2.png|Primer 2]]
[[FGprimer3.png|Primer 3]]