#fax #math #a1 [deo poglavlja [[Limes funkcije|"limes funkcije"]]]  
$\:$

**Def**. Neka su $f,\,g:D\to\mathbb{R}$ funkcije, $a\in \mathrm{int}\, D$ 

| Oznaka                   | Definicija                                                                                                                                                                             |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| $f=o(g),\ \ x\to a$      | $\forall \varepsilon>0\quad \exists\delta>0 \quad \forall x\in \mathring{\mathrm{O}}_{\delta}(a)\quad \mid\!\!f(x)\!\!\mid \, <\varepsilon\!\mid\!\!g(x)\!\!\mid$                      |
| $f=\omega(g),\ \ x\to a$ | $\forall \varepsilon>0\quad \exists\delta>0 \quad \forall x\in \mathring{\mathrm{O}}_{\delta}(a)\quad \mid\!\!f(x)\!\!\mid\, >\varepsilon\!\mid\!\!g(x)\!\!\mid$                       |
| $f=O(g),\ \ x\to a$      | $\exists c>0,\ \delta>0 \quad \forall x\in \mathring{\mathrm{O}}_{\delta}(a)\quad \mid\!\!f(x)\!\!\mid\,\leqslant c\!\mid\!\!g(x)\!\!\mid$                                             |
| $f=\Omega(g),\ \ x\to a$ | $\exists c>0,\ \delta>0 \quad \forall x\in \mathring{\mathrm{O}}_{\delta}(a)\quad \mid\!\!f(x)\!\!\mid\,\geqslant c\!\mid\!\!g(x)\!\!\mid$                                             |
| $f=\Theta(g),\ \ x\to a$ | $\exists c>0,\ c'>0,\ \delta>0 \quad \forall x\in \mathring{\mathrm{O}}_{\delta}(a)\quad c\!\mid\!\!g(x)\!\!\mid\,\leqslant\,\mid\!\!f(x)\!\!\mid\,\leqslant c'\!\mid\!\!g(x)\!\!\mid$ |

**Def**. $f,\,g:D\to\mathbb{R}$ su funkcije, $a\in \mathrm{int}\, D$. Tada $f\sim g,\ \ x\to a\quad\Leftrightarrow$
$\Leftrightarrow\quad\exists\alpha:D\to \mathbb{R}$ tako da $\lim\limits_{ x \to a }\alpha(x)=1\:$ i $\ f(x)=\alpha(x)\cdot g(x)$

### Svojstva $o$
Stav. $f,\,g:D\to\mathbb{R}$ su funkcije, $a\in \mathrm{int}\, D$. Tada $f=o(g),\ \ x\to a\quad\Leftrightarrow$
$\Leftrightarrow\quad\exists\varepsilon:D\to \mathbb{R}$ tako da $\lim\limits_{ x \to a }\varepsilon(x)=0\:$ i $\ f(x)=\varepsilon(x)\cdot g(x)$

Za $\alpha,\,\beta>0$ važi:
- $x^{\alpha} = o(x^{\beta}),\ \ x\to 0\quad \Leftrightarrow\quad \alpha>\beta$
- $x^{\alpha} = o(x^{\beta}),\ \ x\to +\infty\quad \Leftrightarrow\quad \alpha<\beta$

[[analiza1_1_10.png|Stav]]. Svojstva $o$:
1. $o(f)+o(f)=o(f),\ \ x\to a$
2. $\lambda\, o(f)=o(f),\ \ x\to a$
3. $f\!\cdot\! o(g)=o(f\,g),\ \ x\to a$
4. $o(f)\!\cdot\! o(g)=o(f\,g),\ \ x\to a$

### Svojstva $\sim$. Veza između $o$ i $\sim$
[[analiza1_1_11.png|Stav]]. $\sim$ je [[Relacija ekvivalencije|relacija ekvivalencije]]

[[analiza1_1_12_1.png|Stav]]. $f\sim g,\ \ x\to a\quad\Rightarrow\quad o(f)=o(g),\ \ x\to a$
[[analiza1_1_12_2.png|Stav]]. $f\sim g,\ \ x\to a\quad\Leftrightarrow\quad f(x)=g(x)+o(g(x)),\ \ x\to a$

>Primer:
>$P_{n}(x)\sim Q_{n}(x),\ \ x\to+\infty$, 
>ako $P_{n}=ax^{n}+a_{n-1}x^{n-1}+\dots$ i $Q_{n}=ax^{n}+b_{n-1}x^{n-1}+\dots$

$\:$
### [[Osnovni limesi]] na jeziku $\sim$ i $o$
kod $x\to 0$ važe
$\begin{array}{|c|c|} 
	\hline
	\sin\,x\sim x & \sin x = x+o(x)\\ 
	\hline
	1-\cos\,x\sim\frac{x^2}{2} & 1-\cos x = \frac{x^2}{2} + o(x^2)\\
	& \cos x= 1-\frac{x^2}{2} + o(x^2)\\
	\hline
	\ln(1+x)\sim x & \ln(1+x)=x+o(x) \\
	\hline
	e^x-1\sim x & e^x-1 = x+o(x) \\
	& e^x =1+ x+o(x) \\
	\hline
	a^x-1\sim x\,\ln a & a^x -1 =x\ln\,a+o(x) \\
	& a^x =1+ x\ln\,a+o(x) \\
	\hline
	(1+x)^\alpha-1\sim \alpha\,x & (1+x)^\alpha-1= \alpha\,x +o(x)\\
	& (1+x)^\alpha=1+\alpha\,x +o(x)\\
	\hline
\end{array}$ ^000000

### [[Složenost algoritma]]