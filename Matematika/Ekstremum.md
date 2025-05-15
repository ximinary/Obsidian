#fax #math #a1 #a3 [deo poglavlja [[Izvod|"izvod"]] i [[Funkcija sa domenom u Rn|"funkcija sa domenom u Rn"]]]


### Ekstremum funkcije jedne promenljive
**Def**. $x_{0}\in \mathrm{int}\, D_{f}$, $f$ ima u $x_{0}\ \  \{\dots|\}$ ako $\exists\mathrm{O}(x_{0})\ \ \forall x\in \mathrm{O}(x_{0})\cap D_{f}\ \ \{|\dots\}$:

$\begin{align}\mathrm{lokalni}\\ \mathrm{ekstrmum}\end{align}\left\{\begin{array}{c | c}
\mathrm{lokalni\ maksimum} & f(x)\leqslant f(x_0) \\
\mathrm{strogi\ lokalni\ maksimum} & f(x)< f(x_0) \\
\mathrm{lokalni\ minimum} & f(x)\geqslant f(x_0) \\
\mathrm{strogi\ lokalni\ minimum} & f(x)> f(x_0) \\
\end{array}\right\}$

$\:$
[[analiza1_2_ferma.png|Teorema]] (Fermaova; nužni uslov lokalnog ekstremuma).
$x_{0}\in \mathrm{int}\,D_{f},\ f\,\mathcal{D}\,x_{0},\ f$ ima lokalni ekstremum u $x_{0}$.
Tada $f'(x_{0})=0$

$\:$
**Def**. Tačka $x_{0}$ za koju važi $f'(x_{0})=0$ zove se **kritična** tačka.
> Skup tačaka ekstremuma je podskup skupa kritičnih tačaka

$\:$
[[analiza1_2_dovoljniUslovEkstremuma.png|Teorema]] (dovoljni uslov lokalnog ekstremuma).
$f\,\mathcal{C}^{k}\,\mathrm{O}(x_{0}),\ \ f'(x_{0})=f''(x_{0})=\dots=f^{(k-1)}(x_{0})=0, \ \ f^{(n)}(x_{0})\ne 0$
1\) $\ \ k$ je paran broj$\ \ \Rightarrow\ \ x_{0}$ je ekstremum
$\quad\:$ ako $f^{(n)}(x_{0})>0$, $\ \ x_{0}$ je minimum
$\quad\:$ ako $f^{(n)}(x_{0})<0$, $\ \ x_{0}$ je maksimum
2\) $\ \ k$ je neparan broj$\ \ \Rightarrow\ \ x_{0}$ nije ekstremum (ali jeste [[Konveksnost i konkavnost|prevojna tačka]])

$\:$
### Ekstremum funkcije više promenljivih
**Def**. $D_{f}\subseteq\mathbb{R}^{n}$, $f:\ D_{f}\to\mathbb{R}$, $\mathbf{x}^{0}\in \mathrm{int}\, D_{f}$,
$f$ ima u $\mathbf{x}^{0}\ \  \{\dots|\}$ ako $\exists\mathrm{O}(\mathbf{x}^{0})\ \ \forall \mathbf{x}\in \mathrm{O}(\mathbf{x}^{0})\cap D_{f}\ \ \{|\dots\}$:

$\begin{align}\mathrm{lokalni}\\ \mathrm{ekstrmum}\end{align}\left\{\begin{array}{c | c}
\mathrm{lokalni\ maksimum} & f(\mathbf{x})\leqslant f(\mathbf{x}^{0}) \\
\mathrm{strogi\ lokalni\ maksimum} & f(\mathbf{x})< f(\mathbf{x}^{0}) \\
\mathrm{lokalni\ minimum} & f(\mathbf{x})\geqslant f(\mathbf{x}^{0}) \\
\mathrm{strogi\ lokalni\ minimum} & f(\mathbf{x})> f(\mathbf{x}^{0}) \\
\end{array}\right\}$

$\:$
**Teorema** (nužni uslov lokalnog ekstremuma).
$\mathbf{x}^{0}\in \mathrm{int}\,D_{f},\ f\,\mathcal{D}\,\mathbf{x}^{0},\ f$ ima lokalni ekstremum u $\mathbf{x}^{0}$.
Tada $\nabla\!f(\mathbf{x}^{0})=\mathbf{0}$

> Dokaz: Neka je $\mathbf{x}^{0}$ lokalni maksimum. Tada $\exists\mathrm{O}(\mathbf{x}^{0})\ \ \forall \mathbf{x}\in \mathrm{O}(\mathbf{x}^{0})\cap D_{f}\ \ \ f(\mathbf{x})\leqslant f(\mathbf{x}^{0})$.
> Tada specijalno $f\left(\begin{array}{}x^{0}_{1}\\\dots\\x^{0}_{i-1}\\x_{i}\\x^{0}_{i+1}\\\dots\\x_{n}\end{array}\right)\leqslant f\left(\begin{array}{}x^{0}_{1}\\\dots\\x^{0}_{i-1}\\x^{0}_{i}\\x^{0}_{i+1}\\\dots\\x_{n}\end{array}\right)$ za svako $i=\overline{1,n}$, gde je $x_{i}$ takvo da $\left(\begin{array}{}x^{0}_{1}\\\dots\\x^{0}_{i-1}\\x_{i}\\x^{0}_{i+1}\\\dots\\x_{n}\end{array}\right)\in\mathrm{O}(\mathbf{x}^{0})\cap D_{f}$. $\quad$ $\varphi_{i}(x_{i}):=f\left(\begin{array}{}x^{0}_{1}\\\dots\\x^{0}_{i-1}\\x_{i}\\x^{0}_{i+1}\\\dots\\x_{n}\end{array}\right)$
> Imamo da fja jedne promenljive $\varphi_{i}$ ima lokalni maksimum u $x^{0}_{i}$
> Iz Fermaove teoreme: $\varphi'_{i}(x^{0}_{i})=f'_{x_{i}}(\mathbf{x}^{0})=0,\quad\forall i=\overline{1,n}$

$\:$
**Def**. Tačka $\mathbf{x}^{0}$ za koju važi $\nabla\!f(\mathbf{x}^{0})=\mathbf{0}$ zove se **kritična** tačka.

$\:$
**Teorema** (dovoljni uslov lokalnog ekstremuma). Neka $f$ ima sve parcijalne izvode do reda 3 u nekoj $\mathrm{O}(\mathbf{x}^{0})$ i neka $\nabla\!f(\mathbf{x}^{0})=\mathbf{0}$. Neka je $\mathbf{q}$ [[Bilinearna i kvadratna forma#Kvadratne forme|kvadratna forma]], koja je [[Bilinearna i kvadratna forma#^ef95f8|pridružena]] [[Funkcija sa domenom u Rn#^39ff87|matrici drugog izvoda]] u $\mathbf{x}^{0}$. Tada
- ako je $\mathbf{q}$ [[Bilinearna i kvadratna forma#^3b0bdd|strogo pozitivna]] onda je $\mathbf{x}^{0}$ lokalni minimum;
- ako je $\mathbf{q}$ [[Bilinearna i kvadratna forma#^8d6aad|strogo negativna]] onda je $\mathbf{x}^{0}$ lokalni maksimum;
- ako je $\mathbf{q}$ [[Bilinearna i kvadratna forma#^0e3137|promenljivog znaka]] onda $\mathbf{x}^{0}$ nije lokalni ekstremum.

> Dokaz: Razvijamo $f$ u [[Tejlorov polinom#Tejlorov polinom funkcije više promenljivih|Tejlorov polinom]] drugog stepena u okolini $\mathbf{x}^{0}$:
> $\begin{align}f(\mathbf{x}^{0}+\mathbf{h})=f(\mathbf{x}^{0})+\underbrace{\sum\limits_{i=1}^{n}f'_{x_{i}}(\mathbf{x}^{0})\,h_{i}}_{=0,\ \ \text{jer }\nabla\!f(\mathbf{x}^{0})=\mathbf{0}}+\frac{1}{2}\sum\limits_{i,\,j=1}^{n}f''_{x_{ij}}(\mathbf{x}^{0})\,h_{i}\,h_{j}+o(||\mathbf{h}||^{2})\end{align}$
> Odakle,
> $\begin{align}f(\mathbf{x}^{0}+\mathbf{h})-f(\mathbf{x}^{0})&=\frac{1}{2}\sum\limits_{i,\,j=1}^{n}f''_{x_{ij}}(\mathbf{x}^{0})\,h_{i}\,h_{j}+o(||\mathbf{h}||^{2})=\\&=||\mathbf{h}||^{2}\bigg(\frac{1}{2}\sum\limits_{i,\,j=1}^{n}f''_{x_{i}x_{j}}(\mathbf{x}^{0})\,\frac{h_{i}}{||\mathbf{h}||}\,\frac{h_{j}}{||\mathbf{h}||}+o(1)\bigg)=\\&=||\mathbf{h}||^{2}\bigg(\frac{1}{2}\mathbf{q}\Big(\frac{\mathbf{h}}{||\mathbf{h}||}\Big)+o(1)\bigg)\end{align}$
> > $\mathbb{S}^{n-1}=\{\mathbf{x}\in\mathbb{R}^{n}\ \ |\ \ ||\mathbf{x}||=1\}$ — skup svih jediničnih vektora
> > Zbog toga što je $\mathbf{q}$ neprekidna, a $\mathbb{S}^{n-1}$ je kompaktan, [[Funkcija sa domenom u Rn#^8e141b|dobijamo]] da $\exists \min\limits_{\mathbf{x}\in\mathbb{S}^{n-1}}\mathbf{q}(\mathbf{x})=:m$ i $\exists \max\limits_{\mathbf{x}\in\mathbb{S}^{n-1}}\mathbf{q}(\mathbf{x})=:M$ 
> 
> - Pretpostavljamo da je $\mathbf{q}$ strogo pozitivna, tada $m>0$ i imamo
> $\begin{align}f(\mathbf{x}^{0}+\mathbf{h})-f(\mathbf{x}^{0})&=||\mathbf{h}||^{2}\bigg(\frac{1}{2}\mathbf{q}\Big(\frac{\mathbf{h}}{||\mathbf{h}||}\Big)+o(1)\bigg)\geqslant||\mathbf{h}||^{2}\bigg(\frac{1}{2}m+o(1)\bigg)\to0^{+},\quad\mathbf{h}\to0\end{align}$
> tj. $\exists \mathrm{O}(\mathbf{x}^{0})\quad \forall \mathbf{x}\in\mathrm{O}(\mathbf{x}^{0})\quad f(\mathbf{x})\geqslant f(\mathbf{x}^{0})$
> $\:$
> - Pretpostavljamo da je $\mathbf{q}$ strogo negativna, tada $M<0$ i imamo
> $\begin{align}f(\mathbf{x}^{0}+\mathbf{h})-f(\mathbf{x}^{0})&=||\mathbf{h}||^{2}\bigg(\frac{1}{2}\mathbf{q}\Big(\frac{\mathbf{h}}{||\mathbf{h}||}\Big)+o(1)\bigg)\leqslant||\mathbf{h}||^{2}\bigg(\frac{1}{2}M+o(1)\bigg)\to0^{-},\quad\mathbf{h}\to0\end{align}$
> tj. $\exists \mathrm{O}(\mathbf{x}^{0})\quad \forall \mathbf{x}\in\mathrm{O}(\mathbf{x}^{0})\quad f(\mathbf{x})\leqslant f(\mathbf{x}^{0})$
> $\:$
> - Pretpostavljamo da je $\mathbf{q}$ promenljivog znaka,
> tj. $\exists \mathbf{h},\,\mathbf{k}\in\mathbb{R}^{n}\ \ \:\ \ \mathbf{q}(\mathbf{h})>0\ \text{ i } \ \mathbf{q}(\mathbf{k})<0$
> Neka je $a:=\mathbf{q}(\mathbf{h})$, $b:=\mathbf{q}(\mathbf{k})$
> Tada, $\begin{align}\forall \varepsilon>0\quad \mathbf{q}(\varepsilon\,\mathbf{h})=\varepsilon^{2}\mathbf{q}(\mathbf{h})=\varepsilon^{2}a>0\\\forall \varepsilon>0\quad \mathbf{q}(\varepsilon\,\mathbf{k})=\varepsilon^{2}\mathbf{q}(\mathbf{k})=\varepsilon^{2}b<0\end{align}$
> Odakle, $\begin{align}f(\mathbf{x}^{0}+\varepsilon\,\mathbf{h})-f(\mathbf{x}^{0})=\bigg(\frac{1}{2}\mathbf{q}\Big(\varepsilon\,\mathbf{h}\Big)+o(||\varepsilon\,\mathbf{h}||^{2})\bigg)=\varepsilon^{2}\bigg(\frac{1}{2}a+o(1)\bigg)>0, \quad\varepsilon\to0\\f(\mathbf{x}^{0}+\varepsilon\,\mathbf{k})-f(\mathbf{x}^{0})=\bigg(\frac{1}{2}\mathbf{q}\Big(\varepsilon\,\mathbf{k}\Big)+o(||\varepsilon\,\mathbf{k}||^{2})\bigg)=\varepsilon^{2}\bigg(\frac{1}{2}b+o(1)\bigg)<0, \quad\varepsilon\to0\end{align}$
> tj. u svakoj $\varepsilon$-okolini tačke $\mathbf{x}^{0}$ postoje $\mathbf{x}^{1}:=\mathbf{x}^{0}+\mathbf{h}$ $\:$ i $\:$ $\mathbf{x}^{2}:=\mathbf{x}^{0}+\mathbf{k}$ takve da $f(\mathbf{x}^{1})>0$ $\:$ i $\:$ $f(\mathbf{x}^{2})<0$, tj. $\mathbf{x}^{0}$ nije ekstremum.

$\:$
> Napomena: [[Bilinearna i kvadratna forma#^fd4794|dokazivanje pozitivnosti/negativnosti kvadratne forme]]


$\:$
**Def**. Ako je $\mathbf{x}^{0}$ kritična tačka $\Big(\nabla\!f(\mathbf{x}^{0})=\mathbf{0}\Big)$, ali u svakoj njenoj okolini postoje tačke u kojima $f$ uzima i veće i manje vrednosti od $f(\mathbf{x}^{0})$, onda je $\mathbf{x}^{0}$ **sedlo**.

### Uslovni ekstremum
**Def**. Neka je $f$ definisana na $S\subset\mathbb{R}^{n}$, a $S$ je zadat pomoću sistema jednačina $\begin{cases}\varphi_{1}(x_{1},\,\dots,\,x_{n})=0\\\varphi_{2}(x_{1},\,\dots,\,x_{n})=0\\\dots\\\varphi_{m}(x_{1},\,\dots,\,x_{n})=0\end{cases}$. Funkcija $f$ ima **uslovni** lokalni ekstremum na skupu $S$ u tački $\mathbf{x}^{0}$ ako $f\big|_{S}$ ima lokalni ekstremum u $\mathbf{x}^{0}$.

$\:$
**Teorema**. Neka je skup $S$ zadat pomoću sistema jednačina $\begin{cases}\varphi_{1}(\mathbf{x})=0\\\varphi_{2}(\mathbf{x})=0\\\dots\\\varphi_{m}(\mathbf{x})=0\end{cases}$, pri tome fja $\varphi_{i}$ je diferencijabilna za $\forall i=\overline{1,n}$ i skup vektora $\Big\{\nabla\varphi_{i}(\mathbf{x})\ \Big|\ i=\overline{1,n}\Big\}$ je linearno nezavisan za $\forall\mathbf{x}\in S$. Neka je $f$ diferencijabilna na nekom otvorenom skupu $I$ takvom da $S\subseteq I$ i neka je $\mathbf{x}^{0}$ lokalni ekstremum fje $f\big|_{S}$. Tada
$\exists\lambda_{1},\,\dots,\,\lambda_{m}\in\mathbb{R}\ \ :\ \ \nabla\!f(\mathbf{x}^{0})=\lambda_{1}\,\nabla\varphi_{1}(\mathbf{x}^{0})+\dots+\lambda_{m}\,\nabla\varphi_{m}(\mathbf{x}^{0})$
(Brojeve $\lambda_{1},\,\dots,\,\lambda_{m}$ se nazivaju **Lagranževi množioci**)
> Dokaz: razmotrimo dva osnovna slučaja, koje je moguće generalizovati.
> - Slučaj $n = 3,\ \  m = 1\:$ — površ u prostoru.
> 
> Neka je površ $S$ data jednačinom $\varphi(x,\,y,\,z)=0$; linearna nezavisnost skupa $\Big\{\nabla\varphi(x,\,y,\,z)\Big\}$ za $\forall(x,\,y,\,z)\in S$ daje da $\nabla\varphi(x,\,y,\,z)\ne (0,\,0,\,0)$, tj $S$ je [[Regularna kriva i tangenta. Regularna površ i tangentna površ#^5afd44|regularna površ]].
> Neka je $(x_{0},\,y_{0},\,z_{0})$ tačka lokalnog ekstremuma fje $f\big|_{S}$ i neka je $\mathbf{r}:\ (t_{0}-\varepsilon,\,t_{0}+\varepsilon)\to\mathbb{R}^{3}$ [[Regularna kriva i tangenta. Regularna površ i tangentna površ#^f25bf0|regularna kriva]] na površi $S$ takva da $\mathbf{r}(t_{0})=(x_{0},\,y_{0},\,z_{0})$.
> Zbog toga što $\mathbf{r}$ leži u $S$ i $(x_{0},\,y_{0},\,z_{0})$ je ekstremum $f$ na $S$, dobijamo da je $t_{0}$ ekstremum fje $f\circ\mathbf{r}$, odakle $(f\circ\mathbf{r})'(t_{0})=0$. 
> 
> Iz [[Preslikavanje sa vrednostima u Rm#^4816ca|stava]], $0=(f\circ \mathbf{r})'(t_{0})=df\big(\mathbf{r}(t_{0})\big)\, d\mathbf{r}(t_{0})=\nabla\!f(x_{0},\,y_{0},\,z_{0})\cdot \mathbf{r}'(t_{0})$
> tj. $\nabla\!f(x_{0},\,y_{0},\,z_{0})\perp \mathbf{r}'(t_{0})$
> Iz [[Regularna kriva i tangenta. Regularna površ i tangentna površ#^635980|stava]] $\nabla\varphi(x_{0},\,y_{0},\,z_{0})\perp \mathbf{r}'(t_{0})$
> 
> Odakle, $\exists \lambda\in\mathbb{R}\ \ :\ \ \nabla\!f(x_{0},\,y_{0},\,z_{0})=\lambda \nabla\varphi(x_{0},\,y_{0},\,z_{0})$
>
> - Slučaj $n = 3,\ \  m = 2\:$ — kriva u prostoru.
>
>Neka je kriva $S$ data sa $\begin{cases}\varphi_{1}(x,\,y,\,z)=0\\\varphi_{2}(x,\,y,\,z)=0\end{cases}$ $\:$ tj. kao presek dve površi; skup $\Big\{\nabla\varphi_{1}(x,\,y,\,z),\ \nabla\varphi_{2}(x,\,y,\,z)\Big\}$ je linearno nezavisan za $\forall(x,\,y,\,z)\in S$ odakle vidimo da je $S$ presek dve regularne površi, tj. jeste [[Regularna kriva i tangenta. Regularna površ i tangentna površ#^f25bf0|regularna kriva]], koju parametrizujemo sa $\mathbf{r}(t)$.
> Neka je $(x_{0},\,y_{0},\,z_{0})$ tačka lokalnog ekstremuma fje $f\big|_{S}$ i neka važi $\mathbf{r}(t_{0})=(x_{0},\,y_{0},\,z_{0})$. Tada je $t_{0}$ ekstremum fje $f\circ\mathbf{r}$, odakle $(f\circ\mathbf{r})'(t_{0})=0$. 
> 
> Iz [[Preslikavanje sa vrednostima u Rm#^4816ca|stava]], $0=(f\circ \mathbf{r})'(t_{0})=df\big(\mathbf{r}(t_{0})\big)\, d\mathbf{r}(t_{0})=\nabla\!f(x_{0},\,y_{0},\,z_{0})\cdot \mathbf{r}'(t_{0})$
> tj. $\nabla\!f(x_{0},\,y_{0},\,z_{0})\perp \mathbf{r}'(t_{0})$ 
> Iz [[Regularna kriva i tangenta. Regularna površ i tangentna površ#^635980|stava]] $\begin{align}\nabla\varphi_{1}(x_{0},\,y_{0},\,z_{0})\perp \mathbf{r}'(t_{0})\\\nabla\varphi_{2}(x_{0},\,y_{0},\,z_{0})\perp \mathbf{r}'(t_{0})\end{align}$
> Odakle, $\nabla\!f(x_{0},\,y_{0},\,z_{0}),\ \nabla\varphi_{1}(x_{0},\,y_{0},\,z_{0}),\ \nabla\varphi_{2}(x_{0},\,y_{0},\,z_{0})$ su linearno zavisni, tj. $\exists \lambda_{1},\,\lambda_{2}\in\mathbb{R}\ \ :\ \ \nabla\!f(x_{0},\,y_{0},\,z_{0})=\lambda_{1}\nabla\varphi_{1}(x_{0},\,y_{0},\,z_{0})+\lambda_{2}\nabla\varphi_{2}(x_{0},\,y_{0},\,z_{0})$

$\:$
> Napomena:
> Neka je $f:\ \mathbb{R}^{n}\to\mathbb{R}$
> 
> Uslove $\begin{cases}\nabla\!f(\mathbf{x})=\lambda_{1}\nabla\varphi_{1}(\mathbf{x})+\lambda_{2}\nabla\varphi_{2}(\mathbf{x})+\dots+\lambda_{m}\nabla\varphi_{m}(\mathbf{x})\\\varphi_{1}(\mathbf{x})=0\\\varphi_{2}(\mathbf{x})=0\\\dots\\\varphi_{m}(\mathbf{x})=0\\\end{cases}$
> možemo zameniti uslovom $dF(\mathbf{x},\,\lambda_{1},\,\lambda_{2},\,\dots,\,\lambda_{m})=0$, gde je 
> $F:\ \mathbb{R}^{n+m}\to\mathbb{R}$ $\ \:$ def. sa $\ \:$  $F(\mathbf{x},\,\lambda_{1},\,\lambda_{2},\,\dots,\,\lambda_{m})=f(\mathbf{x})-\Big[\lambda_{1}\varphi_{1}(\mathbf{x})+\lambda_{2}\varphi_{2}(\mathbf{x})+\dots+\lambda_{m}\varphi_{m}(\mathbf{x})\Big]$
> 
> 