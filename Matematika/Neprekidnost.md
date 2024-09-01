#fax #math #a1 [deo [[Analiza|analize]]]

[[Limes funkcije]]

**Def**. $f:\ D_{f}\to\mathbb{R}$ je **neprekidna** u tački $a\in D_{f}\ \  (f\,\mathcal{C}\,a)$ akko $\forall\varepsilon>0\quad\exists\delta>0\quad\forall x\in D_{f}\cap\mathrm{O}_{\delta}(a)\quad|f(x)-f(a)|<\varepsilon \ \ \Leftrightarrow$
$\Leftrightarrow \ \ \begin{cases} \mathrm{uvek\ važi,\quad\quad\quad\ ako}\ a\notin D_{f}'\\ \lim\limits_{ x \to a } f(x) = f(a),\ \mathrm{\ \ \!ako}\ a\in D_{f}'\end{cases}$

**Def**. $f:\ D_{f}\to\mathbb{R}$ je **neprekidna sleva**/**zdesna** u tački $a\in D_{f} \:$ akko $\forall\varepsilon>0\quad\exists\delta>0\quad\forall x\in D_{f}\cap\mathrm{O}_{\delta}^{-/+}(a)\quad|f(x)-f(a)|<\varepsilon \ \ \Leftrightarrow$
$\Leftrightarrow \ \ \begin{cases} \mathrm{uvek\ važi,\quad\quad\quad\quad\:\, ako}\ a\notin D_{f}'\\ \lim\limits_{ x \to a^{-/+} } f(x) = f(a),\ \mathrm{\ \ \!ako}\ a\in D_{f}'\end{cases}$

### [[Neprekidnost osnovnih funkcija]]

### Lokalna svojstva neprekidnosti
- [[Limes funkcije#^9993ac|1)]]  $f$ je neprekidna u $a\in D_{f} \ \ \Rightarrow$
$\Rightarrow\ \ \exists c>0,\, \delta>0\quad\forall x\in {\mathrm{O}}_{\delta}(a)\quad|f(x)|\leqslant c$
- [[Limes funkcije#^abfa5c|2)]] $f$ je neprekidna u $a\in D_{f}; f(a)>c\ \ (<c) \ \ \Rightarrow$
$\Rightarrow\ \ \exists\delta>0\quad\forall x\in D_{f}\cap {\mathrm{O}}_{\delta}(a)\quad f(x) >c\  (<c)$
- [[Limes funkcije#^2c8b48|3)]] $f$ i $g$ su neprekidni u $a\in D_{f} \ \ \Rightarrow$
	$|\quad$ [[Limes funkcije#^a79518|1.]] $f+g$ je neprekidna u $a$
	$|\quad$ [[Limes funkcije#^53cf78|2.]] $f\cdot g$ je neprekidna u $a$
	$|\quad$ [[Limes funkcije#^44b570|3.]] $\frac{f}{g}$ je neprekidna u $a$, ako $g(a)\ne0$
- [[analiza1_1_neprKompozicije.png|4)]] $f$ je neprekidna u $y_{0}=g(x_{0}),\ g$ je neprekidna u $x_{0} \ \ \Rightarrow$
$\Rightarrow\ \ f\!\circ\!g$ je neprekidna u $x_{0}$

### Globalna svojstva neprekidnosti
[[analiza1_1_kbt.png|Teorema]] (Koši-Bolcanova). $f:[a,\,b]\to\mathbb{R},\ \ f\,\mathcal{C}\,[a,\,b],\ \ f(a)\!\cdot\!f(b)<0\quad\Rightarrow$
$\Rightarrow\quad\exists c\in (a,\,b)\ :\ f(c)=0$

[[analiza1_1_međuvr.png|Teorema]] (o međuvrednosti). 
$f:[a,\,b]\to\mathbb{R},\ \ f\,\mathcal{C}\,[a,\,b],\ \ \gamma$ je između $f(a)$ i $f(b)\quad\Rightarrow$
$\Rightarrow\quad \exists c\in [a,\,b]\ :\ f(c)=\gamma$

> Iz teoreme:
> - Svaka vrednost između $f(a)$ i $f(b)$ se dostiže
> - Neprekidna slika intervala je interval

[[analiza1_1_vajer.png|Teorema]] (Vajerštrasova). $f:[a,\,b]\to\mathbb{R},\ \ f\,\mathcal{C}\,[a,\,b]$. Tada
1. $f$ je [[Relacija poretka#Donje i gornje ograničenje. Infinum i supremum|ograničena]].
2. $\exists \max\limits_{[a,\,b]}f,\ \min\limits_{[a,\,b]}f$

### [[Prekidi]]

### Neprekidnost i monotonost

[[analiza1_1_neprMonot.png|Teorema]]. $f:[a,\,b]\to\mathbb{R}$ je monotona fja, $f\Big[[a,\,b]\Big]$ je interval. 
Tada je $f$ neprekidna.

[[analiza1_1_16.png|Stav]]. $f:I\to\mathbb{R}$ je neprekidna i [[Funkcija|"1-1"]] ($I$ je neki interval).
Tada je $f$ strogo monotona. 

[[Inverzna funkcija]]

[[analiza1_1_17.png|Stav]]. $f:I\to f[I]$ je strogo rastuća (opadajuća) bijekcija. Tada je $\exists f^{-1}:f[I]\to I$ strogo rastuća (opadajuća)

[[analiza1_1_neprInverzne.png|Teorema]]. $f:[a,\,b] \to [\alpha,\,\beta]$ je strogo monotona neprekidna bijekcija. Tada je $f^{-1}$ neprekidna.

Posledica. $\sqrt[n]{x},\,\arcsin x,\,\arccos x,\,\mathrm{arctg}\, x,\,\ln x$ su neprekidne ^223f62