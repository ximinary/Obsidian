#fax #math #a1 [deo [[Analiza|analize]]]
$\:$

[[Okolina tačke]]
[[Vrste tačaka u odnosu na neki skup#^3de7f2|Tačaka nagomilavanja skupa]]


**Def**. **Limes funkcije** $f:\ D_{f}\to\mathbb{R}$ u tački $a\in  D_{f}'\:$ je jednak $L\in \overline{\mathbb{R}}\ \:$  $\Big( \lim\limits_{ x \to a }f(x) = L \Big)$ akko $\forall\varepsilon>0 \quad \exists \delta>0 \quad \forall x\in D_{f}\cap\mathring{\mathrm{O}}_{\delta}(a) \quad f(x)\in \mathrm{O}_{\varepsilon}(L)$

**Def**. **Levi**/**desni limes funkcije** $f:\ D_{f}\to\mathbb{R}$ u tački $a\in  D_{f}'\:$ je jednak $L\in \overline{\mathbb{R}}\ \:$  $\Big( f(a^{-/+}) =\lim\limits_{ x \to a^{-/+} }f(x) = L \Big)$ akko $\forall\varepsilon>0 \quad \exists \delta>0 \quad \forall x\in D_{f}\cap\mathring{\mathrm{O}}_{\delta}^{-/+}(a) \quad f(x)\in \mathrm{O}_{\varepsilon}(L)$

--- 

[[analiza1_3_Hajne.png|Teorema]] (Hajneova definicija limesa funkcije).
$f:\ D_{f}\to\mathbb{R},\ \ \ a\in  D_{f}',\ \ \  L\in \overline{\mathbb{R}}$
$\lim\limits_{ x \to x_{0} }f(x)=L\quad\Leftrightarrow\quad\forall\text{niz }\underset{(a_{n}\,\ne\,x_{0})}{a_{n}\to x_{0}}\ \ \text{ važi }\ \lim\limits_{ n \to \infty }f(a_{n})=L$

Posledica. Ako $\exists \underset{\ \ _{\ne0}}{a_{n}},\,\underset{\ \ _{\ne0}}{b_{n}}\to x_{0} \ \ :\ \ \lim\limits_{ n \to \infty }f(a_{n})\ne\lim\limits_{ n \to \infty }f(b_{n}),$
Tada $\nexists\lim\limits_{ x \to x_{0} }f(x)$
$\:$

[[analiza1_3_KošijevKriterijum.png|Teorema]] (Košijev kriterijum postojanja limesa funkcije). $x_{0}\in\overline{\mathbb{R}}$.
$\exists\lim\limits_{ x \to x_{0} }f(x)\in\mathbb{R}\quad\Leftrightarrow$
$\Leftrightarrow\quad\forall\varepsilon>0\quad\exists\delta>0\quad\forall x,\,y\in\mathring{\mathrm{O}}_{\delta}(x_{0})\quad\left|f(x)-f(y)\right|<\varepsilon$

### [[Neprekidnost]]

### Svojstva limesa funkcije

$f$ je ograničena na skupu $A$ (tj [[Direktna i inverzna slika skupa|slika skupa]] $A$ je [[Relacija poretka#Donje i gornje ograničenje. Infinum i supremum|ograničena]]) akko $\exists c>0 \quad \forall x\in A \quad |f(x)|<c$ 

[[analiza1_1_1.png|Tvrđenje 1]]. $f:\ D_{f}\to \mathbb{R}$; $a\in D_{f}$; $\lim\limits_{ x \to a }f(x) \in \mathbb{R}$ 
Tada $\exists c>0,\, \delta>0\quad\forall x\in \mathring{\mathrm{O}}_{\delta}(a)\quad|f(x)|\leqslant c$ 
(tj $f$ je ograničena u nekoj okolini tačke $a$)
Oznaka: $f(x) = O(1),\ \ \ x\!\to\! a$  ^9993ac

[[analiza1_1_2.png|Tvrđenje 2]]. $f:\ D_{f}\to \mathbb{R}$; $a\in D_{f}$; $\:$ $\lim\limits_{ x \to a }f(x) = L > c\ \  (<c)\ \ \Rightarrow$ $\Rightarrow\ \ \exists\delta>0\quad\forall x\in D_{f}\cap \mathring{\mathrm{O}}_{\delta}(a)\quad f(x) >c\  (<c)$  ^abfa5c

**Def**. $\alpha:D_{\alpha}\to \mathbb{R}$; $a\in D_{\alpha}$
$\alpha(x)$ je **beskonačno mala funkcija** (b.m.f.) u okolini tačke $a$  
Oznaka: $\alpha(x)=o(1),\ \ \ x\!\to\!a$

Tvrđenje 3. $a\in \overline{\mathbb{R}}$
- [[analiza1_1_3_1.png|1)]] $\lim\limits_{ x \to a }f(x) = L \in \mathbb{R}\ \ \Leftrightarrow$
  $\quad \Leftrightarrow\ \ \exists \alpha(x)=o(1), \ \ x\!\to\!a \ :\ f(x) = L + \alpha(x)$ ^cabb77
- [[analiza1_1_3_2.png|2)]] $\alpha(x)=o(1),\,\beta(x)=o(1),\ \ x\!\to\!a \ \ \Rightarrow$
  $\quad \Rightarrow \ \ \alpha(x) + \beta(x) = o(1),\ \ x\!\to\!a$
- [[analiza1_1_3_3.png|3)]] $\alpha(x)=o(1),\,f(x)=O(1),\ \ x\!\to\!a \ \ \Rightarrow$
  $\quad \Rightarrow \ \ \alpha(x) \, f(x) = o(1),\ \ x\!\to\!a$

Teorema (aritmetičke operacije). $a\in D';$ $f:D\!\to\!\mathbb{R},\ \ \lim\limits_{ x \to a }f(x) = L\in \mathbb{R}; \ \:$$g:D\!\to\!\mathbb{R}, \ \ \lim\limits_{ x \to a }g(x) =M \in \mathbb{R}$. Tada: ^2c8b48
- [[analiza1_1_teoAritmOplim_1.png|1)]] $\quad\lim\limits_{ x \to a } \Big[f(x) +g(x) \Big] = L + M$ ^a79518
- [[analiza1_1_teoAritmOplim_2.png|2)]] $\quad\lim\limits_{ x \to a } f(x)\cdot g(x) = L\cdot M$ ^53cf78
- [[analiza1_1_teoAritmOplim_3_1.png|3.1)]] $\,\begin{align} \lim\limits_{ x \to a } \frac{1}{g(x)} = \frac{1}{M}\end{align},$ ako $M\ne 0$
- [[analiza1_1_teoAritmOplim_3_2.png|3.2)]] $\,\begin{align} \lim\limits_{ x \to a } \frac{f(x)}{g(x)} = \frac{L}{M}\end{align},$ ako $M\ne 0$ ^44b570

[[analiza1_1_4.png|Tvrđenje 4]]. $a\in D';$
 $f:D\!\to\!\mathbb{R},\ \ \lim\limits_{ x \to a }f(x) = L\in \mathbb{R}; \ \:$$g:D\!\to\!\mathbb{R}, \ \  \lim\limits_{ x \to a }g(x) =M \in \mathbb{R};$
 $\exists \delta_{1}>0\quad \forall x\in \mathring{\mathrm{O}}_{\delta_{1}}(a) \quad f(x)\leqslant g(x)$. $\:$ Tada $L\leqslant M$

[[analiza1_1_teo3lim.png|Teorema]] (o tri limesa / o dva policajaca).
$a \in D';\ \ \exists \delta_{0}>0\quad \forall x\in \mathrm{O}_{\delta_{0}}(a) \quad f(x)\leqslant g(x)\leqslant h(x);$
$\lim\limits_{ x \to a }f(x) = \lim\limits_{ x \to a }g(x) = L\in \mathbb{R}$. $\:$ Tada $\:$  $\lim\limits_{ x \to a }h(x) = L$ ^dd4e68

Teorema. $a\in D',\ \  f:D\!\to\!\mathbb{R},\ \ g:D\!\to\!\mathbb{R}, \ \ L\in \mathbb{R}$
![[analiza1_1_8.png]]

[[analiza1_1_NeprIlimKomut.png|Teorema]] ([[Neprekidnost|neprekidna fja]] i limes komutiraju). $a\in \overline{\mathbb{R}}$
$\varphi$ je neprekidna u $L\in\mathbb{R}\:$ i $\:\lim\limits_{ x \to a }f(x)=L$
Tada: $\lim\limits_{ x \to a }\varphi\big(f(x)\big) = \varphi \Big(\lim_{ x \to a }f(x)\Big) = \varphi(L)$

Teorema (smena promenljive u limesu). 
$a,\,b,\,c,\,d\in\mathbb{R};\ L\in\overline{\mathbb{R}}; \ t_{0}\in(a,\,b);\ x_{0}\in(c,\,d)$
$\varphi:\ (a,\,b)\to(c,\,d)$ je neprekidna bijekcija. Tada
$\exists\lim\limits_{ x \to x_{0} }f(x)=L\ \ \Leftrightarrow\ \ \exists\lim\limits_{ t \to t_{0} }f\big(\varphi(t)\big) = L$

### Neodređeni oblici
1. $+\infty -\infty$
2. $\begin{align}\frac{0}{0}\end{align}$
3. $\begin{align}\frac{\infty}{\infty}\end{align}$
4. $0\cdot\infty$
5. $1^{\infty}=e^{\infty\cdot\ln1}=e^{\infty\cdot0}$
6. $\infty^{0}=e^{0\cdot\ln\infty}=e^{0\cdot\infty}$
7. $0^{0}=e^{0\cdot\ln0}=e^{0\cdot\infty}$

### [[Osnovni limesi#Limesi funkcija|Osnovni limesi]]

### Limes monotone funkcije

$\inf\limits_{A}f:=\inf f[A]\ \ \:$ — infinum slike skupa $A$, funkcija $f$
$\sup\limits_{A}f:=\sup f[A]\ \ \:$ — supremum slike skupa $A$, funkcija $f$

[[analiza1_1_limMonotone.png|Teorema]]. $f:\ D_{f}\to\mathbb{R};\ \ (a,\,b)\subseteq D_{f}$
1. $f$ je rastuća i ograničena odozgo na $(a,\,b)\ \ \Rightarrow$
$\Rightarrow\ \ \lim\limits_{ x \to b^{-} }f(x)=\sup\limits_{(a,\,b)}f$
2. $f$ je rastuća i ograničena odozdo na $(a,\,b)\ \ \Rightarrow$
$\Rightarrow\ \ \lim\limits_{ x \to a^{+} }f(x)=\inf\limits_{(a,\,b)}f$
3. $f$ je opadajuća i ograničena odozgo na $(a,\,b)\ \ \Rightarrow$
$\Rightarrow\ \ \lim\limits_{ x \to a^{+} }f(x)=\sup\limits_{(a,\,b)}f$
4. $f$ je opadajuća i ograničena odozdo na $(a,\,b)\ \ \Rightarrow$
$\Rightarrow\ \ \lim\limits_{ x \to b^{-} }f(x)=\inf\limits_{(a,\,b)}f$
- Napomena: ako $f$ nije ograničena odozgo/odozdo onda je odgovarajući limes jednak $+\infty\,(-\infty)$

### [[Asimptotske klase. Asimptotska relacija ekvivalencije]]
### [[Asimptota]]
---
### Rešavanje limesa funkcije

Posledica [[Lopitalova pravila|Lapitalovih pravila]]:
[[analiza1_2_skala.png|Skala]]. Za $\alpha>0,\ a>1\:\:$važi
$\ln x \ll x^{\alpha}\ll a^{x},\ \ x\to+\infty$
(tj. $\ln x=o(x^{\alpha}),\ \ x\to +\infty\quad \mathrm{i}\quad x^{\alpha}=o(a^{x}),\ \ x\to +\infty$)

[[Lopitalova pravila]]
[[Tejlorov polinom]]