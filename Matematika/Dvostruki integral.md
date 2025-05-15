#fax #math #a3 [deo [[Analiza|analize]]]

### Podela pravougaonika
**Def**. Neka su $a=x_{0}<x_{1}<\dots<x_{n}=b$ $\:$ i $\:$ $c=y_{0}<y_{1}<\dots<y_{m}=d$. Skup pravougaonika $\mathcal{P}=\Big\{[x_{i-1},\,x_{i}]\times[y_{j-1},\,y_{j}]\ \Big|\ i=\overline{1,n},\ j=\overline{1,m}\Big\}$ je **podela** pravougaonika $\Pi=[a,\,b]\times[c,\,d]$.
- Zadavanje podele $\mathcal{P}$ je ekvivalentno zadavanju skupa tačaka $\{(x_{i},\,y_{j})\ |\ i=\overline{1,n},\ j=\overline{1,m}\}$
- $\lambda(\mathcal{P})=\max\{x_{1}-x_{0},\,\dots,\,x_{n}-x_{n-1},\,y_{1}-y_{0},\,\dots,\,y_{m}-y_{m-1}\}$ je **parametar podele** $\mathcal{P}$
- $\mathcal{P}(\Pi)$ — skup svih podela pravougaonika $\Pi$.
___
$\xi_{ij}\in[x_{i-1},\,x_{i}]\times[y_{j-1},\,y_{j}],\quad \forall i=\overline{1,n},\ j=\overline{1,m}$. Tada su
$\xi=\left(\begin{array}{}\xi_{11}&\xi_{12}&\dots&\xi_{1m}\\\xi_{21}&\xi_{22}&\dots&\xi_{2m}\\\dots&\dots&\dots&\dots\\\xi_{n1}&\xi_{n2}&\dots&\xi_{nm}\end{array}\right)$ istaknute tačke podele $\mathcal{P}$.

**Def**. $(\mathcal{P},\,\xi)$ — **podela sa istaknutim tačkama** pravougaonika $\Pi=[a,\,b]\times[c,\,d]$


##### Površina skupa u $\mathbb{R}^{2}$
Neka je $D\in\mathbb{R}^{2}$ ograničen (tj. $\exists \Pi\in\mathbb{R}^{2}\ \ :\ \ D\subseteq\Pi$)
Neka je $\begin{align}S(D,\,\mathcal{P})=\sum\limits_{i,\,j}\delta_{ij}(x_{i}-x_{i-1})(y_{j}-y_{j-1})\end{align}$, gde je $\delta_{ij}=\begin{cases}0, &[x_{i-1},\,x_{i}]\times[y_{j-1},\,y_{j}]\cap D=\varnothing\\1,&\text{inače}\end{cases}$
Tada je **površina skupa** $D$ jednaka $\mathrm{P}(D)\in\mathbb{R}$   ako 
$\begin{align}\forall\varepsilon>0\quad\exists\delta>0\quad\forall\binom{\mathcal{P}\ \text{— podela pravougaonika }\Pi}{\text{takva da } \mathcal{P}(\lambda)<\delta}\quad \Big|\mathrm{P}(D)-S(D,\,\mathcal{P})\Big|<\varepsilon\end{align}$ ^e1916e
### Definicija i svojstva dvostrukog integrala na pravougaoniku
**Def**. Neka je $f:\ \Pi\to\mathbb{R}\ \:$ i $\ \:(\mathcal{P},\,\xi)$ podela sa istaknutim tačkama pravougaonika $\Pi$. Zbir $\begin{align}\sigma(f,\,\mathcal{P},\,\xi)=\sum\limits_{i,\,j}(x_{i}-x_{i-1})(y_{j}-y_{j-1})\,f(\xi_{ij})\end{align}$ je **integralna suma**. ^1d8e3b

$\:$
**Def**. Neka je $f:\ \Pi\to\mathbb{R}$. $\ \:$ $I\in\mathbb{R}$ je limes integralnih suma $\sigma(f,\,\mathcal{P},\,\xi)$ kad $\lambda(\mathcal{P})\to0$ ako
$\begin{align}\forall\varepsilon>0\quad\exists\delta>0\quad\forall\binom{(\mathcal{P},\,\xi )\ \text{— podela sa istaknutim tačkama}}{\text{ pravougaonika }\Pi\text{ takva da } \lambda(\mathcal{P})<\delta}\quad \Big|I-\sigma(f,\,\mathcal{P},\,\xi)\Big|<\varepsilon\end{align}$
$\:$
Tada je $\begin{align}I=\iint_{\Pi} f(x,\,y) \, dxdy \end{align}$ $\:$ **dvostruki integral** fje $f$ na $\Pi$.

Ako postoji dvostruki integral (odnosno limes), $f$ je integrabilna na $\Pi$ ($f\,\mathcal{R}\,\Pi$).
___
Napomena: [[Riman-integrabilnost funkcija i svojstva određenog integrala#Svojstva određenog integrala|svojstva određenog integrala]]

**Stav**. Ako $f:\ \Pi\to\mathbb{R}$ nije ograničena na $\Pi$ onda $\begin{align}\nexists\iint_{\Pi}f(x,\,y) \, dxdy \end{align}$

**Teorema**. $f:\ \Pi\to \mathbb{R}$ je ograničena i njen skup tačaka prekida je [[Dvostruki integral#Površina skupa u $ mathbb{R} {2}$|površine]] nula. Tada  $f\,\mathcal{R}\,\Pi$ ^8e5e56

**Teorema** (Fubinijeva na pravougaoniku). Neka je $f:\ \Pi\to\mathbb{R}$ neprekidna ($\Pi=[a,\,b]\times[c,\,d]$). Tada važi:
$\varphi_{y}(x):=f(x,\,y)$ je neprekidna na $[a,\,b]$  za fiksirano $y$
$\varphi_{x}(y):=f(x,\,y)$ je neprekidna na $[c,\,d]$ za fiksirano $x$
$\begin{align}\alpha(y):=\int_{a}^{b} f(x,\,y) \, dx\end{align}$ je neprekidna na $[c,\,d]$
$\begin{align}\beta(x):=\int_{c}^{d} f(x,\,y) \, dy\end{align}$ je neprekidna na $[a,\,b]$
i važi $\boxed{\begin{align}\iint_{\Pi}f(x,\,y)\,dxdy=\int_{a}^{b} \bigg(\int_{c}^{d}f(x,\,y)  \, dy\bigg) \, dx = \int_{c}^{d} \bigg(\int_{a}^{b}f(x,\,y)  \, dx\bigg) \, dy \end{align}}$

### Definicija i svojstva dvostrukog integrala na proizvoljnom merljivom skupu

 **Def**. Skup $D\subseteq\Pi\subseteq\mathbb{R}^{2}$ je **merljiv** ako je [[Dvostruki integral#Površina skupa u $ mathbb{R} {2}$|površina]] njegovog [[Vrste tačaka u odnosu na neki skup. Ograničenost i kompaktnost#^1ecb22|ruba]] jednaka nuli, $\mathrm{P}(\partial D)=0$.

[[Karakteristična funkcija|Karakteristična funkcija]] merljivog skupa $D$, $\chi_{D}(x,\,y)=\begin{cases}1,&(x,\,y)\in D\\0,&(x,\,y)\notin D\end{cases}$ $\ \:$ je [[Dvostruki integral#^8e5e56|integrabilna]].

**Def**. Neka je $D\subseteq\Pi\subseteq\mathbb{R}^{2}$ merljiv i $f$ je integrabilna na $\Pi$, tada je $f$ integrabilna na $D$ i važi $\boxed{\begin{align}\iint_{D} f(x,\,y) \, dxdy=\iint_{\Pi} f(x,\,y)\, \chi_{D}(x,\,y)\, dxdy \end{align}}$

> Napomena: 
> $\begin{align}\iint_{D} f(x,\,y) \, dxdy\end{align}$ možemo definisati i drugačije: kao kombinaciju [[Dvostruki integral#^e1916e|1]] i [[Dvostruki integral#^1d8e3b|2]].
> $\begin{align}\widetilde{\sigma}(f,\,\mathcal{P},\,\xi,\,D)=\sum\limits_{i,\,j}\delta_{ij}(x_{i}-x_{i-1})(y_{j}-y_{j-1})\,f(\xi_{ij})\end{align}$.
> $\begin{align}I= \iint_{D} f(x,\,y) \, dxdy\quad\Leftrightarrow\end{align}$ $\begin{align}\forall\varepsilon>0\quad\exists\delta>0\quad\forall\binom{(\mathcal{P},\,\xi )\ \text{— podela sa istaknutim tačkama}}{\text{ pravougaonika }\Pi\text{ takva da } \mathcal{P}(\lambda)<\delta}\quad \Big|I-\widetilde\sigma(f,\,\mathcal{P},\,\xi,\,D)\Big|<\varepsilon\end{align}$

^188805

$\:$
**[[Riman-integrabilnost funkcija i svojstva određenog integrala#^cfc6a3|Stav]]**.  $f,\,g\,\mathcal{R}\,D$; $\ \ \alpha,\,\beta\in\mathbb{R}$. Tada $(\alpha\,f+\beta\,g)\,\mathcal{R}\,D$ i važi
$\begin{align}\iint_{D}(\alpha\,f+\beta\,g)(x,\,y) \, dxdy = \alpha\iint_{D} f(x,\,y) \, dxdy+\beta \iint_{D} g(x,\,y) \, dxdy \end{align}$

**Stav**.  $f,\,g\,\mathcal{R}\,D$; $\ \ \forall (x,\,y)\in D\quad f(x)\leqslant g(x)$. Tada $\begin{align}\iint_{D} f(x,\,y) \, dxdy\leqslant \iint_{D} g(x,\,y) \, dxdy \end{align}$

**Stav**. $f\,\mathcal{R}\,\Pi$, $\ \:$ $D,\,E\subseteq\Pi$, $\ \:$ $D\cap E=\varnothing$. $\ \:$ Tada
$\begin{align}\iint_{D\cup E} f(x,\,y) \, dxdy = \iint_{D} f(x,\,y) \, dxdy + \iint_{E} f(x,\,y) \, dxdy\end{align}$
> Dokaz:
> $\left.\begin{array}{l}\chi_{D\cup E}=\chi_{D}+\chi_{E}+\chi_{D}\chi_{E}\\D\cap E =\varnothing\quad\Rightarrow\quad\chi_{D}\chi_{E}=0\end{array}\ \ \right|\Rightarrow\quad\chi_{D\cup E}=\chi_{D}+\chi_{E}$

**Stav**.
- $\begin{align}\iint_{D} 1 \, dxdy = \mathrm{P}(D) \end{align}$
- $\begin{align}\mathrm{P}(D)=0\quad\Rightarrow\quad \iint_{D} f(x,\,y) \, dxdy = 0 \end{align}$

**[[Riman-integrabilnost funkcija i svojstva određenog integrala#Predstavljanje određenog integrala proizvodom|Stav]]**. 
- $f\,\mathcal{R}\,D$, $\ \:$ $m=\min\limits_{D} f$, $\ \:$ $M=\max\limits_{D}f$. $\ \:$ Tada $\begin{align}\exists \mu\in[m,\,M]\quad \iint_{D} f(x,\,y) \, dxdy = \mu\cdot\mathrm{P}(D) \end{align}$
- $f\,\mathcal{C}\,D$.$\ \:$ Tada $\begin{align}\exists (x_{0},\,y_{0})\in D\quad \iint_{D} f(x,\,y) \, dxdy = f(x_{0},\,y_{0})\cdot\mathrm{P}(D) \end{align}$

**Teorema** (Fubinijeva na oblasti). Neka je $f:\ \Pi\to\mathbb{R}$ neprekidna i
- neka je $D=\Big\{(x,\,y)\in\mathbb{R}^{2}\ \Big| \ a\leqslant x\leqslant b,\ \alpha(x)\leqslant y\leqslant \beta(x)\Big\}\subseteq \Pi$. Tada važi
$\boxed{\begin{align}\iint_{D}f(x,\,y)\,dxdy=\int_{a}^{b} \bigg(\int_{\alpha(x)}^{\beta(x)}f(x,\,y)  \, dy\bigg) \, dx \end{align}}$
- neka je $D=\Big\{(x,\,y)\in\mathbb{R}^{2}\ \Big| \ c\leqslant y\leqslant d,\ \gamma(y)\leqslant x\leqslant \delta(y)\Big\}\subseteq \Pi$. Tada važi
$\boxed{\begin{align}\iint_{D}f(x,\,y)\,dxdy=\int_{c}^{d} \bigg(\int_{\gamma(y)}^{\delta(y)}f(x,\,y)  \, dx\bigg) \, dy \end{align}}$

> Dokaz: pokažemo prvo tvrđene, drugo je analogno.
> $\Pi=[a,\,b]\times[c,\,d]$, gde je $c\leqslant\alpha(x)\leqslant\beta(x)\leqslant d,\quad\forall x\in[a,\,b]$.
> 
> $\begin{align}\iint_{D}f(x,\,y)\,dxdy=\iint_{\Pi}\chi_{D}(x,\,y)f(x,\,y)\,dxdy=\int_{a}^{b} \bigg(\int_{c}^{d} \chi_{D}(x,\,y) f(x,\,y) \, dy\bigg) \, dx\end{align}$
> Jer $\chi_{D}(x,\,y)=0$ za $c\leqslant y\leqslant\alpha(x)$ i za $\beta(x)\leqslant y\leqslant d$ (pri fiksiranom $x$) važi $\begin{align}\int_{c}^{d} \chi_{D}(x,\,y) f(x,\,y) \, dy=\int_{\alpha(x)}^{\beta(x)} f(x,\,y) \, dx\end{align}$


$\:$
### Smena promenljivih
**Teorema** (opšta smena). Neka smena $F$ slika merljiv skup $D$ u merljiv skup $F[D]$, $F$ ima sve parcijalne izvode na $\overline{D}$, $F^{-1}$ ima sve parcijalne izvode na $\overline{F[D]}$ i $f\,\mathcal{C}\,F[D]$. Tada
$\begin{align}\iint_{F[D]} f(x,\,y) \, dxdy = \iint_{D} (f\circ F)(u,\,v)\,|J_{F}(u,\,v)| \, dudv\end{align}$

$\:$
**Teorema** (polarna smena). Neka polarna smena $F:\ (r,\,\theta)\mapsto(r\cos \theta,\, r \sin \theta), \quad r\geqslant0,\ 0\leqslant\theta<2\pi$
slika merljiv skup $D$ u merljiv skup $F[D]$, $f\,\mathcal{C}\,F[D]$. Tada
$\begin{align}\iint_{F[D]} f(x,\,y) \, dxdy = \iint_{D} f(r\cos \theta,\,r\sin \theta)\,r \, drd\theta\end{align}$
> Dokaz:
> >Definišemo podelu merljivog skupa $D$ na manje merljive skupove koji se seku po svojim granicama. $\mathcal{P}=\Big\{D_{i}\subseteq D\ \Big|\ i=\overline{1,n};\quad \forall i\ne j\quad D_{i}\cap D_{j}\subseteq\partial(D_{i}\cap D_{j})\Big\}$
> Parametar takve podele: $\lambda(\mathcal{P})=\max\limits_{i=\overline{1,n}}\Big(\sup\limits_{x,\,y\in D_{i}}||x-y||\Big)$
> 
> Neka je $\mathrm{S}=\Big\{(r,\,\theta)\ \Big|\ \tilde{r}\leqslant r\leqslant \tilde{\tilde{r}},\ \ \tilde{\theta}\leqslant\theta\leqslant\tilde{\tilde{\theta}}\Big\}\supseteq D$, presek isečka i kružnog prstena u koji upada $D$.
> $\mathcal{P}=\Big\{\mathrm{S}_{ij}\ \Big|\ i=\overline{1,n},\ j=\overline{1,m}\Big\}$ — podela $\mathrm{S}$, pri čemu 
> $\mathrm{S}_{ij}=\Big\{(r,\,\theta)\ \Big|\ r_{i}\leqslant r\leqslant r_{i+1},\ \ \theta_{j}\leqslant\theta\leqslant\theta_{j+1}\Big\}$
> Površina $\mathrm{S}_{ij}$ je jednaka $\begin{align}\frac{r_{i+1}^{2}(\theta_{j+1}-\theta_{j})}{2}-\frac{r_{i}^{2}(\theta_{j+1}-\theta_{j})}{2}=\bigg(r_{i}-\frac{\Delta r_{i}}{2}\bigg)\Delta r_{i}\Delta\theta_{j}\end{align}$
> uz oznake $\Delta r_{i}=r_{i+1}-r_{i}$ $\ \:$ i $\ \:$ $\Delta \theta_{j}=\theta_{j+1}-\theta_{j}$
> 
> Biramo istaknute tačke: $\begin{align}\xi_{ij}=\bigg(r_{i}+\frac{\Delta r_{i}}{2},\ \hat{\theta}_{j}\bigg),\quad \theta_{j}<\hat{\theta}_{j}<\theta_{j+1}\end{align}$
> 
> $\delta_{ij}=\begin{cases}0, &\mathrm{S}_{ij}\cap D=\varnothing\\1,&\text{inače}\end{cases}$
> 
> $\begin{align}\widetilde\sigma(f,\,\mathcal{P},\,\xi,\,D)=\sum\limits_{i,\ j} f\bigg(r_{i}+\frac{\Delta r_{i}}{2},\ \hat{\theta}_{j}\bigg)\cdot\bigg(r_{i}-\frac{\Delta r_{i}}{2}\bigg)\Delta r_{i}\Delta\theta_{j}\cdot\delta_{ij}\end{align}$
> 
> $\begin{align}f\bigg(r_{i}+\frac{\Delta r_{i}}{2},\ \hat{\theta}_{j}\bigg)\cdot\bigg(r_{i}-\frac{\Delta r_{i}}{2}\bigg)\to f(r_{i},\,\hat{\theta}_{j})\cdot r_{i},\quad \text{ kad }\ \lambda(\mathcal{P})\to 0\end{align}$
> 
> Iz [[Dvostruki integral#^188805|napomene]] je jasno da $\begin{align}I=\iint_{D} f(r\sin \theta,\,r\cos \theta)\, r\, drd\theta \end{align}$
> 
> Sa druge strane u normalnim koordinatama imamo $\begin{align}I=\iint_{F[D]} f(x,\,y) \, dxdy \end{align}$
^10b6ee

