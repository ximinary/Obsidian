#fax #math #a3 [deo [[Analiza|analize]]]
$\:$
**Def**. Neka su $D_{f}\subseteq\mathbb{R}^{n}$, $\ \:$  $f:\ D_{f}\to\mathbb{R}$, $\ \:$ $\mathbf{x}^{0}=(x^{0}_{1},\,x^{0}_{2},\,\dots,\,x^{0}_{n})\in\mathrm{int}\,D_{f}$. Tada ako $\begin{align}\exists  \lim\limits_{ h \to 0 }\frac{f(x^{0}_{1},\,\dots,\,x^{0}_{i}+h,\,\dots,\,x^{0}_{n})-f(x^{0}_{1},\,\dots,\,x^{0}_{i},\,\dots,\,x^{0}_{n})}{h} := f'_{x_{i}}(\mathbf{x}^{0})=\frac{\partial f}{\partial x_{i}}(\mathbf{x}^{0}) \end{align}$,
 on se zove **parcijalni izvod** fje $f$ po $x_{i}$ u tački $\mathbf{x}^{0}$

$\:$
**Def**. Neka su $D_{f}\subseteq\mathbb{R}^{n}$, $\ \:$  $f:\ D_{f}\to\mathbb{R}$, $\ \:$ $\mathbf{x}^{0}\in\mathrm{int}\,D_{f}$ $\:$ i $\:$ $\mathbf{v}\in\mathbb{R}^{n}$ takav da $||\mathbf{v}||=1$. Tada ako $\begin{align}\exists  \lim\limits_{ h \to 0 }\frac{f(\mathbf{x}^{0}+h\,\mathbf{v})-f(\mathbf{x}^{0})}{h} := f'_{\mathbf{v}}(\mathbf{x}^{0})=\frac{\partial f}{\partial \mathbf{v}}(\mathbf{x}^{0})\end{align}$,
 on se zove **izvod u pravcu** vektora $\mathbf{v}$ fje $f$ u tački $\mathbf{x}^{0}$

> Napomena: parcijalni izvod po $x_{i}$ je izvod u pravcu vektora $\mathbf{e}_{i}=(0,\,0,\,\dots,\,0,\,\overset{i}{1},\,0,\,\dots,\,0,\,0)$ 
> tj. $\begin{align}\frac{\partial f}{\partial x_{i}}(\mathbf{x}^{0})=\frac{\partial f}{\partial \mathbf{e}_{i}}(\mathbf{x}^{0})\end{align}$

$\:$
**Def**. Parcijalni izvod drugog reda:
$\begin{align}f''_{x_{i}x_{j}}=\frac{\partial^{2} f}{\partial x_{j}\,\partial x_{i}}:=\big(f'_{x_{i}}\big)'_{x_{j}}=\frac{\partial }{\partial x_{j}}\bigg(\frac{\partial f}{\partial x_{i}}\bigg)\end{align}$ 
Analogno se definišu parcijalni izvodi višeg (3, 4, ...) reda.
Pri tome $\begin{align}f^{(0)}=\partial^{0}f=f\end{align}$

$\:$
**Stav**. Ako na $\mathrm{O}(\mathbf{x}^{0})$ postoje parcijalni izvodi $f''_{x_{i}x_{j}}$ i $f''_{x_{j}x_{i}}$, koje su neprekidne u $\mathbf{x}^{0}$ onda $f''_{x_{i}x_{j}}(\mathbf{x}^{0})=f''_{x_{j}x_{i}}(\mathbf{x}^{0})$

$\:$
**Def**. Hesijan (ili matrica drugog izvoda) fje $f$ u $\mathbf{x}^{0}$ je
$Hf(\mathbf{x}^{0})=d^{2}f(\mathbf{x}^{0})=\left(\begin{array}{}f''_{x_{1}x_{1}}(\mathbf{x}^{0})&f''_{x_{1}x_{2}}(\mathbf{x}^{0})&\dots&f''_{x_{1}x_{n}}(\mathbf{x}^{0})\\f''_{x_{2}x_{1}}(\mathbf{x}^{0})&f''_{x_{2}x_{2}}(\mathbf{x}^{0})&\dots&f''_{x_{2}x_{n}}(\mathbf{x}^{0})\\\dots&\dots&\dots&\dots\\f''_{x_{n}x_{1}}(\mathbf{x}^{0})&f''_{x_{n}x_{2}}(\mathbf{x}^{0})&\dots&f''_{x_{n}x_{n}}(\mathbf{x}^{0})\end{array}\right)$ ^39ff87

### Operator nabla
**Def**. Neka su $D_{f}\subseteq\mathbb{R}^{n}$, $\ \:$  $f:\ D_{f}\to\mathbb{R}$, $\ \:$ $\mathbf{x}^{0}\in\mathrm{int}\,D_{f}$.
Vektor  $\nabla\!f(\mathbf{x}^{0})=\Big(f'_{x_{1}}(\mathbf{x}^{0}),\ \ f'_{x_{2}}(\mathbf{x}^{0}),\ \ \cdots,\ \ f'_{x_{n}}(\mathbf{x}^{0})\Big)$ zove se **gradijent** fje $f$ u tački $\mathbf{x}^{0}$.

$\nabla$ zove se **operator nabla**. $\begin{align}\nabla=\bigg(\frac{\partial}{\partial x_{1}},\ \frac{\partial}{\partial x_{2}},\ \dots,\ \frac{\partial}{\partial x_{n}}\bigg)\end{align}$, gde je $n$ dimenzija domena funkcije na koju se primenjuje. 

### [[Tejlorov polinom funkcije više promenljivih|Tejlorov polinom]]