#fax #math #a3 [deo [[Analiza|analize]]]
$\:$

[[Okolina tačke#Okolina u proizvoljnom Metrika metričkom prostoru|Okolina tačke]]
[[Vrste tačaka u odnosu na neki skup. Ograničenost i kompaktnost#^3de7f2|Tačaka nagomilavanja skupa]]

### Limes
**Def**. Neka je $D_{f}\subseteq\mathbb{R}^{n}$. **Limes funkcije** $f:\ D_{f}\to\mathbb{R}$ u tački $\mathbf{a}\in  D'_{f}\:$ je jednak $L\in \overline{\mathbb{R}}\ \:$  $\Big( \lim\limits_{ \mathbf{x} \to \mathbf{a} }f(\mathbf{x}) = L \Big)$ akko $\forall\varepsilon>0 \quad \exists \delta>0 \quad \forall \mathbf{x}\in D_{f}\cap\mathring{\mathrm{O}}_{\delta}(\mathbf{a}) \quad f(\mathbf{x})\in \mathrm{O}_{\varepsilon}(L)$

Slično limesu funkcije jedne promenljive za limes funkcije više promenljivih važe [[Limes funkcije#Svojstva limesa funkcije|svojstva]]: tvrđenja 1-4, aritmetičke operacije i teorema o tri limesa.

$\:$
Teorema (Hajneova definicija limesa funkcije).
Neka su $D_{f}\subseteq\mathbb{R}^{n},\ \ \ f:\ D_{f}\to\mathbb{R},\ \ \ \mathbf{a}\in  D_{f}',\ \ \  L\in \overline{\mathbb{R}}$
$\lim\limits_{ \mathbf{x} \to \mathbf{a} }f(\mathbf{x})=L\quad\Leftrightarrow\quad\forall\text{niz }\underset{(\mathbf{a}_{n}\,\ne\,\mathbf{a})}{\mathbf{a}_{n}\to \mathbf{a}}\ \ \text{ važi }\ \lim\limits_{ n \to \infty }f(\mathbf{a}_{n})=L$

### Neprekidnost
**Def**. Neka je $D_{f}\subseteq\mathbb{R}^{n}$.  $f:\ D_{f}\to\mathbb{R}$ je **neprekidna** u tački $\mathbf{a}\in D_{f}\ \  (f\,\mathcal{C}\,\mathbf{a})$ akko $\forall\varepsilon>0\quad\exists\delta>0\quad\forall \mathbf{x}\in D_{f}\cap\mathrm{O}_{\delta}(\mathbf{a})\quad|f(\mathbf{x})-f(\mathbf{a})|<\varepsilon \ \ \Leftrightarrow$
$\Leftrightarrow \ \ \begin{cases} \mathrm{uvek\ važi,\quad\quad\quad\ \ \! ako}\ \mathbf{a}\notin D_{f}'\\ \lim\limits_{ \mathbf{x} \to \mathbf{a} } f(\mathbf{x}) = f(\mathbf{a}),\ \mathrm{\ \ \!ako}\ \mathbf{a}\in D_{f}'\end{cases}$

Slično kao za neprekidnu funkciju jedne promenljive za neprekidnu funkciju više promenljivih važe [[Neprekidnost#Lokalna svojstva neprekidnosti|svojstva]] 1-4 $\Big($u 4) $f$ je funkcija jedne promenljive$\Big)$.

**Stav**. Neka su $u(x,\,y)$ $\,$ i $\,$ $v(x,\,y)$ neprekidne u $(x_{0},\,y_{0})$ i važi $u(x_{0},\,y_{0})=u_{0}$ $\,$ i $\,$ $v(x_{0},\,y_{0})=v_{0}$. Ako je $f(s,\,t)$ neprekidna u $(u_{0},\,v_{0})$ onda je $g(x,\,y):=f\big(u(x,\,y),\ v(x,\,y)\big)$ neprekidna u $(x_{0},\,y_{0})$

**Teorema** (Vajerštrasova). $K\subseteq\mathbb{R}^{n}$ je [[Vrste tačaka u odnosu na neki skup. Ograničenost i kompaktnost#^3969f8|kompaktan]]. $f:K\to\mathbb{R},\ \ f\,\mathcal{C}\,K$. Tada ^8e141b
1. $f$ je ograničena
2. $\exists \max\limits_{\mathbf{x}\in K}f(\mathbf{x}),\ \min\limits_{\mathbf{x}\in K}f(\mathbf{x})$
### Parcijalni izvod i izvod u pravcu
**Def**. Neka su $D_{f}\subseteq\mathbb{R}^{n}$, $\ \:$  $f:\ D_{f}\to\mathbb{R}$, $\ \:$ $\mathbf{x}^{0}=(x^{0}_{1},\,x^{0}_{2},\,\dots,\,x^{0}_{n})\in\mathrm{int}\,D_{f}$. Tada ako $\begin{align}\exists  \lim\limits_{ h \to 0 }\frac{f(x^{0}_{1},\,\dots,\,x^{0}_{i}+h,\,\dots,\,x^{0}_{n})-f(x^{0}_{1},\,\dots,\,x^{0}_{i},\,\dots,\,x^{0}_{n})}{h} := f'_{x_{i}}(\mathbf{x}^{0})=\frac{\partial f}{\partial x_{i}}(\mathbf{x}^{0}) \end{align}$,
 on se zove **parcijalni izvod** fje $f$ po $x_{i}$ u tački $\mathbf{x}^{0}$

$\:$
**Def**. Neka su $D_{f}\subseteq\mathbb{R}^{n}$, $\ \:$  $f:\ D_{f}\to\mathbb{R}$, $\ \:$ $\mathbf{x}^{0}\in\mathrm{int}\,D_{f}$ $\:$ i $\:$ $\mathbf{v}\in\mathbb{R}^{n}$ takav da $||\mathbf{v}||=1$. Tada ako $\begin{align}\exists  \lim\limits_{ h \to 0 }\frac{f(\mathbf{x}^{0}+h\,\mathbf{v})-f(\mathbf{x}^{0})}{h} := f'_{\mathbf{v}}(\mathbf{x}^{0})=\frac{\partial f}{\partial \mathbf{v}}(\mathbf{x}^{0})\end{align}$,
 on se zove **izvod u pravcu** vektora $\mathbf{v}$ fje $f$ u tački $\mathbf{x}^{0}$

> Napomena: parcijalni izvod po $x_{i}$ je izvod u pravcu vektora $\mathbf{e}_{i}=(0,\,0,\,\dots,\,0,\,\overset{i}{1},\,0,\,\dots,\,0,\,0)$ 
> tj. $\begin{align}\frac{\partial f}{\partial x_{i}}(\mathbf{x}^{0})=\frac{\partial f}{\partial \mathbf{e}_{i}}(\mathbf{x}^{0})\end{align}$

$\:$
**Def**. Parcijalni izvod drugog reda:
$\begin{align}f''_{x_{i}x_{j}}=\frac{\partial^{2} f}{\partial x_{i}\,\partial x_{j}}:=\big(f'_{x_{i}}\big)'_{x_{j}}=\frac{\partial }{x_{j}}\bigg(\frac{\partial f}{x_{i}}\bigg)\end{align}$ 
Analogno se definišu parcijalni izvodi višeg (3, 4, ...) reda.
Pri tome $\begin{align}f^{(0)}=\partial^{0}f=f\end{align}$

$\:$
**Stav**. Ako na $\mathrm{O}(\mathbf{x}^{0})$ postoje parcijalni izvodi $f''_{x_{i}x_{j}}$ i $f''_{x_{j}x_{i}}$, koje su neprekidne u $\mathbf{x}^{0}$ onda $f''_{x_{i}x_{j}}(\mathbf{x}^{0})=f''_{x_{j}x_{i}}(\mathbf{x}^{0})$

$\:$
**Def**. Hesijan (ili matrica drugog izvoda) fje $f$ u $\mathbf{x}^{0}$ je
$Hf(\mathbf{x}^{0})=d^{2}f(\mathbf{x}^{0})=\left(\begin{array}{}f''_{x_{1}x_{1}}(\mathbf{x}^{0})&f''_{x_{1}x_{2}}(\mathbf{x}^{0})&\dots&f''_{x_{1}x_{n}}(\mathbf{x}^{0})\\f''_{x_{2}x_{1}}(\mathbf{x}^{0})&f''_{x_{2}x_{2}}(\mathbf{x}^{0})&\dots&f''_{x_{2}x_{n}}(\mathbf{x}^{0})\\\dots&\dots&\dots&\dots\\f''_{x_{n}x_{1}}(\mathbf{x}^{0})&f''_{x_{n}x_{2}}(\mathbf{x}^{0})&\dots&f''_{x_{n}x_{n}}(\mathbf{x}^{0})\end{array}\right)$ ^39ff87

### [[Tejlorov polinom#Tejlorov polinom funkcije više promenljivih|Tejlorov polinom]]

### Diferencijabilnost
> Napomena: diferencijabilnost fje jedne promenljive: [[Izvod#^0328e7|*]], [[Izvod#^85d2e1|*]]

**Def**. Neka su $D_{f}\subseteq\mathbb{R}^{n}$, $\ \:$  $f:\ D_{f}\to\mathbb{R}$, $\ \:$ $\mathbf{x}^{0}\in\mathrm{int}\,D_{f}$.
$f$ je **diferencijabilna** u $\mathbf{x}^{0}$ ako postoji linearno preslikavanje $L:\,\mathbb{R}^{n}\to\mathbb{R}$ takvo da
$\begin{align}f(\mathbf{x}^{0}+\mathbf{h})=f(\mathbf{x}^{0})+L\,\mathbf{h}+o\big(||\mathbf{h}||\big),\quad \mathbf{h}\to\mathbf{0}\quad\ &&&&&&&&&(1)\end{align}$
> $\begin{align}\Leftrightarrow \quad\lim\limits_{ \mathbf{h} \to \mathbf{0} } \frac{f(\mathbf{x}^{0}+\mathbf{h})-f(\mathbf{x}^{0})-L\,\mathbf{h}}{||\mathbf{h}||}=0&&&&&&&&&&(2)\end{align}$

Preslikavanje $L$ se zove **diferencijal** (izvod) fje $f$ u tački $\mathbf{x}^{0}$ i označava se sa $df(\mathbf{x}^{0})$ ili $f'(\mathbf{x}^{0})$

$\:$
**Stav**. Neka su $D_{f}\subseteq\mathbb{R}^{n}$, $\ \:$  $f:\ D_{f}\to\mathbb{R}$, $\ \:$ $\mathbf{x}^{0}\in\mathrm{int}\,D_{f}$.
Ako je $f$ diferencijabilna u $\mathbf{x}^{0}$ onda $\forall\big(\mathbf{v}\in\mathbb{R}^{n}\ \ :\ \ ||\mathbf{v}||=1\big)\quad\exists f'_{\mathbf{v}}(\mathbf{x}^{0})=df(\mathbf{x}^{0})\,\mathbf{v}$
> Dokaz: Neka je $L=df_{\mathbf{v}}(\mathbf{x}^{0})$.
> 
> Iz $(1)$: $\quad$ $\begin{align}f(\mathbf{x}^{0}+\mathbf{h})=f(\mathbf{x}^{0})+L\,\mathbf{h}+o\big(||\mathbf{h}||\big),\quad \mathbf{h}\to\mathbf{0}\end{align}$
jer je $\mathbf{h}$ proizvoljno, suzimo ga do $\mathbf{h}=\lambda\,\mathbf{v}$, pri tome važi
$\begin{align}f(\mathbf{x}^{0}+\lambda\,\mathbf{v})=f(\mathbf{x}^{0})+L\,\lambda\,\mathbf{v}+o\big(||\lambda\,\mathbf{v}||\big),\quad \lambda\to\mathbf{0}\end{align}$
$\begin{align}\frac{f(\mathbf{x}^{0}+\lambda\,\mathbf{v})-f(\mathbf{x}^{0})}{\lambda}=\,L\,\mathbf{v}+o(1),\quad \lambda\to\mathbf{0}\end{align}$
$\begin{align}f'_{\mathbf{v}}(\mathbf{x}^{0})=\lim\limits_{ \lambda \to \infty }\frac{f(\mathbf{x}^{0}+\lambda\,\mathbf{v})-f(\mathbf{x}^{0})}{\lambda}=\,L\,\mathbf{v}\end{align}$

$\:$
**Posledica**. Neka su $D_{f}\subseteq\mathbb{R}^{n}$, $\ \:$  $f:\ D_{f}\to\mathbb{R}$, $\ \:$ $\mathbf{x}^{0}\in\mathrm{int}\,D_{f}$.
Ako je $f$ diferencijabilna u $\mathbf{x}^{0}$ onda $df(\mathbf{x}^{0})=\Big(\begin{array}{}f'_{x_{1}}(\mathbf{x}^{0})&f'_{x_{2}}(\mathbf{x}^{0})&\cdots&f'_{x_{n}}(\mathbf{x}^{0})\end{array}\Big)$
tj. važi $\begin{align}df(\mathbf{x}^{0})\left(\begin{array}{}h_{1}\\h_{2}\\\dots\\h_{n}\end{array}\right)=h_{1}\,f'_{x_{1}}(\mathbf{x}^{0})+h_{2}\,f'_{x_{2}}(\mathbf{x}^{0})+\dots+h_{n}\,f'_{x_{n}}(\mathbf{x}^{0})=\sum\limits_{i=1}^{n}h_{i}\,f'_{x_{i}}(\mathbf{x}^{0})\end{align}$ ^d2bcd7
> Dokaz: iz prethodnog stava $\forall i=\overline{1,n}\quad df(\mathbf{x}^{0})\,\mathbf{e}_{i}=f'_{\mathbf{e}_{i}}(\mathbf{x}^{0})=f'_{x_{i}}(\mathbf{x}^{0})$

**Def**. Neka su $D_{f}\subseteq\mathbb{R}^{n}$, $\ \:$  $f:\ D_{f}\to\mathbb{R}$, $\ \:$ $\mathbf{x}^{0}\in\mathrm{int}\,D_{f}$.
Vektor  $\nabla\!f(\mathbf{x}^{0})=\Big(f'_{x_{1}}(\mathbf{x}^{0}),\ \ f'_{x_{2}}(\mathbf{x}^{0}),\ \ \cdots,\ \ f'_{x_{n}}(\mathbf{x}^{0})\Big)$ zove se **gradijent** fje $f$ u tački $\mathbf{x}^{0}$.

$\:$
> Napomena: Tražimo diferencijal $L=df(\mathbf{x}^{0})$ tako što prvo nalazimo sve parcijalne izvode (ako neki parcijalni izvod ne postoji ne postoji i diferencijal).
> Zatim konstruišemo matricu iz posledice, pa ako postoji limes $(2)$ onda $L$ jeste diferencijal.

$\:$
**Stav**. $f$ je diferencijabilna u $\mathrm{x}^{0}$ $\quad$ $\Rightarrow$ $\quad$ $f$ je neprekidna u $\mathrm{x}^{0}$.
> Dokaz: iz diferencijabilnosti $f$ u $\mathbf{x}^{0}$ sledi da postoji preslikavanje $L:\,\mathbb{R}^{n}\to\mathbb{R}$ takvo da $\begin{align}f(\mathbf{x}^{0}+\mathbf{h})=f(\mathbf{x}^{0})+L\,\mathbf{h}+o\big(||\mathbf{h}||\big),\quad \mathbf{h}\to\mathbf{0}\end{align}$
> ili drugačije $f(\mathbf{x})=f(\mathbf{x}^{0})+L(\mathbf{x}-\mathbf{x}^{0})+o\big(||\mathbf{x}-\mathbf{x}^{0}||\big),\quad \mathbf{x}\to\mathbf{x}^{0}$
> odakle $\lim\limits_{ \mathbf{x} \to \mathbf{x}^{0} } f(\mathbf{x})=f(\mathbf{x}^{0})$ $\quad$ tj. $f\,\mathcal{C}\,\mathbf{x}^{0}$

$\:$
**Teorema** (dovoljni uslov diferencijabilnosti). Ako $f$ ima sve parcijalne izvode na $\mathrm{O}(\mathbf{x}^{0})$, i svaki od njih je neprekidan u $\mathbf{x}^{0}$ onda je $f$ diferencijabilna u $\mathbf{x}^{0 }$
> Dokaz: Pokazati da  $\begin{align}\lim\limits_{ \mathbf{x} \to \mathbf{x}^{0} }\frac{f(\mathbf{x})-f(\mathbf{x}^{0})-L(\mathbf{x}-\mathbf{x}^{0})}{||\mathbf{x}-\mathbf{x}^{0}||}=0\end{align}$
>
> Razmotrimo brojilac u limesu — oduzimamo i dodajemo iste članove:
> $\underbrace{f\left(\begin{array}{}x_{1}\\x_{2}\\x_{3}\\\dots\\x_{n}\end{array}\right)-f\left(\begin{array}{}x^{0}_{1}\\x_{2}\\x_{3}\\\dots\\x_{n}\end{array}\right)}_{=f'_{x_{1}}\left(\begin{array}{}\xi_{1}\\x_{2}\\x_{3}\\\dots\\x_{n}\end{array}\right)(x_{1}-x^{0}_{1})}+\underbrace{f\left(\begin{array}{}x^{0}_{1}\\x_{2}\\x_{3}\\\dots\\x_{n}\end{array}\right)-f\left(\begin{array}{}x^{0}_{1}\\x^{0}_{2}\\x_{3}\\\dots\\x_{n}\end{array}\right)}_{=f'_{x_{2}}\left(\begin{array}{}x^{0}_{1}\\\xi_{2}\\x_{3}\\\dots\\x_{n}\end{array}\right)(x_{2}-x^{0}_{2})}+\underbrace{f\left(\begin{array}{}x^{0}_{1}\\x^{0}_{2}\\x_{3}\\\dots\\x_{n}\end{array}\right)-}_{\dots}\dots \underbrace{-f\left(\begin{array}{}x^{0}_{1}\\x^{0}_{2}\\\dots\\x^{0}_{n-1}\\x_{n}\end{array}\right)}_{\dots}+\underbrace{f\left(\begin{array}{}x^{0}_{1}\\x^{0}_{2}\\\dots\\x^{0}_{n-1}\\x_{n}\end{array}\right)-f\left(\begin{array}{}x^{0}_{1}\\x^{0}_{2}\\\dots\\x^{0}_{n-1}\\x^{0}_{n}\end{array}\right)}_{=f'_{x_{n}}\left(\begin{array}{}x^{0}_{1}\\x^{0}_{2}\\\dots\\x^{0}_{n}\\\xi_{n}\end{array}\right)(x_{n}-x^{0}_{n})}-L(\mathbf{x}-\mathbf{x}^{0})=$
> > Što dobijamo iz [[Teoreme o srednjoj vrednosti#^e52da5|Lagranževe teoreme]] za fje jedne promenljive,
> > pri čemu $\forall i=\overline{1,n}\quad\xi_{i}$ je između $x_{i}$ i $x^{0}_{i}$ 
> >
> > Iz [[Funkcija sa domenom u Rn#^d2bcd7|posledice]] imamo $\begin{align}L(\mathbf{x}-\mathbf{x}^{0})=\sum\limits_{i=1}^{n}f'_{x_{i}}(\mathbf{x}^{0})(x_{i}-x^{0}_{i})\end{align}$
> 
> $\begin{align}=\sum\limits_{i=1}^{n}\underbrace{\left(f'_{x_{i}}\left(\begin{array}{}x^{0}_{1}\\\dots\\x^{0}_{i-1}\\\xi_{i}\\x_{i+1}\\\dots\\x_{n}\end{array}\right)-f'_{x_{i}} \left(\begin{array}{}x^{0}_{1}\\\dots\\x^{0}_{i-1}\\x^{0}_{i}\\x^{0}_{i+1}\\\dots\\x^{0}_{n}\end{array}\right)\right)}_{=\,\varphi_{i}(\mathbf{x})}(x_{i}-x^{0}_{i})\end{align}$
>
> Odakle jer su parcijalni izvodi neprekidni važi $\varphi_{i}(\mathbf{x})\to0,\quad\mathbf{x}\to\mathbf{x}^{0},\quad\forall i=\overline{1,n}$
> Odakle,
>  $\begin{align}\lim\limits_{ \mathbf{x} \to \mathbf{x}^{0} }\frac{f(\mathbf{x})-f(\mathbf{x}^{0})-L(\mathbf{x}-\mathbf{x}^{0})}{||\mathbf{x}-\mathbf{x}^{0}||}=\lim\limits_{ \mathbf{x} \to \mathbf{x}^{0} }\frac{\sum\limits_{i=1}^{n}\varphi_{i}(\mathbf{x})(x_{i}-x^{0}_{i})}{||\mathbf{x}-\mathbf{x}^{0}||}=\lim\limits_{ \mathbf{x} \to \mathbf{x}^{0} }\sum\limits_{i=1}^{n}\varphi_{i}(\mathbf{x})\frac{(x_{i}-x^{0}_{i})}{||\mathbf{x}-\mathbf{x}^{0}||}\end{align}$
>  
>  $\begin{align}\left|\sum\limits_{i=1}^{n}\varphi_{i}(\mathbf{x})\frac{(x_{i}-x^{0}_{i})}{||\mathbf{x}-\mathbf{x}^{0}||}\right|\leqslant\sum\limits_{i=1}^{n}\left|\varphi_{i}(\mathbf{x})\frac{(x_{i}-x^{0}_{i})}{||\mathbf{x}-\mathbf{x}^{0}||}\right|\leqslant\sum\limits_{i=1}^{n}\left|\varphi_{i}(\mathbf{x})\right|\to0,\quad\mathbf{x}\to\mathbf{x}^{0}\end{align}$
>
> Time iz teoreme o tri limesa dobijamo da je limes jednak $0$.

$\:$
### [[Ekstremum#Funkcija više promenljivih|Ekstremum ]]. [[Ekstremum#Uslovni ekstremum|Uslovni ekstremum]]