#fax #math #a3 [deo [[Analiza|analize]]]
$\:$

> Napomena: diferencijabilnost fje jedne promenljive: [[Izvod funkcije jedne promenljive#^0328e7|*]], [[Izvod funkcije jedne promenljive#^85d2e1|*]]

$\:$
### Diferencijabilnost funkcije $\mathbb{R}^{n}\to\mathbb{R}$

**Def**. Neka su $D_{f}\subseteq\mathbb{R}^{n}$, $\ \:$  $f:\ D_{f}\to\mathbb{R}$, $\ \:$ $\mathbf{x}^{0}\in\mathrm{int}\,D_{f}$.
$f$ je **diferencijabilna** u $\mathbf{x}^{0}$ ako postoji linearno preslikavanje $L:\,\mathbb{R}^{n}\to\mathbb{R}$ takvo da
$\begin{align}f(\mathbf{x}^{0}+\mathbf{h})=f(\mathbf{x}^{0})+L\,\mathbf{h}+o\big(||\mathbf{h}||\big),\quad \mathbf{h}\to\mathbf{0}\quad\ &&&&&&&&&(1)\end{align}$
> $\begin{align}\Leftrightarrow \quad\lim\limits_{ \mathbf{h} \to \mathbf{0} } \frac{f(\mathbf{x}^{0}+\mathbf{h})-f(\mathbf{x}^{0})-L\,\mathbf{h}}{||\mathbf{h}||}=0&&&&&&&&&&(2)\end{align}$

Preslikavanje $L$ se zove **diferencijal** (izvod) fje $f$ u tački $\mathbf{x}^{0}$ i označava se sa $df(\mathbf{x}^{0})$ ili $f'(\mathbf{x}^{0})$

$\:$
**Stav**. Neka su $D_{f}\subseteq\mathbb{R}^{n}$, $\ \:$  $f:\ D_{f}\to\mathbb{R}$, $\ \:$ $\mathbf{x}^{0}\in\mathrm{int}\,D_{f}$.
Ako je $f$ diferencijabilna u $\mathbf{x}^{0}$ onda $\forall\big(\mathbf{v}\in\mathbb{R}^{n}\ \ :\ \ ||\mathbf{v}||=1\big)\quad\exists f'_{\mathbf{v}}(\mathbf{x}^{0})=df(\mathbf{x}^{0})\,\mathbf{v}$
> Dokaz: Neka je $L=df(\mathbf{x}^{0})$.
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

$\:$
> Napomena: $df(\mathbf{x}^{0})=\Big(\nabla f(\mathbf{x}^{0})\Big)^{\mathrm{T}}$ $\quad$ (veza sa [[Parcijalni izvod#Operator nabla|gradijentom]])

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
> > Iz [[Diferencijabilnost funkcije više promenljivih#^d2bcd7|posledice]] imamo $\begin{align}L(\mathbf{x}-\mathbf{x}^{0})=\sum\limits_{i=1}^{n}f'_{x_{i}}(\mathbf{x}^{0})(x_{i}-x^{0}_{i})\end{align}$
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
### [[Ekstremum funkcije više promenljivih|Ekstremum]]

### Diferencijabilnost funkcije $\mathbb{R}^{n}\to\mathbb{R}^{m}$


**Def**. Neka su $D_{f}\subseteq\mathbb{R}^{n}$, $\ \:$  $F:\ D_{f}\to\mathbb{R}^{m}$, $\ \:$ $\mathbf{x}^{0}\in\mathrm{int}\,D_{f}$.
$f$ je **diferencijabilna** u $\mathbf{x}^{0}$ ako postoji linearno preslikavanje $L:\,\mathbb{R}^{n}\to\mathbb{R}^{m}$ takvo da
$\begin{align}F(\mathbf{x}^{0}+\mathbf{h})=F(\mathbf{x}^{0})+L\,\mathbf{h}+\mathbf{o}\big(||\mathbf{h}||\big),\quad \mathbf{h}\to\mathbf{0}\quad\ \ \, &&&&&&&&&&&(1)\end{align}$
gde je $\mathbf{o}(||h||)$ vektor fja $A=(\alpha_{1},\,\alpha_{2},\,\dots,\,\alpha_{m})$, takva da $\forall j=\overline{1,m}\quad \alpha(||\mathbf{h}||)\to0,\quad \mathbf{h}\to0$ 
> $\begin{align}\Leftrightarrow\quad\forall j=\overline{1,m}\quad f_{j}(\mathbf{x}^{0}+\mathbf{h})=f_{j}(\mathbf{x}^{0})+L_{j}\,\mathbf{h}+o\big(||\mathbf{h}||\big),\quad \mathbf{h}\to\mathbf{0}&&(2)\end{align}$
> gde je $L_{j}:\ \mathbb{R}^{n}\to\mathbb{R}$ linearno preslikavanje ($j$-ta vrsta matrice $L$).

Preslikavanje $L$ se zove **diferencijal** (izvod) fje $F$ u tački $\mathbf{x}^{0}$ i označava se sa $dF(\mathbf{x}^{0})$ ili $F'(\mathbf{x}^{0})$. Pri tome matricu tog preslikavanja zovemo **Jakobijevom matricom**, a determinantu te matrice $J_{F}(\mathbf{x}^{0})=\det dF(\mathbf{x}^{0})$ **jakobijanom**.

Iz [[Diferencijabilnost funkcije više promenljivih#^d2bcd7|posledice]] i $(2)$ dobijamo da
$\begin{align}dF(\mathbf{x}^{0})=\left(\begin{array}{}\frac{\partial f_{1}}{\partial x_{1}}(\mathbf{x}^{0})&\frac{\partial f_{1}}{\partial x_{2}}(\mathbf{x}^{0})&\cdots&\frac{\partial f_{1}}{\partial x_{n}}(\mathbf{x}^{0})\\\frac{\partial f_{2}}{\partial x_{1}}(\mathbf{x}^{0})&\frac{\partial f_{2}}{\partial x_{2}}(\mathbf{x}^{0})&\cdots&\frac{\partial f_{2}}{\partial x_{n}}(\mathbf{x}^{0})\\\cdots&\cdots&\cdots&\cdots\\\frac{\partial f_{m}}{\partial x_{1}}(\mathbf{x}^{0})&\frac{\partial f_{m}}{\partial x_{2}}(\mathbf{x}^{0})&\cdots&\frac{\partial f_{m}}{\partial x_{n}}(\mathbf{x}^{0})\end{array}\right)\end{align}$

**Primedba**. Neka su $D_{f}\subseteq\mathbb{R}^{n}$, $\ \:$  $F:\ D_{f}\to\mathbb{R}^{m}$, $\ \:$ $\mathbf{x}^{0}\in\mathrm{int}\,D_{f}$.
Ako je $F$ linearno preslikavanje onda $dF(\mathbf{x}^{0})=F(\mathbf{x}^{0})$

$\:$
**Stav** (diferenciranje složene fje). Neka su $A\subseteq\mathbb{R}^{n}$, $\:$ $B\subseteq\mathbb{R}^{m}$ $\:$ otvoreni skupovi i neka su $F:\ A\to B$, $\ \:$ $G:\ B\to\mathbb{R}^{k}$. $\:$ $\mathbf{x}^{0}\in A$, $\:$ $\mathbf{y}^{0}=F(\mathbf{x}^{0})\in B$. Tada
ako je $F$ diferencijabilna u $\mathbf{x}^{0}$ i $G$ je diferencijabilna u $\mathbf{y}^{0}$ onda je $G\circ F$ diferencijabilna u $\mathbf{x}^{0}$ i važi: $\boxed{d(G\circ F)(\mathbf{x}^{0})=dG(\mathbf{y}^{0})\circ dF(\mathbf{x}^{0})}$ ^4816ca
> Dokaz:
> $F\,\mathcal{D}\,\mathbf{x}^{0}\quad\Leftrightarrow\quad F(\mathbf{x}^{0}+\mathbf{h})=F(\mathbf{x}^{0})+dF(\mathbf{x}^{0})\,\mathbf{h}+\mathbf{o}\big(||\mathbf{h}||\big),\quad \mathbf{h}\to \mathbf{0}$
> $G\,\mathcal{D}\,\mathbf{y}^{0}\quad\Leftrightarrow\quad G(\mathbf{y}^{0}+\mathbf{k})=G(\mathbf{y}^{0})+dG(\mathbf{y}^{0})\,\mathbf{k}+\mathbf{o}\big(||\mathbf{k}||\big),\quad \mathbf{k}\to \mathbf{0}$
>
> $\mathbf{k}:= F(\mathbf{x}^{0}+\mathbf{h})-F(\mathbf{x}^{0})=F(\mathbf{x}^{0}+\mathbf{h})-\mathbf{y}^{0}\to0,\quad \mathbf{h}\to\mathbf{0}$ $\ \:$ (jer je $F$ neprekidna)
> 
> Odakle, $G\big(F(\mathbf{x}^{0}+\mathbf{h})\big)=G\big(F(\mathbf{x}^{0})\big)+dG\big(F(\mathbf{x}^{0})\big)\big(F(\mathbf{x}^{0}+\mathbf{h})-F(\mathbf{x}^{0})\big)+\mathbf{o}\big(||F(\mathbf{x}^{0}+\mathbf{h})-F(\mathbf{x}^{0})||\big),\quad\mathbf{h}\to\mathbf{0}$
$G\big(F(\mathbf{x}^{0}+\mathbf{h})\big)=G\big(F(\mathbf{x}^{0})\big)+dG\big(F(\mathbf{x}^{0})\big)\big(dF(\mathbf{x}^{0})\,\mathbf{h}+\mathbf{o}(||\mathbf{h||})\big)+\mathbf{o}\big(dF(\mathbf{x}^{0})\,\mathbf{h}+\mathbf{o}(||\mathbf{h||})\big),\quad\mathbf{h}\to\mathbf{0}$
$G\big(F(\mathbf{x}^{0}+\mathbf{h})\big)=G\big(F(\mathbf{x}^{0})\big)+dG\big(\mathbf{y}^{0}\big)dF(\mathbf{x}^{0})\,\mathbf{h}+\mathbf{o}\big(||\mathbf{h||}\big),\quad\mathbf{h}\to\mathbf{0}$

$\:$
**Stav** (diferenciranje inverzne fje). Neka su $A\subseteq\mathbb{R}^{n}$, $\:$ $F:\ A\to \mathbb{R}^{m}$, $\:$ $\mathbf{x}^{0}\in A$, $\:$ $\mathbf{y}^{0}=F(\mathbf{x}^{0})$. I neka je $F^{-1}:\ \mathrm{O}(\mathbf{y}^{0})\to A$ inverzna od $F$ na $\mathrm{O}(\mathbf{y}^{0})$. Tada ako su $F$ i $G$ diferencijabilni onda važi $\boxed{dF^{-1}\big(\mathbf{y}^{0}\big)=dF(\mathbf{x}^{0})^{-1}}$
> Dokaz: Iz prethodne teoreme:
> uzimamo $G:=F^{-1}$ i imamo $d(F^{-1}\circ F)(\mathbf{x}^{0})=dF^{-1}(\mathbf{y}^{0})dF(\mathbf{x}^{0})$
> Zbog toga što je $F^{-1}\circ F=\mathrm{id}_{\mathbf{x}}$ koristeći primedbu dobijamo da $d(F^{-1}\circ F)(\mathbf{x}^{0})=\mathrm{id}_{\mathbf{x}}$.
> Dakle, $dF^{-1}(\mathbf{y}^{0})dF(\mathbf{x}^{0})=\mathrm{id}_{\mathbf{x}}$