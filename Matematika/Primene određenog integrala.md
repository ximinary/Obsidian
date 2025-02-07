#fax #math #a2 [deo poglavlja [[Određeni integral|"određeni integral"]]]

### Površina figure između dve krive
**Teorema**. Neka su $f,\,g:\ [a,\,b]\to\mathbb{R}$ neprekidne, takve da $\forall x\in[a,\,b]\quad f(x)\geqslant g(x)$.

Figura ograničena sa $f$ i $g$ na intervalu $[a,\,b]$ je
$\Phi=\Big\{ (x,\,y) \ \ \Big|\ \ a\leqslant x\leqslant b\quad g(x)\leqslant y\leqslant f(x)\Big\}$

Tada je površina te figure jednaka
$\begin{align}P(\Phi)=\int_{a}^{b} \Big(f(x)-g(x)\Big) \, dx\end{align}$
### Dužina krive
**Teorema**. Neka je $f:\ [a,\,b]\to\mathbb{R}$ takva da $f\,\mathcal{C}^{1}\,[a,\,b]$.
Tada je dužina krive $f$ jednaka $\begin{align}L=\int_{a}^{b} \sqrt[]{1+\big(f'(x)\big)^{2}} \, dx\end{align}$

> Dokaz: Neka je $\mathcal{P}$ [[Određeni integral#^fbc37a|podela]] intervala $[a,\,b]$
> Rastojanje između tačaka $\Big(x_{i-1},\,f(x_{i-1})\Big)$ i $\Big(x_{i},\,f(x_{i})\Big)$ je 
> $L_{i}=\sqrt[]{\Big(x_{i} - x_{i-1}\Big)^{2}+\Big(f(x_{i}) - f(x_{i-1})\Big)^{2}} =$
> $\begin{align}=(x_{i} - x_{i-1})\sqrt[]{1+\bigg(\frac{f(x_{i}) - f(x_{i-1})}{x_{i} - x_{i-1}}\bigg)^{2}},\quad\quad\forall i = \overline{1,n}\end{align}$
> 
> Iz [[Teoreme o srednjoj vrednosti#^e52da5|Lagranževe teoreme]]:
> $\begin{align}\forall i = \overline{1,n}\quad\exists\xi_{i}\in(x_{i-1},\,x_{i})\ \ :\ \ f'(\xi_{i})=\frac{f(x_{i}) - f(x_{i-1})}{x_{i} - x_{i-1}}\end{align}$
> Uzimamo $\xi=(\xi_{1},\,\xi_{2},\,\dots,\,\xi_{n})$ kao podeone tačke podele.
> 
> Dužina krive:
> $\begin{align}L = \lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sum\limits_{i=1}^{n}L_{i}= \lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sum\limits_{i=1}^{n} (x_{i} - x_{i-1})\sqrt[]{1+\big(f'(\xi_{i})\big)^{2}} = \end{align}$
> $\begin{align}=\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sigma\bigg(\sqrt[]{1+\big(f'(x)\big)^{2}},\ \mathcal{P},\ \xi\bigg)=\int_{a}^{b} \sqrt[]{1+\big(f'(x)\big)^{2}} \, dx\end{align}$
> 
> Limes postoji jer je $\sqrt[]{1+\big(f'(x)\big)^{2}}$ neprekidna a samim tim i Riman-integrabilna.

^6fea35

$\:$
**Teorema**. Neka je $f$ funkcija koja je zadata parametarski $x = x(t),\ \ y=y(t), \ \ t\in[\alpha,\,\beta]$ i neka važi  $x,\,y\,\mathcal{C}^{1}\,(a,\,b)$.
Tada je dužina krive $f$ jednaka $\begin{align}L=\int_{\alpha}^{\beta} \sqrt[]{\big(x'(t)\big)^{2}+\big(y'(t)\big)^{2}} \, dt\end{align}$

### Zapremina tela dobijenog rotiranjem krive
**Teorema**. Neka je $f:\ [a,\,b]\to\mathbb{R}$ pozitivna i važi $f\,\mathcal{C}\,[a,\,b]$.
Tada je zapremina tela dobijenog rotiranjem krive $f$ oko ose $\mathrm{O}x$ jednaka $\begin{align}V=\pi\int_{a}^{b} \big(f(x)\big)^{2} \, dx\end{align}$

> Dokaz: Neka je $(\mathcal{P},\,\xi)$ [[Određeni integral#^fbc37a|podela]] sa istaknutim tačkama intervala $[a,\,b]$.
> Zapremina na svakom od intervala $[x_{i-1},\,x_{i}]$ bi bila otprilike jednaka površine kruga sa poluprečnikom $f(\xi_{i})$ pomnožene dužinom intervala:
>  $V_{i}=\pi\big(f(\xi_{i})\big)^{2}\cdot(x_{i}-x_{i-1}), \quad \forall i=\overline{1,n}$
>  
>  Zapremina tela:
>  $\begin{align}V = \lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sum\limits_{i=1}^{n}V_{i}= \lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sum\limits_{i=1}^{n} \pi\big(f(\xi_{i})\big)^{2}\cdot(x_{i}-x_{i-1})= \end{align}$
> $\begin{align}=\pi\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sigma\bigg(\big(f(x)\big)^{2},\ \mathcal{P},\ \xi\bigg)=\pi\int_{a}^{b} \big(f(x)\big)^{2} \, dx\end{align}$
> 
> Limes postoji jer je $\big(f(x)\big)^{2}$ neprekidna a samim tim i Riman-integrabilna.

$\:$
**Teorema**. Neka je $f$ funkcija koja je zadata parametarski $x = x(t),\ \ y=y(t), \ \ t\in[\alpha,\,\beta]$ i neka važi  $x,\,y\,\mathcal{C}\,(a,\,b)$.
Tada je zapremina tela dobijenog rotiranjem krive $f$ oko ose $\mathrm{O}x$ jednaka $\begin{align}V=\int_{\alpha}^{\beta} \big(y(t)\big)^{2}x'(t) \, dt\end{align}$

### Površina omotača tela dobijenog rotiranjem krive
**Teorema**. Neka je $f:\ [a,\,b]\to\mathbb{R}$ takva da $f\,\mathcal{C}^{1}\,[a,\,b]$.
Tada je površina omotača tela dobijenog rotiranjem krive $f$ oko ose $\mathrm{O}x$ jednaka  $\begin{align}S=2\pi\int_{a}^{b} f(x) \sqrt[]{1+\big(f'(x)\big)^{2}} \, dx\end{align}$
> Dokaz: Neka je $(\mathcal{P},\,\xi)$ [[Određeni integral#^fbc37a|podela]] sa istaknutim tačkama intervala $[a,\,b]$.
> Površina na svakom od intervala $[x_{i-1},\,x_{i}]$ bi bila otprilike jednaka površine omotača zarubljene kupe sa poluprečnicima $f(x_{i-1})$, $f(x_{i})$ i izvodnice sa dužinom $L_{i}$:
>  $S_{i}=\pi\big(f(x_{i-1})+f(x_{i})\big)\cdot L_{i}, \quad \forall i=\overline{1,n}$
> 
> U [[Primene određenog integrala#^6fea35|teoremi u kojoj se izvodi dužina krive]] definisali smo $L_{i}$ i izrazili sa:
> $\begin{align}L_{i}=(x_{i} - x_{i-1})\sqrt[]{1+\big(f'(\xi_{i})\big)^{2}},\quad\quad\forall i = \overline{1,n}\quad \xi_{i}\in[x_{i-1},\,x_{i}]\end{align}$
> 
> Površina omotača tela:
> $\begin{align}S = \lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sum\limits_{i=1}^{n}S_{i}= \lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sum\limits_{i=1}^{n} \pi\big(f(x_{i-1})+f(x_{i})\big)\cdot(x_{i} - x_{i-1})\sqrt[]{1+\big(f'(\xi_{i})\big)^{2}}= \end{align}$
> > Zbog neprekidnosti $f$ iz [[Neprekidnost#^1b740a|teoreme o međuvrednosti]]:
> > $\forall i=\overline{1,n}\quad \exists\eta_{i}\in[x_{i-1},\,x_{i}] \ \ :\ \ 2f(\eta_{i})=f(x_{i-1})+f(x_{i})$
> 
> $\begin{align}=\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sum\limits_{i=1}^{n}\pi\cdot2f(\eta_{i})\cdot(x_{i} - x_{i-1})\sqrt[]{1+\big(f'(\xi_{i})\big)^{2}}=\end{align}$
> $\begin{align}=\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sum\limits_{i=1}^{n}2\pi f(\xi_{i})\cdot(x_{i} - x_{i-1})\sqrt[]{1+\big(f'(\xi_{i})\big)^{2}}+\underbrace{\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sum\limits_{i=1}^{n}2\pi \big(f(\eta_{i})-f(\xi_{i})\big)\cdot(x_{i} - x_{i-1})\sqrt[]{1+\big(f'(\xi_{i})\big)^{2}}}_{=0}=\end{align}$
> $\begin{align}=2\pi\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sigma\bigg(f(x) \sqrt[]{1+\big(f'(x)\big)^{2}},\ \mathcal{P},\ \xi\bigg)=2\pi\int_{a}^{b} f(x) \sqrt[]{1+\big(f'(x)\big)^{2}} \, dx\end{align}$
> 
> Limes postoji jer je $f(x)\sqrt[]{1+\big(f'(x)\big)^{2}}$ neprekidna a samim tim i Riman-integrabilna.

$\:$
**Teorema**. Neka je $f$ funkcija koja je zadata parametarski $x = x(t),\ \ y=y(t), \ \ t\in[\alpha,\,\beta]$ i neka važi  $x,\,y\,\mathcal{C}^{1}\,(a,\,b)$.
Tada je dužina krive $f$ jednaka $\begin{align}L=2\pi\int_{\alpha}^{\beta} y(t)\sqrt[]{\big(x'(t)\big)^{2}+\big(y'(t)\big)^{2}} \, dt\end{align}$