#fax #math #a3 [deo [[Analiza|analize]]]
$\:$

> Napomena:
[[Okolina tačke#Okolina u proizvoljnom Metrika metričkom prostoru|Okolina tačke]]
[[Vrste tačaka u odnosu na neki skup. Ograničenost i kompaktnost#^3de7f2|Tačaka nagomilavanja skupa]]

$\:$
### Limes funkcije $\mathbb{R}^{n}\to\mathbb{R}$
**Def**. Neka je $D_{f}\subseteq\mathbb{R}^{n}$. **Limes funkcije** $f:\ D_{f}\to\mathbb{R}$ u tački $\mathbf{a}\in  D'_{f}\:$ je jednak $L\in \overline{\mathbb{R}}\ \:$  $\Big( \lim\limits_{ \mathbf{x} \to \mathbf{a} }f(\mathbf{x}) = L \Big)$ akko $\forall\varepsilon>0 \quad \exists \delta>0 \quad \forall \mathbf{x}\in D_{f}\cap\mathring{\mathrm{O}}_{\delta}(\mathbf{a}) \quad f(\mathbf{x})\in \mathrm{O}_{\varepsilon}(L)$

Slično limesu funkcije jedne promenljive za limes funkcije više promenljivih važe [[Limes funkcije jedne promenljive#Svojstva limesa funkcije|svojstva]]: tvrđenja 1-4, aritmetičke operacije i teorema o tri limesa.

$\:$
Teorema (Hajneova definicija limesa funkcije).
Neka su $D_{f}\subseteq\mathbb{R}^{n},\ \ \ f:\ D_{f}\to\mathbb{R},\ \ \ \mathbf{a}\in  D_{f}',\ \ \  L\in \overline{\mathbb{R}}$
$\lim\limits_{ \mathbf{x} \to \mathbf{a} }f(\mathbf{x})=L\quad\Leftrightarrow\quad\forall\text{niz }\underset{(\mathbf{a}_{n}\,\ne\,\mathbf{a})}{\mathbf{a}_{n}\to \mathbf{a}}\ \ \text{ važi }\ \lim\limits_{ n \to \infty }f(\mathbf{a}_{n})=L$

### Neprekidnost funkcije $\mathbb{R}^{n}\to\mathbb{R}$
**Def**. Neka je $D_{f}\subseteq\mathbb{R}^{n}$.  $f:\ D_{f}\to\mathbb{R}$ je **neprekidna** u tački $\mathbf{a}\in D_{f}\ \  (f\,\mathcal{C}\,\mathbf{a})$ akko $\forall\varepsilon>0\quad\exists\delta>0\quad\forall \mathbf{x}\in D_{f}\cap\mathrm{O}_{\delta}(\mathbf{a})\quad|f(\mathbf{x})-f(\mathbf{a})|<\varepsilon \ \ \Leftrightarrow$
$\Leftrightarrow \ \ \begin{cases} \mathrm{uvek\ važi,\quad\quad\quad\ \ \! ako}\ \mathbf{a}\notin D_{f}'\\ \lim\limits_{ \mathbf{x} \to \mathbf{a} } f(\mathbf{x}) = f(\mathbf{a}),\ \mathrm{\ \ \!ako}\ \mathbf{a}\in D_{f}'\end{cases}$

Slično kao za neprekidnu funkciju jedne promenljive za neprekidnu funkciju više promenljivih važe [[Neprekidnost funkcije jedne promenljive#Lokalna svojstva neprekidnosti|svojstva]] 1-4 $\Big($u 4) $f$ je funkcija jedne promenljive$\Big)$.

**Stav**. Neka su $u(x,\,y)$ $\,$ i $\,$ $v(x,\,y)$ neprekidne u $(x_{0},\,y_{0})$ i važi $u(x_{0},\,y_{0})=u_{0}$ $\,$ i $\,$ $v(x_{0},\,y_{0})=v_{0}$. Ako je $f(s,\,t)$ neprekidna u $(u_{0},\,v_{0})$ onda je $g(x,\,y):=f\big(u(x,\,y),\ v(x,\,y)\big)$ neprekidna u $(x_{0},\,y_{0})$

**Teorema** (Vajerštrasova). $K\subseteq\mathbb{R}^{n}$ je [[Vrste tačaka u odnosu na neki skup. Ograničenost i kompaktnost#^3969f8|kompaktan]]. $f:K\to\mathbb{R},\ \ f\,\mathcal{C}\,K$. Tada ^8e141b
1. $f$ je ograničena
2. $\exists \max\limits_{\mathbf{x}\in K}f(\mathbf{x}),\ \min\limits_{\mathbf{x}\in K}f(\mathbf{x})$
### Limes i neprekidnost funkcije $\mathbb{R}^{n}\to\mathbb{R}^{m}$
**Def**. Neka je $D_{f}\subseteq\mathbb{R}^{n}$. **Limes funkcije** $F:\ D_{f}\to\mathbb{R}^{m}$ u tački $a\in  D'_{f}\:$ je jednak $L\in \mathbb{R}^{m}\ \:$  $\Big( \lim\limits_{ x \to a }F(x) = L \Big)$ akko $\forall\varepsilon>0 \quad \exists \delta>0 \quad \forall x\in D_{f}\cap\mathring{\mathrm{O}}_{\delta}(a) \quad F(x)\in \mathrm{O}_{\varepsilon}(L)$

$\:$
**Stav**. Neka je $A\subseteq\mathbb{R}^{n}$, $\ \:$ $a\in A'$, $\ \:$  $\forall i=\overline{1,m}\quad f_{i}:\ A\to\mathbb{R}$, $\ \:$ $F:\ A\to\mathbb{R}^{m}$ $\:$ takva da $\:$ $F(x)=\big(f_{1}(x),\,f_{2}(x),\,\dots,\,f_{m}(x)\big)$. Tada
$\lim\limits_{ x \to a }F(x)=(l_{1},\,l_{2},\,\dots,\,l_{m})\quad\Leftrightarrow\quad\forall i=\overline{1,m}\quad\lim\limits_{ x \to a }f_{i}(x)=l_{i}$

$\:$
**Def**. Neka je $A\subseteq\mathbb{R}^{n}$, $\ \:$ $a\in A$, $\ \:$  $\forall i=\overline{1,m}\quad f_{i}:\ A\to\mathbb{R}$, $\ \:$ $F:\ A\to\mathbb{R}^{m}$ $\:$ takva da $\:$ $F(x)=\big(f_{1}(x),\,f_{2}(x),\,\dots,\,f_{m}(x)\big)$. 
$F$ je neprekidna u tački $a$ ako je $f_{i}$ neprekidna u tački $a$ za $\forall i=\overline{1,m}$

$\:$
> Svojstva limesa i neprekidnosti vektorske funkcije se svode na svojstva koordinatnih funkcija.