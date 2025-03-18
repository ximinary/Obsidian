#fax #math #a3 [deo [[Analiza|analize]]]
$\:$

[[Okolina tačke#Okolina u proizvoljnom Metrika metričkom prostoru|Okolina tačke]]
[[Vrste tačaka u odnosu na neki skup. Ograničenost i kompaktnost#^3de7f2|Tačaka nagomilavanja skupa]]

$\:$
**Def**. Neka je $D_{f}\subseteq\mathbb{R}^{n}$. **Limes funkcije** $f:\ D_{f}\to\mathbb{R}$ u tački $a\in  D'_{f}\:$ je jednak $L\in \overline{\mathbb{R}}\ \:$  $\Big( \lim\limits_{ x \to a }f(x) = L \Big)$ akko $\forall\varepsilon>0 \quad \exists \delta>0 \quad \forall x\in D_{f}\cap\mathring{\mathrm{O}}_{\delta}(a) \quad f(x)\in \mathrm{O}_{\varepsilon}(L)$

Slično limesu funkcije jedne promenljive za limes funkcije više promenljivih važe [[Limes funkcije#Svojstva limesa funkcije|svojstva]]: tvrđenja 1-4, aritmetičke operacije i teorema o tri limesa.

$\:$
Teorema (Hajneova definicija limesa funkcije).
Neka su $D_{f}\subseteq\mathbb{R}^{n},\ \ \ f:\ D_{f}\to\mathbb{R},\ \ \ a\in  D_{f}',\ \ \  L\in \overline{\mathbb{R}}$
$\lim\limits_{ x \to x_{0} }f(x)=L\quad\Leftrightarrow\quad\forall\text{niz }\underset{(a_{n}\,\ne\,x_{0})}{a_{n}\to x_{0}}\ \ \text{ važi }\ \lim\limits_{ n \to \infty }f(a_{n})=L$
___
**Def**. Neka je $D_{f}\subseteq\mathbb{R}^{n}$.  $f:\ D_{f}\to\mathbb{R}$ je **neprekidna** u tački $a\in D_{f}\ \  (f\,\mathcal{C}\,a)$ akko $\forall\varepsilon>0\quad\exists\delta>0\quad\forall x\in D_{f}\cap\mathrm{O}_{\delta}(a)\quad|f(x)-f(a)|<\varepsilon \ \ \Leftrightarrow$
$\Leftrightarrow \ \ \begin{cases} \mathrm{uvek\ važi,\quad\quad\quad\ ako}\ a\notin D_{f}'\\ \lim\limits_{ x \to a } f(x) = f(a),\ \mathrm{\ \ \!ako}\ a\in D_{f}'\end{cases}$

Slično kao za neprekidnu funkciju jedne promenljive za neprekidnu funkciju više promenljivih važe [[Neprekidnost#Lokalna svojstva neprekidnosti|svojstva]] 1-4 $\Big($u 4) $f$ je funkcija jedne promenljive$\Big)$.

**Stav**. Neka su $u(x,\,y)$ $\,$ i $\,$ $v(x,\,y)$ neprekidne u $(x_{0},\,y_{0})$ i važi $u(x_{0},\,y_{0})=u_{0}$ $\,$ i $\,$ $v(x_{0},\,y_{0})=v_{0}$. Ako je $f(s,\,t)$ neprekidna u $(u_{0},\,v_{0})$ onda je $g(x,\,y):=f\big(u(x,\,y),\ v(x,\,y)\big)$ neprekidna u $(x_{0},\,y_{0})$

**Teorema** (Vajerštrasova). $K\subseteq\mathbb{R}^{n}$ je [[Vrste tačaka u odnosu na neki skup. Ograničenost i kompaktnost#^3969f8|kompaktan]]. $f:K\to\mathbb{R},\ \ f\,\mathcal{C}\,K$. Tada
1. $f$ je [[Relacija poretka#Donje i gornje ograničenje. Infinum i supremum|ograničena]]
2. $\exists \max\limits_{x\in K}f(x),\ \min\limits_{x\in K}f(x)$
