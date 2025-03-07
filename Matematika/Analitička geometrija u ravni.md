#fax #math #geom  [deo [[Geometrija|geometrije]]]


### Prava
- Eksplicitna jednačina
  $p: \ y=kx+n$
  vertikalne prave se ne mogu zapisati
$\:$
- Implicitna jednačina
  $p:\ ax+by+c=0$ $\quad$ — nije jedinstvena (moguće pomnožiti sa $\lambda\in\mathbb{R}$)
  $n_{p}=(a,\,b)$ je normalni vektor na pravu $p$
  
  normalizovana je ako je normalni vektor jedinični:
  $\begin{align}p:\ \frac{a}{\sqrt[]{a^{2}+b^{2}}}\,x+\frac{b}{\sqrt[]{a^{2}+b^{2}}}\,y+\frac{c}{\sqrt[]{a^{2}+b^{2}}}=0\end{align}$ $\quad$ — jedinstvena do na znak, tj. na smer vektora normale.
$\:$
- Normalna jednačina
  $p:\ x\cos\varphi+x\sin\varphi=\rho,\quad \varphi\in[0,\,2\pi),\quad\rho\geqslant0$
  $\cos \varphi=\frac{a}{\sqrt[]{a^{2}+b^{2}}},\quad \sin\varphi=\frac{b}{\sqrt[]{a^{2}+b^{2}}},\quad\rho=-\frac{c}{\sqrt[]{a^{2}+b^{2}}}\geqslant0$
  Uslov $\rho\geqslant0$ daje jedinstvenost.
$\:$
- $\forall \mathrm{M}\in p\quad\boxed{\overrightarrow{\rm PM}\circ \overrightarrow{n_{p}}=0}$, gde je $\ \:\mathrm{P}(x_{0},\,y_{0})\in p$, $\ \:\overrightarrow{n_{p}}\:$ normalni vektor.
  $(x-x_{0},\,y-y_{0})\circ(a,\,b)=0$
  $a(x-x_{0})+b(y-y_{0})=0$
  $ax+by\underbrace{-ax_{0}-by_{0}}_{=\,c}=0$
  $\:$

- Parametarska jednačina
  $\mathrm{P}(x_{0},\,y_{0})\in p$, $\ \:\overrightarrow{p}=(p_{x},\,p_{y})\:$ vektor pravca prave $p$.
  > $\overrightarrow{p}\perp \overrightarrow{n_{p}}\quad\Leftrightarrow\quad \overrightarrow{p}\circ \overrightarrow{n_{p}}=0\quad \Leftrightarrow\quad\overrightarrow{p}=(-b,\,a)$
  
  $p:\ \mathrm{M}(t)=\mathrm{P}+t\,\overrightarrow{p},\quad t\in\mathbb{R}$
  $\:$
  $p:\ \begin{cases}x=x_{0}+t\,p_{x}\\y = y_{0}+t\,p_{y}\end{cases}\quad t\in\mathbb{R}$
  $\:$
- Kanonska jednačina
$\begin{align}\frac{x-x_{0}}{p_{x}}=\frac{y-y_{0}}{p_{y}} = t\end{align}$


___
Neka je $f(x,\,y)=0$ implicitna jednačina prave $p$. Tada
$C$ i $D$ su sa iste stane od $p$ $\quad\Leftrightarrow\quad \mathrm{sgn}\,f(C)=\mathrm{sgn}f(D)$

### Parametarska jednačina paralelograma
Svaka tačka unutra paralelograma ${\rm ABCD}$ može biti predstavljena u obliku:
$\mathrm{X}(t_{1},\,t_{2})=\mathrm{A}+t_{1}\overrightarrow{\rm AB}+t_{2}\overrightarrow{\rm AD},\quad 0\leqslant t_{1},\,t_{2}\leqslant1$
### Parametarska jednačina trougla
Svaka tačka unutra trougla ${\rm ABC}$ može biti predstavljena u obliku:
$\mathrm{X}(t_{1},\,t_{2})=\mathrm{A}+t_{1}\overrightarrow{\rm AB}+t_{2}\overrightarrow{\rm AB},\quad 0\leqslant t_{1},\,t_{2}\leqslant1,\quad t_{1}+t_{2}\leqslant1$

### Rastojanje tačke od prave

**Stav**. Rastojanje tačke $\mathrm{M}(x_{0},\,y_{0})$ od prave $p:\ ax+by+c=0$ je $\begin{align}\mathrm{d}(\mathrm{M},\,p)=\frac{|ax_{0}+by_{0}+c|}{\sqrt[]{a^{2}+b^{2}}}\end{align}$
> Dokaz: tačka $\mathrm{P}\in p$ je takva da $|| \overrightarrow{\rm PM}||=\mathrm{d}(\mathrm{M},\,p)$,
> tada iz $\overrightarrow{\rm PM}\circ \overrightarrow{n_{p}}=|| \overrightarrow{\rm PM}||\cdot|| \overrightarrow{n_{p}}||\,\underbrace{\cos \widehat{(\overrightarrow{\rm PM},\,\overrightarrow{n_{p}})}}_{=\,\pm 1}$ dobijamo:
> 
 $\begin{align}\mathrm{d}(\mathrm{M},\,p)=||\overrightarrow{\rm PM}||=\frac{\Big|\overrightarrow{\rm PM}\circ \overrightarrow{n_{p}}\Big|}{|| \overrightarrow{n_{p}}||}=\frac{\Big|\big(\overrightarrow{\rm OM}-\overrightarrow{\rm OP}\big)\circ \overrightarrow{n_{p}}\Big|}{|| \overrightarrow{n_{p}}||}=\end{align}$
 $\begin{align}=\frac{\Big|\overbrace{\overrightarrow{\rm OM}\circ \overrightarrow{n_{p}}}^{=\,ax_{0}\,+\,by_{0}}\ \overbrace{-\ \overrightarrow{\rm OP}\circ \overrightarrow{n_{p}}}^{=\,c}\Big|}{|| \overrightarrow{n_{p}}||}=\frac{|ax_{0}+by_{0}+c|}{\sqrt[]{a^{2}+b^{2}}}\end{align}$

^02dde3

$\:$
**[[Analitička geometrija u prostoru#^f9c9c9|Stav]]**. Rastojanje tačke $\mathrm{M}$ od prave $p:\ P,\,\overrightarrow{\rm p}$ $\ \:$ je
$\begin{align}\mathrm{d}(\mathrm{M},\,p)=\frac{|| \overrightarrow{\rm MP}\times\overrightarrow{p}\,||}{||\, \overrightarrow{p}\,||}\end{align}$ 

### Uzajamni položaj pravih
$p:\ a_{1}x+b_{1}y+c_{1}=0$
$q:\ a_{2}x+b_{2}y+c_{2}=0$

[[Sistem linearnih jednačina#^ec3686|Kramerovo pravilo]]:
$\begin{cases}a_{1}x+b_{1}y=-c_{1}\\a_{2}x+b_{2}y=-c_{2}\end{cases}$
$\Delta=\left|\begin{array}{}a_{1}&b_{1}\\a_{2}&b_{2}\end{array}\right|\quad\quad\Delta_{x}=-\left|\begin{array}{}c_{1}&b_{1}\\c_{2}&b_{2}\end{array}\right|\quad\quad\Delta_{y}=-\left|\begin{array}{}a_{1}&c_{1}\\a_{2}&c_{2}\end{array}\right|$

- Poklapaju se:
  $\begin{align}p \equiv q\quad&\Leftrightarrow\quad\begin{cases} \overrightarrow{n_{p}}=\lambda \overrightarrow{n_{q}},\ \lambda\in\mathbb{R}\\\mathrm{P}\in p\quad\Rightarrow\quad\mathrm{P}\in q\end{cases}\\\\& \Leftrightarrow\quad\Delta=0,\ \ \Delta_{x}=0,\ \ \Delta_{y}=0\end{align}$
  $\:$
- Paralelne:
  $\begin{align}p \parallel q\quad&\Leftrightarrow\quad\begin{cases} \overrightarrow{n_{p}}=\lambda \overrightarrow{n_{q}},\ \lambda\in\mathbb{R}\\\mathrm{P}\in p\quad\Rightarrow\quad\mathrm{P}\notin q\end{cases}\\\\& \Leftrightarrow\quad\Delta=0,\ \ \Delta_{x}\ne0,\ \ \Delta_{y}\ne0\end{align}$ 
  $\:$
- Seku se:
  $\begin{align}p\text{ i }q \text{ se seku}\quad&\Leftrightarrow\quad\exists \mathrm{M}(x_{0},\,y_{0})\ \ : \ \ \mathrm{M}\in p\ \text{ i }\  \mathrm{M}\in q\\& \quad\quad\ \ \, x_{0}=\frac{\Delta_{x}}{\Delta},\quad y_{0}=\frac{\Delta_{y}}{\Delta}\\\\& \Leftrightarrow\quad\Delta\ne0\end{align}$

> Tražimo presek pravih datih parametarski:
> $p:\ \mathrm{M}(t)=\mathrm{P}+t\,\overrightarrow{p},\quad t\in \mathbb{R}$
> $q:\ \mathrm{M}(s)=\mathrm{Q}+s\,\overrightarrow{q},\quad s\in \mathbb{R}$
> 
> $\mathrm{P}+t\,\overrightarrow{p}=\mathrm{M}=\mathrm{Q}+s\,\overrightarrow{q}$
> $t\,\overrightarrow{p}-s\,\overrightarrow{q}=\mathrm{Q}-\mathrm{P}$
> $t\,\overrightarrow{p}-s\,\overrightarrow{q}=\overrightarrow{\rm PQ}$
> > vektorski množimo sa $\overrightarrow{p}$ :
> > $(-s\,\overrightarrow{q}\,)\times \overrightarrow{p}=\overrightarrow{\rm PQ}\times \overrightarrow{p}$
> > $s(\,\overrightarrow{p}\,\times \overrightarrow{q}\,)=\overrightarrow{\rm PQ}\times \overrightarrow{p}$
> > $\begin{align}s=\frac{\overrightarrow{\rm PQ}\times \overrightarrow{p}}{\overrightarrow{p}\,\times \overrightarrow{q}}\end{align}$
> > $\begin{align}\boxed{s=\frac{D\Big(\overrightarrow{\rm PQ},\ \overrightarrow{p}\,\Big)}{D\Big(\overrightarrow{p},\  \overrightarrow{q}\,\Big)}}\end{align}$
>
>$\:$
> > vektorski množimo sa $\overrightarrow{q}$ :
> > $(t\,\overrightarrow{p}\,)\times \overrightarrow{q}=\overrightarrow{\rm PQ}\times \overrightarrow{q}$
> > $t(\,\overrightarrow{p}\,\times \overrightarrow{q}\,)=\overrightarrow{\rm PQ}\times \overrightarrow{q}$
> > $\begin{align}t=\frac{\overrightarrow{\rm PQ}\times \overrightarrow{q}}{\overrightarrow{p}\,\times \overrightarrow{q}}\end{align}$
> > $\begin{align}\boxed{t=\frac{D\Big(\overrightarrow{\rm PQ},\ \overrightarrow{q}\,\Big)}{D\Big(\overrightarrow{p},\  \overrightarrow{q}\,\Big)}}\end{align}$
> 
> Tražimo $s$ ili $t$ i zatim nalazimo $\mathrm{M}$.
 