#fax #math #a2 [deo poglavlja [[Određeni integral|"određeni integral"]]]
$\:$
[[Metode integracije (neodređeni integral)|Metode integracije za neodređeni integral]]
___
**Teorema** (o smene promenljive).
Neka je $f:\ [a,\,b]\to\mathbb{R}$, $\ \:$ $f\,\mathcal{C}\,[a,\,b]$
i neka je $g:\ [\alpha,\,\beta]\to[a,\,b]$, $\ \:$ $g\,\mathcal{C}^{1}\,[\alpha,\,\beta]$
Tada, $\begin{align}\int_{g(\alpha)}^{g(\beta)} f(x) \, dx = \int_{\alpha}^{\beta} \Big((f\circ g)\cdot g'\Big)(t) \, dt=\int_{\alpha}^{\beta} f\big(g(t)\big)\cdot g'(t) \, dt\end{align}$
>Dokaz:
>Neka je $F:\ [a,\,b]\to\mathbb{R}$ primitivna za $f$ na $[a,\,b]$
>Iz [[Veza između određenog integrala i izvoda. Njutn-Lajbnicova formula#^08f509|Njutn-Lajbnicove formule]]:
> $\begin{align}\int_{g(\alpha)}^{g(\beta)} f(x) \, dx =F\big(g(\beta)\big)-F\big(g(\alpha)\big)\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\ \ \,(1)\end{align}$
>  
>  Sa druge strane, neka je $H:\ [\alpha,\,\beta]\to\mathbb{R}$ def. sa $H(t)=F\big(g(t)\big)$
>  $\forall t\in[\alpha,\,\beta]\quad H'(t)=F'\big(g(t)\big)\cdot g'(t)=f\big(g(t)\big)\cdot g'(t)$
>  Tj. $H$ je primitivna za $(f\circ g)\cdot g'$
>  Dakle,
>  $\begin{align}\int_{\alpha}^{\beta} \Big((f\circ g)\cdot g'\Big)(t) \, dt=H(\beta)-H(\alpha)= F\big(g(\beta)\big)-F\big(g(\alpha)\big)\quad\quad\quad (2)\end{align}$
>  
>  Iz $(1)$ i $(2)$ sledi tvrđenje.

$\:$

**Teorema** (o parcijalnoj integraciji).
Neka su $u,v\,\mathcal{C}^{1}\,[a,\,b]$. Tada
$\begin{align}\int_{a}^{b} \big(u\, v'\big)(x) \, dx = \big(u\,v\big)(x)\bigg|_{a}^{b}-\int_{a}^{b} \big(u'\,v\big)(x) \, dx\end{align}$
>Dokaz:
>Iz [[Veza između određenog integrala i izvoda. Njutn-Lajbnicova formula#^08f509|Njutn-Lajbnicove formule]]:
> $\begin{align}\int_{a}^{b} \big(u\,v\big)'(x) \, dx = \big(u\,v\big)(b) - \big(u\,v\big)(a)\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\ \, (1)\end{align}$
> 
> Sa druge strane:
> $\begin{align}\int_{a}^{b} \big(u\,v\big)'(x) \, dx &= \int_{a}^{b} \big(u'\,v+u\,v'\big)(x) \, dx\\&=\int_{a}^{b} \big(u'\,v\big)(x) \, dx+\int_{a}^{b} \big(u\,v'\big)(x) \, dx\end{align}\quad\quad\quad\quad(2)$
>  
>  Iz $(1)$ i $(2)$ sledi tvrđenje.