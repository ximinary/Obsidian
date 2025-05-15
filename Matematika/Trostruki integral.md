#fax #math #a3 [deo [[Analiza|analize]]]

### Podela kvadra
**Def**. Neka su $a=x_{0}<x_{1}<\dots<x_{n}=b$, $\:$ $c=y_{0}<y_{1}<\dots<y_{m}=d$ $\:$ i $\:$ $g=z_{0}<z_{1}<\dots<z_{l}=h$. Skup kvadara $\mathcal{P}=\Big\{[x_{i-1},\,x_{i}]\times[y_{j-1},\,y_{j}]\times[z_{k-1},\,z_{k}]\ \Big|\ i=\overline{1,n},\ j=\overline{1,m},\ k=\overline{1,l}\Big\}$ je **podela** kvadra $K=[a,\,b]\times[c,\,d]\times[g,\,h]$.
- Zadavanje podele $\mathcal{P}$ je ekvivalentno zadavanju skupa tačaka $\{(x_{i},\,y_{j},\,z_{k})\ |\ i=\overline{1,n},\ j=\overline{1,m},\ k=\overline{1,l}\}$
- $\lambda(\mathcal{P})=\max\{x_{1}-x_{0},\,\dots,\,x_{n}-x_{n-1},\,y_{1}-y_{0},\,\dots,\,y_{n}-y_{n-1},\,z_{1}-z_{0},\,\dots,\,z_{l}-z_{l-1}\}$ je **parametar podele** $\mathcal{P}$
- $\mathcal{P}(K)$ — skup svih podela kvadra $K$.
___
$\xi_{ij}\in[x_{i-1},\,x_{i}]\times[y_{j-1},\,y_{j}]\times[z_{k-1},\,z_{k}],\quad \forall i=\overline{1,n},\ j=\overline{1,m},\ k=\overline{1,l}$. Tada su
$\xi=(\xi_{ijk})$ istaknute tačke podele $\mathcal{P}$.

**Def**. $(\mathcal{P},\,\xi)$ — **podela sa istaknutim tačkama** pravougaonika $\Pi=[a,\,b]\times[c,\,d]\times[g,\,h]$


##### Zapremina skupa u $\mathbb{R}^{3}$
Neka je $D\in\mathbb{R}^{3}$ ograničen (tj. $\exists K\in\mathbb{R}^{3}\ \ :\ \ D\subseteq K$)
Neka je $\begin{align}S(D,\,\mathcal{P})=\sum\limits_{i,\,j,\,k}\delta_{ijk}(x_{i}-x_{i-1})(y_{j}-y_{j-1})(z_{k}-z_{k-1})\end{align}$, gde je $\delta_{ijk}=\begin{cases}0, &[x_{i-1},\,x_{i}]\times[y_{j-1},\,y_{j}]\times[z_{k-1},\,z_{k}]\cap D=\varnothing\\1,&\text{inače}\end{cases}$
Tada je **zapremina skupa** $D$ jednaka $\mathrm{V}(D)\in\mathbb{R}$   ako 
$\begin{align}\forall\varepsilon>0\quad\exists\delta>0\quad\forall\binom{\mathcal{P}\ \text{— podela kvadra }K}{\text{takva da } \mathcal{P}(\lambda)<\delta}\quad \Big|\mathrm{V}(D)-S(D,\,\mathcal{P})\Big|<\varepsilon\end{align}$ ^e1916e
### Definicija i svojstva trostrukog integrala na kvadru
**Def**. Neka je $f:\ K\to\mathbb{R}\ \:$ i $\ \:(\mathcal{P},\,\xi)$ podela sa istaknutim tačkama kvadra $K$. Zbir $\begin{align}\sigma(f,\,\mathcal{P},\,\xi)=\sum\limits_{i,\,j,\,k}(x_{i}-x_{i-1})(y_{j}-y_{j-1})(z_{k}-z_{k-1})\,f(\xi_{ijk})\end{align}$ je **integralna suma**. ^1d8e3b

$\:$
**Def**. Neka je $f:\ K\to\mathbb{R}$. $\ \:$ $I\in\mathbb{R}$ je limes integralnih suma $\sigma(f,\,\mathcal{P},\,\xi)$ kad $\lambda(\mathcal{P})\to0$ ako
$\begin{align}\forall\varepsilon>0\quad\exists\delta>0\quad\forall\binom{(\mathcal{P},\,\xi )\ \text{— podela sa istaknutim tačkama}}{\text{ kvadra }K\text{ takva da } \lambda(\mathcal{P})<\delta}\quad \Big|I-\sigma(f,\,\mathcal{P},\,\xi)\Big|<\varepsilon\end{align}$
$\:$
Tada je $\begin{align}I=\iiint_{K} f(x,\,y,\,z) \, dxdydz \end{align}$ $\:$ **trostruki integral** fje $f$ na $K$.

Ako postoji trostruki integral (odnosno limes), $f$ je integrabilna na $K$ ($f\,\mathcal{R}\,K$).
___
Napomena: [[Riman-integrabilnost funkcija i svojstva određenog integrala#Svojstva određenog integrala|svojstva određenog integrala]]

**Stav**. Ako $f:\ K\to\mathbb{R}$ nije ograničena na $K$ onda $\begin{align}\nexists\iiint_{K}f(x,\,y,\,z) \, dxdydz \end{align}$

**Teorema**. $f:\ K\to \mathbb{R}$ je ograničena i njen skup tačaka prekida je [[Trostruki integral#Zapremina skupa u $ mathbb{R} {3}$|zapremine]] nula. Tada  $f\,\mathcal{R}\,K$ ^8e5e56

**Teorema** (Fubinijeva na kvadru). Neka je $f:\ K\to\mathbb{R}$ neprekidna ($K=[a,\,b]\times[c,\,d]\times[g,\,h]$). Tada važi $\boxed{\begin{align}\iiint_{K}f(x,\,y,\,z)\,dxdydz=\int_{a}^{b} \bigg(\int_{c}^{d}\bigg(\int_{g}^{h} f(x,\,y)\, dz\bigg) \, dy\bigg) \, dx =\cdots \end{align}}$
(u bilo kom redosledu integriranja)

### Definicija i svojstva trostrukog integrala na proizvoljnom merljivom skupu

 **Def**. Skup $D\subseteq K\subseteq\mathbb{R}^{3}$ je **merljiv** ako je [[Trostruki integral#Zapremina skupa u $ mathbb{R} {3}$|zapremina]] njegovog [[Vrste tačaka u odnosu na neki skup. Ograničenost i kompaktnost#^1ecb22|ruba]] jednaka nuli, $\mathrm{V}(\partial D)=0$.

[[Karakteristična funkcija|Karakteristična funkcija]] merljivog skupa $D$, $\chi_{D}(x,\,y,\,z)=\begin{cases}1,&(x,\,y,\,z)\in D\\0,&(x,\,y,\,z)\notin D\end{cases}$ $\ \:$ je [[Dvostruki integral#^8e5e56|integrabilna]].

**Def**. Neka je $D\subseteq K\subseteq\mathbb{R}^{3}$ merljiv i $f$ je integrabilna na $K$, tada je $f$ integrabilna na $D$ i važi $\boxed{\begin{align}\iiint_{D} f(x,\,y,\,z) \, dxdydz=\iiint_{K} f(x,\,y,\,z)\, \chi_{D}(x,\,y,\,z)\, dxdydz \end{align}}$


$\:$
**[[Riman-integrabilnost funkcija i svojstva određenog integrala#^cfc6a3|Stav]]**.  $f,\,g\,\mathcal{R}\,D$; $\ \ \alpha,\,\beta\in\mathbb{R}$. Tada $(\alpha\,f+\beta\,g)\,\mathcal{R}\,D$ i važi
$\begin{align}\iiint_{D}(\alpha\,f+\beta\,g)(x,\,y,\,z) \, dxdydz = \alpha\iiint_{D} f(x,\,y,\,z) \, dxdydz+\beta \iiint_{D} g(x,\,y,\,z) \, dxdydz \end{align}$

**Stav**.  $f,\,g\,\mathcal{R}\,D$; $\ \ \forall (x,\,y,\,z)\in D\quad f(x)\leqslant g(x)$. Tada $\begin{align}\iiint_{D} f(x,\,y,\,z) \, dxdydz\leqslant \iiint_{D} g(x,\,y,\,z) \, dxdydz \end{align}$

**Stav**. $f\,\mathcal{R}\,K$, $\ \:$ $D,\,E\subseteq K$, $\ \:$ $D\cap E=\varnothing$. $\ \:$ Tada
$\begin{align}\iiint_{D\cup E} f(x,\,y,\,z) \, dxdydz = \iiint_{D} f(x,\,y,\,z) \, dxdydz + \iiint_{E} f(x,\,y,\,z) \, dxdydz\end{align}$


**Stav**.
- $\begin{align}\iiint_{D} 1 \, dxdydz = \mathrm{V}(D) \end{align}$
- $\begin{align}\mathrm{V}(D)=0\quad\Rightarrow\quad \iiint_{D} f(x,\,y,\,z) \, dxdydz = 0 \end{align}$

**[[Riman-integrabilnost funkcija i svojstva određenog integrala#Predstavljanje određenog integrala proizvodom|Stav]]**. 
- $f\,\mathcal{R}\,D$, $\ \:$ $m=\min\limits_{D} f$, $\ \:$ $M=\max\limits_{D}f$. $\ \:$ Tada $\begin{align}\exists \mu\in[m,\,M]\quad \iiint_{D} f(x,\,y,\,z) \, dxdydz = \mu\cdot\mathrm{P}(D) \end{align}$
- $f\,\mathcal{C}\,D$.$\ \:$ Tada $\begin{align}\exists (x_{0},\,y_{0},\,z_{0})\in D\quad \iiint_{D} f(x,\,y,\,z) \, dxdydz = f(x_{0},\,y_{0},\,z_{0})\cdot\mathrm{P}(D) \end{align}$

**Teorema** (Fubinijeva na oblasti). Neka je $f:\ K\to\mathbb{R}$ neprekidna i neka je $D=\Big\{(x,\,y,\,z)\in\mathbb{R}^{2}\ \Big| \ a\leqslant x\leqslant b,\ \alpha(x)\leqslant y\leqslant \beta(x),\ \varphi(x,\,y)\leqslant z\leqslant\psi(x,\,y)\Big\}\subseteq K$. Tada važi
$\boxed{\begin{align}\iiint_{D}f(x,\,y,\,z)\,dxdydz=\int_{a}^{b} \bigg(\int_{\alpha(x)}^{\beta(x)} \bigg(\int_{\varphi(x,\,y)}^{\psi(x,\,y)} f(x,\,y,\,z) \, dz\bigg) \, dy\bigg) \, dx \end{align}}$
(analogno važi i za druge oblasti sa drugačijem redosledom zavisnosti $x$, $y$, $z$)

### Smena promenljivih
**Teorema** (opšta smena). Neka smena $F$ slika merljiv skup $D$ u merljiv skup $F[D]$, $F$ ima sve parcijalne izvode na $\overline{D}$, $F^{-1}$ ima sve parcijalne izvode na $\overline{F[D]}$ i $f\,\mathcal{C}\,F[D]$. Tada
$\begin{align}\iiint_{F[D]} f(x,\,y,\,z) \, dxdydz = \iiint_{D} (f\circ F)(u,\,v,\,w)\,|J_{F}(u,\,v,\,w)| \, dudvdw\end{align}$

$\:$
**Teorema** (cilindrička smena). Neka cilindrička smena $F:\ (r,\,\theta,\,z)\mapsto (r\cos \theta,\,r\sin \theta,\,z), \quad r\geqslant0,\ 0\leqslant\theta<2\pi$
slika merljiv skup $D$ u merljiv skup $F[D]$, $f\,\mathcal{C}\,F[D]$. Tada
$\begin{align}\iiint_{F[D]} f(x,\,y,\,z) \, dxdydz = \iiint_{D} f(r\cos \theta,\,r\sin \theta,\,z)\,r \, drd\theta dz\end{align}$
> Dokaz: sledi iz [[Dvostruki integral#^10b6ee|polarne smene]] u $\mathbb{R}^{2}$

$\:$
**Teorema** (sferna smena). Neka sferna smena $F:\ (r,\,\theta,\,\varphi)\mapsto (r\cos \theta\sin\varphi,\,r\sin \theta\sin\varphi,\,r\cos\varphi), \quad r\geqslant0,\ 0\leqslant\theta<2\pi,\,-\frac{\pi}{2}\leqslant\varphi\leqslant\frac{\pi}{2}$
slika merljiv skup $D$ u merljiv skup $F[D]$, $f\,\mathcal{C}\,F[D]$. Tada
$\begin{align}\iiint_{F[D]} f(x,\,y,\,z) \, dxdydz = \iiint_{D} f(r\cos \theta\sin\varphi,\,r\sin \theta\sin\varphi,\,r\cos\varphi)\,r^{2}\sin\varphi \, drd\theta d\varphi\end{align}$
> Dokaz:
> >Definišemo podelu merljivog skupa $D$ na manje merljive skupove koji se seku po svojim granicama. $\mathcal{P}=\Big\{D_{i}\subseteq D\ \Big|\ i=\overline{1,n};\quad \forall i\ne j\quad D_{i}\cap D_{j}\subseteq\partial(D_{i}\cap D_{j})\Big\}$
> Parametar takve podele: $\lambda(\mathcal{P})=\max\limits_{i=\overline{1,n}}\Big(\sup\limits_{x,\,y\in D_{i}}||x-y||\Big)$
> 
> Neka je $\mathrm{S}=\Big\{(r,\,\theta,\,\varphi)\ \Big|\ \tilde{r}\leqslant r\leqslant \tilde{\tilde{r}},\ \ \tilde{\theta}\leqslant\theta\leqslant\tilde{\tilde{\theta}},\ \ \tilde{\varphi}\leqslant\varphi\leqslant\tilde{\tilde{\varphi}}\Big\}\supseteq D$
> $\mathcal{P}=\Big\{\mathrm{S}_{ijk}\ \Big|\ i=\overline{1,n},\ j=\overline{1,m},\ k =\overline{1,l}\Big\}$ — podela $\mathrm{S}$, pri čemu 
> $\mathrm{S}_{ijk}=\Big\{(r,\,\theta)\ \Big|\ r_{i}\leqslant r\leqslant r_{i+1},\ \ \theta_{j}\leqslant\theta\leqslant\theta_{j+1},\ \ \varphi_{k}\leqslant\varphi\leqslant\varphi_{k+1}\Big\}$
> Zapremina $\mathrm{S}_{ijk}$ je jednaka $\begin{align}\frac{(r_{i+1}^{3}-r_{i}^{3})(\theta_{j+1}-\theta_{j})(\cos\varphi_{k}-\cos\varphi_{k+1})}{3}=\frac{1}{3}3\hat{r}_{i}^{2}\Delta r_{i}\Delta\theta_{j}(-\sin \hat{\varphi}_{k})(-\Delta\varphi_{k})=\hat{r}_{i}^{2}\sin \hat{\varphi}_{k}\Delta r_{i}\Delta\theta_{j}\Delta\varphi_{k}\end{align}$
> uz primenu [[Teoreme o srednjoj vrednosti#^e52da5|Lagranževe teoreme]] na fje $x^{3}$ ($\exists \hat{r}_{i}\in(r_{i},\,r_{i+1})$) i $\cos x$ ($\exists\hat{\varphi}_{k}\in(\varphi_{k},\,\varphi_{k+1})$) i uz oznake $\Delta r_{i}=r_{i+1}-r_{i}$, $\ \:$ $\Delta \theta_{j}=\theta_{j+1}-\theta_{j}$, $\ \:$ $\Delta \varphi_{k}=\varphi_{k+1}-\varphi_{k}$
> 
> Biramo istaknute tačke: $\begin{align}\xi_{ijk}=(\hat{r}_{i},\ \hat{\theta}_{j},\,\hat{\varphi}_{k}),\quad \theta_{j}<\hat{\theta}_{j}<\theta_{j+1}\end{align}$
> 
> $\delta_{ijk}=\begin{cases}0, &\mathrm{S}_{ijk}\cap D=\varnothing\\1,&\text{inače}\end{cases}$
> 
> $\begin{align}\widetilde\sigma(f,\,\mathcal{P},\,\xi,\,D)=\sum\limits_{i,\ j} f(\hat{r}_{i},\ \hat{\theta}_{j},\,\hat{\varphi}_{k})\cdot\hat{r}_{i}^{2}\sin \hat{\varphi}_{k}\Delta r_{i}\Delta\theta_{j}\Delta\varphi_{k}\cdot\delta_{ijk}\end{align}$
> 
> Imamo, $\begin{align}I=\iiint_{D} f(r\sin \theta\sin\varphi,\,r\cos \theta\sin\varphi,\,r\cos\varphi)\, r^{2}\sin\varphi\, drd\theta d\varphi \end{align}$
> 
> Sa druge strane u normalnim koordinatama imamo $\begin{align}I=\iiint_{F[D]} f(x,\,y,\,z) \, dxdydz \end{align}$