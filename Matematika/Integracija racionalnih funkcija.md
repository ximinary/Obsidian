#fax #math #a2 [deo poglavlja [[Neodređeni integral|"neodređeni integral"]]]
$\:$

1. $A,\,a \in \mathbb{R}\quad x\in (-\infty,\,a)\cup(a,\,+\infty)$
   $\:$
  $\begin{align}\int \frac{A}{x-a} \, dx=\binom{t = x - a}{dt = dx}=A\int \frac{1}{t} \, dt=A\ln|t|+C=A\ln|x-a|+C,\quad C\in \mathbb{R}\end{align}$
  $\:$ ^c41ecb
2. $A,\,a \in \mathbb{R}\quad k \in \mathbb{N}\setminus\{ 1 \}\quad x\in (-\infty,\,a)\cup(a,\,+\infty)$
  $\:$
  $\begin{align}\int \frac{A}{(x-a)^{k}} \, dx=\binom{t = x - a}{dt = dx}=A\int \frac{1}{t^{k}} \, dt=\frac{A}{1-k}\cdot\frac{1}{t^{k-1}}+C=\frac{A}{1-k}\cdot\frac{1}{(x-a)^{k-1}}+C,\quad C\in \mathbb{R}\end{align}$
$\:$ ^08e8de
3. $A,\,a \in \mathbb{R}\quad a>0\quad x\in \mathbb{R}$
   $\:$
  $\begin{align}\int \frac{Ax}{x^{2}+a} \, dx=\binom{t = x^{2} + a}{dt = 2x\,dx}=\frac{A}{2}\int \frac{1}{t} \, dt=\frac{A}{2}\ln|t|+C=\frac{A}{2}\ln(x^{2}+a)+C,\quad C\in \mathbb{R}\end{align}$
  $\:$
4. $A,\,a \in \mathbb{R}\quad a>0\quad k \in \mathbb{N}\setminus\{ 1 \}\quad x\in \mathbb{R}$
  $\:$
  $\begin{align}\int \frac{Ax}{(x^{2}+a)^{k}} \, dx=\binom{t = x^{2} + a}{dt = 2x\,dx}=\frac{A}{2}\int \frac{1}{t^{k}} \, dt=\frac{A}{2(1-k)}\cdot\frac{1}{t^{k-1}}+C=\frac{A}{2(1-k)}\cdot\frac{1}{(x^{2}+a)^{k-1}}+C,\quad C\in \mathbb{R}\end{align}$
$\:$
5. $A,\,a \in \mathbb{R}\quad a>0\quad x\in \mathbb{R}$
   $\:$
  $\begin{align}\int \frac{A}{x^{2}+a^{2}} \, dx=\frac{1}{a}\,\mathrm{arctg}\,\frac{x}{a}+C,\quad C\in \mathbb{R}\end{align}$
  $\:$
6. $A,\,a \in \mathbb{R}\quad a>0\quad k \in \mathbb{N}\setminus\{ 1 \}\quad x\in \mathbb{R}$
  $\:$
  $\begin{align}\int \frac{A}{(x^{2}+a^{2})^{k}} \, dx=\binom{t = \frac{x}{a}}{dt = \frac{1}{a}dx}=\frac{A}{a^{2k-1}}\underbrace{\int \frac{1}{(t^{2}+1)^{k}} \, dt}_{I_{n}(t)}\end{align}$
$\:$
$\begin{align}I_{k}(t)=\int \frac{1}{(t^{2}+1)^{k}} \, dt= \left(\begin{array}{}u = \frac{1}{(t^{2}+1)^{k}} & du = \frac{-2kt}{(t^{2}+1)^{k+1}}dt \\ dv = dt & v = t\end{array}\right)=\int u \, dv=\end{align}$
$\begin{align}=uv - \int v \, du= \frac{t}{(t^{2}+1)^{k}} - \int \frac{-2kt^{2}}{(t^{2}+1)^{k+1}}\, dt= \frac{t}{(t^{2}+1)^{k}} +2k \int \frac{(t^{2}+1) - 1}{(t^{2}+1)^{k+1}}\, dt=\end{align}$
$\begin{align}= \frac{t}{(t^{2}+1)^{k}} +2k \underbrace{\int \frac{1}{(t^{2}+1)^{k}}\, dt}_{I_{k}(t)} - 2k \underbrace{\int \frac{1}{(t^{2}+1)^{k+1}}\, dt}_{I_{k+1}(t)}\end{align}$
$\begin{align}\Rightarrow\quad I_{k}(t) = \frac{t}{(t^{2}+1)^{k}} + 2k\, I_{k}(t)-2k\,I_{k+1}(t)\end{align}$
$\begin{align}\Rightarrow\quad 2k\,I_{k+1}(t) = \frac{t}{(t^{2}+1)^{k}} + (2k-1)\, I_{k}(t)\end{align}$
$\begin{align}\Rightarrow\quad I_{k+1}(t) = \frac{t}{2k\,(t^{2}+1)^{k}} + \frac{2k-1}{2k}\, I_{k}(t)\end{align}$
$\:$
$I_{1}(t) = \mathrm{arctg}\,t+C$
$\:$
$\begin{align} I_{2}(t) \xlongequal{k \,= \,1} \frac{t}{2\,(t^{2}+1)^{k}} + \frac{1}{2}\, I_{1}(t)=\frac{t}{2\,(t^{2}+1)^{k}} + \frac{1}{2}\mathrm{arctg}\,t+C\end{align}$
$\:$
$\begin{align} I_{3}(t) \xlongequal{k \,= \,2} \frac{t}{4\,(t^{2}+1)^{k}} + \frac{3}{4}\, I_{2}(t)=\dots\end{align}$
$\:$
7. $M,\,N,\,b,\,c\in \mathbb{R}\quad b^{2}-4c<0\quad x \in \mathbb{R}$
   $\:$
   $\begin{align}\int \frac{Mx+N}{x^{2}+bx+c} \, dx = \int \frac{Mx+N}{\Big( x^{2}+bx+\frac{b^{2}}{4} \Big) + \Big( c-\frac{b^{2}}{4}\Big)} \, dx = \end{align}$
   $\begin{align}\int \frac{M \Big( x+\frac{b}{2} \Big)+\Big(N-\frac{Mb}{2}\Big)}{\Big( x+\frac{b}{2} \Big)^{2} + \Big( c-\frac{b^{2}}{4}\Big)} \, dx = \left(\begin{array}{}t=x+  \frac{b}{2}&&P=N-\frac{Mb}{2}\\dt=dx&&\alpha=\sqrt[]{c-\frac{b^{2}}{4}}\end{array}\right)=\end{align}$
   $\begin{align}=\underbrace{\int \frac{Mt}{t^{2}+\alpha^{2}} \, dt}_{3.} + \underbrace{\int \frac{P}{t^{2}+\alpha^{2}} \, dt}_{5.}=\dots\end{align}$
   $\:$ ^2f2f6f
8. $M,\,N,\,b,\,c\in \mathbb{R}\quad b^{2}-4c<0\quad k \in \mathbb{N}\setminus\{ 1 \}\quad x\in \mathbb{R}$
   $\:$
   $\begin{align}\int \frac{Mx+N}{(x^{2}+bx+c)^{k}} \, dx = \int \frac{Mx+N}{\bigg(\Big( x^{2}+bx+\frac{b^{2}}{4} \Big) + \Big( c-\frac{b^{2}}{4}\Big)\bigg)^{k}} \, dx = \end{align}$
   $\begin{align}\int \frac{M \Big( x+\frac{b}{2} \Big)+\Big(N-\frac{Mb}{2}\Big)}{\bigg(\Big( x+\frac{b}{2} \Big)^{2} + \Big( c-\frac{b^{2}}{4}\Big)\bigg)^{k}} \, dx = \left(\begin{array}{}t=x+  \frac{b}{2}&&P=N-\frac{Mb}{2}\\dt=dx&&\alpha=\sqrt[]{c-\frac{b^{2}}{4}}\end{array}\right)=\end{align}$
   $\begin{align}=\underbrace{\int \frac{Mt}{(t^{2}+\alpha^{2})^{k}} \, dt}_{4.} + \underbrace{\int \frac{P}{(t^{2}+\alpha^{2})^{k}} \, dt}_{6.}=\dots\end{align}$
    ^86d0ee

##### Nalaženje $\begin{align}\int \frac{P(x)}{Q(x)} \, dx \end{align}$, $\quad$ gde su $P$ i $Q$ polinomi, $\mathrm{deg}\,Q\geqslant 1$

- Ako je $\mathrm{deg}\,P < \mathrm{deg}\,Q$ — preći na sledeći korak.
  $\:$
  Ako je $\mathrm{deg}\,P \geqslant\mathrm{deg}\,Q$ — podeliti $P$ sa $Q$:
  $P(x) = S(x)\,Q(x)+P_{1}(x), \quad \mathrm{deg}\,P_{1}<\mathrm{deg}\,Q$. Tada
  $\:$
  $\begin{align}\int \frac{P(x)}{Q(x)} \, dx = \int \frac{S(x)\,Q(x)+P_{1}(x)}{Q(x)} \, dx = \underbrace{\int S(x) \, dx}_{\text{integracija polinoma}} +\underbrace{\int \frac{P_{1}(x)}{Q(x)} \, dx}_{\text{sledeći korak}}\end{align}$
$\:$
- $\begin{align}\int \frac{P(x)}{Q(x)} \, dx \end{align}, \quad \mathrm{deg}\,P < \mathrm{deg}\,Q$
  $\:$
  $\begin{align}Q(x)=&\,q\,(x- a_{1})^{k_{1}}(x-a_{2})^{k_{2}}\cdot\!\cdot\!\cdot(x- a_{s})^{k_{s}}\cdot\\&\cdot(x^{2}+b_{1}\,x+c_{1})^{n_{1}}(x^{2}+b_{2}\,x+c_{2})^{n_{2}}\cdot\!\cdot\!\cdot(x^{2}+b_{t}\,x+c_{t})^{n_{t}}\end{align}$
  $\:$
  $\forall i = \overline{1,s}\quad a_{i}$ je realni koren $Q(x)$ višestrukosti $k_{i}\in\mathbb{N}$
   $\forall j = \overline{1,t}\quad z_{j},\,\overline{z_{j}} \in \mathbb{C\setminus\mathbb{R}}$  su kompleksni koreni $Q(x)$ višestrukosti $n_{i}\in\mathbb{N}$, takvi da $\begin{cases}z_{j}+\overline{z_{j}} = -b_{j}\\ z_{j}\overline{z_{j}} =c_{j} \end{cases}$ $\quad$ $\Big($ važi $\ \ b_{j}^{2} - 4c_{j}<0\, \Big)$ 
$\:$
- $\begin{align}\frac{P(x)}{Q(x)} =&\,\sum\limits_{i=1}^{s}\bigg(\frac{A_{i1}}{x- a_{i}} + \frac{A_{i2}}{(x- a_{i})^{2}} +\dots+ \frac{A_{ik_{i}}}{(x- a_{i})^{k_{i}}} \bigg) +\\&+\sum\limits_{j=1}^{t}\bigg(\frac{M_{j1}x+N_{j1}}{x^{2}+b_{j}x+c_{j}}+\frac{M_{j2}x+N_{j2}}{(x^{2}+b_{j}x+c_{j})^{2}}+\dots+\frac{M_{jn_{j}}x+N_{jn_{j}}}{(x^{2}+b_{j}x+c_{j})^{n_{j}}}\bigg)\end{align}$
  Odrediti sve koeficijente $A_{\cdot\cdot},\,M_{\cdot\cdot},\,N_{\cdot\cdot}$
  $\:$
- Određivanje integrala $\begin{align}\int \frac{P(x)}{Q(x)} \, dx \end{align}$ se svodi na višestruko određivanje integrala [[Integracija racionalnih funkcija#^c41ecb|1.]], [[Integracija racionalnih funkcija#^08e8de|2.]], [[Integracija racionalnih funkcija#^2f2f6f|7.]], [[Integracija racionalnih funkcija#^86d0ee|8.]]  