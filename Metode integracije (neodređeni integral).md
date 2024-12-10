#fax #math #a2 [deo poglavlja [[Neodređeni integral|"neodređeni integral"]]]
$\:$
[[Metode integracije (određeni integral)|Metode integracije za određeni integral]]
___
Napomena: [[Izvod#^fd0bb3|izvod složene funkcije]], [[Izvod#^49dd91|izvod inverzne funkcije]]

Važi: $d \big(g(x)\big)=g'(x)\,dx$

**Teorema** (o smene promenljive 1).
Neka je $F:\ (a,\,b)\to\mathbb{R}$ primitivna za $f:\ (a,\,b)\to\mathbb{R}$ na $(a,\,b)$ i neka je $g: (\alpha,\,\beta)\to(a,\,b)$ — diferencijabilna.
Tada postoji primitivna za funkciju $(f\circ g)\cdot g':\ (\alpha,\,\beta)\to\mathbb{R}$ i važi $\begin{align}\int \Big((f\circ g)\cdot g'\Big)(x) \, dx = \int f\big(g(x)\big)\cdot g'(x) \, dx = F\big(g(x)\big) + C\end{align}$
> Dokaz: $\forall x\in (\alpha,\,\beta)$
> $\Big(F\big(g(x)\big) + C\Big)'=F'\big(g(x)\big)\cdot g'(x)=f\big(g(x)\big)\cdot g'(x)=\Big((f\circ g)\cdot g'\Big)(x)$

Smena 1:
 $\begin{align}\int f\big(g(x)\big)\cdot g'(x) \, dx &= \binom{t = g(x)}{dt = g'(x)\,dx} =\int f(t)\,dt\\\\&=F(t) + C = F\big(g(x)\big) + C\end{align}$
 

$\:$
**Teorema** (o smene promenljive 2).
Neka je $f:\ (a,\,b)\to\mathbb{R}$, neka je $g: (\alpha,\,\beta)\to(a,\,b)$ — diferencijabilna, takva da postoji $g^{-1}:\ (a,\,b)\to(\alpha,\,\beta)$ — diferencijabilna i neka je $H: \ (\alpha,\,\beta)\to\mathbb{R}$ primitivna za $(f\circ g)\cdot g':\ (\alpha,\,\beta)\to\mathbb{R}$.
Tada postoji primitivna za $f$ i važi $\begin{align}\int f(x) \, dx = H\big(g^{-1}(x)\big) + C\end{align}$

Napomena:  $g$ mora da bude bijekcija da ima inverz
> Dokaz: $\forall x\in (\alpha,\,\beta)$
> $\Big(H\big(g^{-1}(x)\big) + C\Big)'=H'\big(g^{-1}(x)\big)\cdot \big(g^{-1}(x)\big)'=$
> $=\Big((f\circ g)\cdot g'\Big)\big(g^{-1}(x)\big)\cdot\big(g^{-1}(x)\big)'=$
> $\begin{align}=f\Big(g\big(g^{-1}(x)\big)\Big)\cdot g'\big(g^{-1}(x)\big)\cdot\frac{1}{g'\big(g^{-1}(x)\big)}=f(x)\end{align}$

Smena 2:
 $\begin{align}\int f(x) \, dx &= \binom{x = g(t)}{dx = g'(t)\,dt} =\int f\big(g(t)\big)\cdot g'(t)\,dt\\\\&=H(t) + C=H\big(g^{-1}(x)\big)+C\end{align}$
$\:$
Prethodne teoreme ukratko:
$\begin{array}{|c|c|c|}\hline \text{funkcija}&\text{njena primitivna}&\text{domen} \to \text{kodomen}\\ \hline f&F\xlongequal{\text{Teorema 2}}H\circ g^{-1}&(a,\,b)\to\mathbb{R}\\\hline g \text{ — difenencijabilna}&&(\alpha,\,\beta)\to(a,\,b)\\\hline (f\circ g)\cdot g'&H \xlongequal{\text{Teorema 1}} F\circ g&(\alpha,\,\beta)\to\mathbb{R}\\\hline\end{array}$

**Teorema** (o parcijalnoj integraciji).
Neka su $u,\,v:\ (a,\,b)\to\mathbb{R}$ diferencijabilne funkcije. Tada $uv':\ (a,\,b)\to\mathbb{R}$ ima primitivnu $\quad\Leftrightarrow\quad$ $u'v:\ (a,\,b)\to\mathbb{R}$ ima primitivnu. Važi $\begin{align}\int u(x)\,v'(x) \, dx = u(x)\,v(x) - \int u'(x)\,v(x) \, dx \end{align}$
Kraće: $\begin{align}\int u \, dv=uv -\int v \, du \end{align}$
> $\forall x\in (a,\,b)$
> $\big(u(x)\,v(x)\big)'=u'(x)\,v(x)+u(x)\,v'(x)$ $\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad$ (1)
> 
> Ako $u'v$ ima primitivnu tada iz (1):
> $u(x)\,v'(x)=\underbrace{\big(u(x)\,v(x)\big)'}_{\text{ima primitivnu}} - \underbrace{u'(x)\,v(x)}_{\text{ima primitivnu}}\:$ — ima primitivnu $\ \ \quad$ (2)
> 
> $\begin{align}\int u(x)\,v'(x) \, dx \xlongequal{\text{(2)}}\int \Big(\big(u(x)\,v(x)\big)' - u'(x)\,v(x)\Big)\, dx=u(x)\,v(x)-\int u'(x)\,v(x) \, dx\end{align}$
