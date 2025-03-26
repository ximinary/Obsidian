#fax #math #a3 [deo [[Analiza|analize]]]
$\:$
 
**Def**. Neka je $A\subseteq\mathbb{R}^{n}$. Preslikavanje $F:\ A\to\mathbb{R}^{m}$ za koje važi $F(x)=\big(f_{1}(x),\,f_{2}(x),\,\dots,\,f_{m}(x)\big)$ zove se **vektorska funkcija**.
$\forall i=\overline{1,m}\quad f_{i}:\ A\to\mathbb{R}$ su **koordinatne funkcije**.

### Limes i neprekidnost
**Def**. Neka je $D_{f}\subseteq\mathbb{R}^{n}$. **Limes funkcije** $F:\ D_{f}\to\mathbb{R}^{m}$ u tački $a\in  D'_{f}\:$ je jednak $L\in \mathbb{R}^{m}\ \:$  $\Big( \lim\limits_{ x \to a }F(x) = L \Big)$ akko $\forall\varepsilon>0 \quad \exists \delta>0 \quad \forall x\in D_{f}\cap\mathring{\mathrm{O}}_{\delta}(a) \quad F(x)\in \mathrm{O}_{\varepsilon}(L)$

$\:$
**Stav**. Neka je $A\subseteq\mathbb{R}^{n}$, $\ \:$ $a\in A'$, $\ \:$  $\forall i=\overline{1,m}\quad f_{i}:\ A\to\mathbb{R}$, $\ \:$ $F:\ A\to\mathbb{R}^{m}$ $\:$ takva da $\:$ $F(x)=\big(f_{1}(x),\,f_{2}(x),\,\dots,\,f_{m}(x)\big)$. Tada
$\lim\limits_{ x \to a }F(x)=(l_{1},\,l_{2},\,\dots,\,l_{m})\quad\Leftrightarrow\quad\forall i=\overline{1,m}\quad\lim\limits_{ x \to a }f_{i}(x)=l_{i}$

$\:$
**Stav**. Neka je $A\subseteq\mathbb{R}^{n}$, $\ \:$ $a\in A$, $\ \:$  $\forall i=\overline{1,m}\quad f_{i}:\ A\to\mathbb{R}$, $\ \:$ $F:\ A\to\mathbb{R}^{m}$ $\:$ takva da $\:$ $F(x)=\big(f_{1}(x),\,f_{2}(x),\,\dots,\,f_{m}(x)\big)$. 
$F$ je neprekidna u tački $a$ ako je $f_{i}$ neprekidna u tački $a$ za $\forall i=\overline{1,m}$

$\:$
> Svojstva limesa i neprekidnosti vektorske funkcije se svode na svojstva koordinatnih funkcija.

$\:$
### Diferencijabilnost
> Napomena: [[Funkcija sa domenom u Rn#Diferencijabilnost|diferencijabilnost]] fje sa kodomenom $\mathbb{R}$.

**Def**. Neka su $D_{f}\subseteq\mathbb{R}^{n}$, $\ \:$  $F:\ D_{f}\to\mathbb{R}^{m}$, $\ \:$ $\mathbf{x}^{0}\in\mathrm{int}\,D_{f}$.
$f$ je **diferencijabilna** u $\mathbf{x}^{0}$ ako postoji linearno preslikavanje $L:\,\mathbb{R}^{n}\to\mathbb{R}^{m}$ takvo da
$\begin{align}F(\mathbf{x}^{0}+\mathbf{h})=F(\mathbf{x}^{0})+L\,\mathbf{h}+\mathbf{o}\big(||\mathbf{h}||\big),\quad \mathbf{h}\to\mathbf{0}\quad\ \ \, &&&&&&&&&&&(1)\end{align}$
gde je $\mathbf{o}(||h||)$ vektor fja $A=(\alpha_{1},\,\alpha_{2},\,\dots,\,\alpha_{m})$, takva da $\forall j=\overline{1,m}\quad \alpha(||\mathbf{h}||)\to0,\quad \mathbf{h}\to0$ 
> $\begin{align}\Leftrightarrow\quad\forall j=\overline{1,m}\quad f_{j}(\mathbf{x}^{0}+\mathbf{h})=f_{j}(\mathbf{x}^{0})+L_{j}\,\mathbf{h}+o\big(||\mathbf{h}||\big),\quad \mathbf{h}\to\mathbf{0}&&(2)\end{align}$
> gde je $L_{j}:\ \mathbb{R}^{n}\to\mathbb{R}$ linearno preslikavanje ($j$-ta vrsta matrice $L$).

Preslikavanje $L$ se zove **diferencijal** (izvod) fje $F$ u tački $\mathbf{x}^{0}$ i označava se sa $dF(\mathbf{x}^{0})$. Pri tome matricu tog preslikavanja zovemo **Jakobijevom matricom**, a determinantu te matrice $J_{F}(\mathbf{x}^{0})=\det dF(\mathbf{x}^{0})$ **jakobijanom**.

Iz [[Funkcija sa domenom u Rn#^d2bcd7|posledice]] i $(2)$ dobijamo da
$\begin{align}dF(\mathbf{x}^{0})=\left(\begin{array}{}\frac{\partial f_{1}}{\partial x_{1}}(\mathbf{x}^{0})&\frac{\partial f_{1}}{\partial x_{2}}(\mathbf{x}^{0})&\cdots&\frac{\partial f_{1}}{\partial x_{n}}(\mathbf{x}^{0})\\\frac{\partial f_{2}}{\partial x_{1}}(\mathbf{x}^{0})&\frac{\partial f_{2}}{\partial x_{2}}(\mathbf{x}^{0})&\cdots&\frac{\partial f_{2}}{\partial x_{n}}(\mathbf{x}^{0})\\\cdots&\cdots&\cdots&\cdots\\\frac{\partial f_{m}}{\partial x_{1}}(\mathbf{x}^{0})&\frac{\partial f_{m}}{\partial x_{2}}(\mathbf{x}^{0})&\cdots&\frac{\partial f_{m}}{\partial x_{n}}(\mathbf{x}^{0})\end{array}\right)\end{align}$

**Primedba**. Neka su $D_{f}\subseteq\mathbb{R}^{n}$, $\ \:$  $F:\ D_{f}\to\mathbb{R}^{m}$, $\ \:$ $\mathbf{x}^{0}\in\mathrm{int}\,D_{f}$.
Ako je $F$ linearno preslikavanje onda $dF(\mathbf{x}^{0})=F$

$\:$
**Stav** (diferenciranje složene fje). Neka su $A\subseteq\mathbb{R}^{n}$, $\:$ $B\subseteq\mathbb{R}^{m}$ $\:$ otvoreni skupovi i neka su $F:\ A\to B$, $\ \:$ $G:\ B\to\mathbb{R}^{k}$. $\:$ $\mathbf{x}^{0}\in A$, $\:$ $\mathbf{y}^{0}=F(\mathbf{x}^{0})\in B$. Tada
ako je $F$ diferencijabilna u $\mathbf{x}^{0}$ i $G$ je diferencijabilna u $\mathbf{y}^{0}$ onda je $G\circ F$ diferencijabilna u $\mathbf{x}^{0}$ i važi: $\boxed{d(F\circ G)(\mathbf{x}^{0})=dG(\mathbf{y}^{0})\circ dF(\mathbf{x}^{0})}$
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