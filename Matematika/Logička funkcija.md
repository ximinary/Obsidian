#fax #math #ds1 [deo [[Iskazna logika|iskazne logike]]]
$\:$

**Def**. Logička funkcija reda $n$ je [[funkcija]] $f:\ \{ 0,\,1 \}^{n}\to\{0,\,1\}.$
$f(\underbrace{x_{1},\,x_{2},\,\dots,\,\,x_{n}}_{\text{ulazni argumenti}})=\underbrace y _{\text{izlaz (vrednost)}},\quad\quad x_{1},\,x_{2},\,\dots,\,x_{n},\,y\in\{ 0,\,1 \}$

Svaka funkcija ima $2^{n}$ različitih ulaza.
Odakle ima $2^{2^{n}}$ različitih funkcija.

### Funkcije reda 0 (bez ulaza)
$2^{2^{0}}=2:\quad f\equiv1,\ f\equiv0$

### Funkcije reda 1
$2^{2^{1}}=4:\quad \underset{\text{nula-fja}}{f(x)=0},\ \underset{\text{jedinična fja}}{f(x)=1},\ \underset{\text{identiteta}}{f(x)=x},\ \underset{\text{negacija}}{f(x)=\overline x}$

### Funkcije reda 2
$2^{2^{2}}=16:$

$
\begin{array}{|c|c|} \hline
f(x,\,y)=0 & \text{nula-funkcija} \\ \hline
f(x,\,y)=1 & \text{jedinična funkcija} \\ \hline
f(x,\,y)=x & \text{prva projekcija} \\ \hline
f(x,\,y)=y & \text{druga projekcija} \\ \hline
f(x,\,y)=\overline x & \text{negacija prve projekcije} \\ \hline
f(x,\,y)=\overline y & \text{negacija druge projekcije} \\ \hline
f(x,\,y)=x\cdot y & \text{konjunkcija} \\ \hline
f(x,\,y)=x+y & \text{disjunkcija} \\ \hline
f(x,\,y)=\overline{x\cdot y} & \text{Šeferova funkcija } (x\uparrow y) \\ \hline
f(x,\,y)=\overline{x+y} & \text{Pirsova funkcija } (x\downarrow y) \\ \hline
f(x,\,y)=\overline x +y & \text{implikacija } x\Rightarrow y \\ \hline
f(x,\,y)=x+\overline y & \text{implikacija } y\Rightarrow x \\ \hline
f(x,\,y)=\overline x \cdot y & \overline{y\Rightarrow x} \\ \hline
f(x,\,y)=x\cdot\overline y & \overline{x\Rightarrow y} \\ \hline
f(x,\,y)=x\cdot \overline y + \overline x\cdot y & \text{ekskluzivna disjunkcija } (x\oplus y)\\ \hline
f(x,\,y)=x\cdot y + \overline x\cdot \overline y & \text{ekvivalencija } (x\Leftrightarrow y)\\ \hline
\end{array}
$