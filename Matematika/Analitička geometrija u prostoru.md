#fax #math #geom  [deo [[Geometrija|geometrije]]]

### Ravan
- Implicitna jednačina
  $\alpha:\ ax+by+cz+d=0$ $\quad$ — nije jedinstvena (moguće pomnožiti sa $\lambda\in\mathbb{R}$)
  $n_{\alpha}=(a,\,b,\,c)$ je normalni vektor na ravan $\alpha$
  
  normalizovana je ako je normalni vektor jedinični:
  $\begin{align}\alpha:\ \frac{a}{\sqrt[]{a^{2}+b^{2}+c^{2}}}\,x+\frac{b}{\sqrt[]{a^{2}+b^{2}+c^{2}}}\,y+\frac{c}{\sqrt[]{a^{2}+b^{2}+c^{2}}}z+\frac{d}{\sqrt[]{a^{2}+b^{2}+c^{2}}}=0\end{align}$ $\quad$ — jedinstvena do na znak, tj. na smer vektora normale.
  $\:$
- $\forall \mathrm{M}\in \alpha\quad\boxed{\overrightarrow{\rm PM}\circ \overrightarrow{n_{\alpha}}=0}$, gde je $\ \:\mathrm{P}(x_{0},\,y_{0},\,z_{0})\in p$, $\ \:\overrightarrow{n_{p}}\:$ normalni vektor.
  $(x-x_{0},\,y-y_{0},\,z-z_{0})\circ(a,\,b,\,c)=0$
  $a(x-x_{0})+b(y-y_{0})+c(z-z_{0})=0$
  $ax+by+cz\underbrace{-ax_{0}-by_{0}-cz_{0}}_{=\,d}=0$
  $\:$
- Parametarska jednačina
  $\mathrm{P}(x_{0},\,y_{0},\,z_{0})\in p$, $\ \:\overrightarrow{u}=(u_{x},\,u_{y},\,u_{z}),\ \overrightarrow{v}=(v_{x},\,v_{y},\,v_{z})\:$ su dva nekolinearna vektora paralelna ravni $\alpha$.
  > $\overrightarrow{n_{\alpha}}\perp\overrightarrow{u},\,\overrightarrow{v}\quad\Leftrightarrow\quad \overrightarrow{n_{\alpha}}\circ \overrightarrow{u}=\overrightarrow{n_{\alpha}}\circ \overrightarrow{v}=0$
  
  $\alpha:\ \mathrm{M}(t)=\mathrm{P}+t_{1}\,\overrightarrow{u}+t_{2}\,\overrightarrow{v},\quad t_{1},\,t_{2}\in\mathbb{R}$
  $\:$
  $\alpha:\ \begin{cases}x=x_{0}+t_{1}\,u_{x}+t_{2}\,v_{x}\\y=y_{0}+t_{1}\,u_{y}+t_{2}\,v_{y}\\z=z_{0}+t_{1}\,u_{z}+t_{2}\,v_{z}\end{cases}\quad t_{1},\,t_{2}\in\mathbb{R}$
___
Neka je $f(x,\,y,\,z)=0$ implicitna jednačina ravni $\alpha$. Tada
$C$ i $D$ su sa iste stane od $\alpha$ $\quad\Leftrightarrow\quad \mathrm{sgn}\,f(C)=\mathrm{sgn}f(D)$
### Prava
- Parametarska jednačina
  $\mathrm{P}(x_{0},\,y_{0},\,z_{0})\in p$, $\ \:\overrightarrow{p}=(p_{x},\,p_{y},\,p_{z})\:$ vektor pravca prave $p$.
  
  $p:\ \mathrm{M}(t)=\mathrm{P}+t\,\overrightarrow{p},\quad t\in\mathbb{R}$
  $\:$
  $p:\ \begin{cases}x=x_{0}+t\,p_{x}\\y = y_{0}+t\,p_{y}\\z=z_{0}+t\,p_{z}\end{cases}\quad t\in\mathbb{R}$
  $\:$
- Kanonska jednačina
$\begin{align}\frac{x-x_{0}}{p_{x}}=\frac{y-y_{0}}{p_{y}} = \frac{z-z_{0}}{p_{z}}=t\end{align}$
$\:$
- Kao presek dve ravni
  $p=\alpha\cap\beta$
  $\alpha:\ a_{1}x+b_{1}y+c_{1}z+d_{1}=0$
  $\beta:\ a_{2}x+b_{2}y+c_{2}z+d_{2}=0$
$\:$
$\Rightarrow\quad p:\ \begin{cases}a_{1}x+b_{1}y+c_{1}z+d_{1}=0\\a_{2}x+b_{2}y+c_{2}z+d_{2}=0\end{cases}$
$\overrightarrow{p}=\overrightarrow{n_{\alpha}}\times\overrightarrow{n_{\beta}}$
$\:$
> prebacivanje u parametarsku:
> izrazimo dve koordinate preko treće, na primer:
> $p:\ \begin{cases}x=c'_{1}z+d'_{1}\\y=c'_{2}z+d'_{2}\end{cases}$ $\quad$ odakle dobijamo $\left(\begin{array}{}x\\y\\z\end{array}\right)=\underbrace{\left(\begin{array}{}c'_{1}\\c'_{2}\\1\end{array}\right)}_{=\ \overrightarrow{p}}z+\underbrace{\left(\begin{array}{}d'_{1}\\d'_{2}\\0\end{array}\right)}_{=\ \mathrm{P}},\quad z\in\mathbb{R}$

### Pramen ravni
**Teorema**. Skup svih ravni koje sadrže pravu $p=\alpha\cap\beta$, $\begin{array}{}\alpha:\ a_{1}x+b_{1}y+c_{1}z+d_{1}=0\\\beta:\ a_{2}x+b_{2}y+c_{2}z+d_{2}=0\end{array}$ $\quad$ je dat jednačinom: 

$\chi_{\alpha,\,\beta}:\ \lambda_{1}(a_{1}x+b_{1}y+c_{1}z+d_{1})+\lambda_{2}(a_{2}x+b_{2}y+c_{2}z+d_{2})=0,\quad\lambda_{1},\,\lambda_{2}\in\mathbb{R}$
### Uzajamni položaj pravih
$p:\ \mathrm{P},\ \overrightarrow{p}$
$q:\ \mathrm{Q},\ \overrightarrow{q}$
- Poklapaju se:
  $p \equiv q\quad\Leftrightarrow\quad\begin{cases} \overrightarrow{p}=\lambda\,\overrightarrow{q},\quad \lambda\in \mathbb{R}\\\mathrm{P}\in p\quad\Rightarrow\quad\mathrm{P}\in q\end{cases}$
  $\:$
- Paralelne:
  $p \parallel q\quad\Leftrightarrow\quad\begin{cases} \overrightarrow{p}=\lambda\,\overrightarrow{q},\quad \lambda\in \mathbb{R}\\\mathrm{P}\in p\quad\Rightarrow\quad\mathrm{P}\notin q\end{cases}$ 
  $\:$
- Seku se:
  $p\text{ i }q \text{ se seku}\quad\Leftrightarrow\quad\exists \mathrm{M}(x_{0},\,y_{0})\ \ : \ \ \mathrm{M}\in p\ \text{ i }\  \mathrm{M}\in q$
  $\:$
- Mimoilazne:
  $p\text{ i }q \text{ su mimoilazne}\quad\Leftrightarrow\quad\nexists \alpha\ \ : \ \ p\subset\alpha\ \text{ i }\  q\subset\alpha$
$\:$

> Algoritam određivanja uzajamnog položaja pravih $p$ i $q$ :
> 1. Ako važi  $\Big[\overrightarrow{p},\ \overrightarrow{q},\ \overrightarrow{\rm PQ}\Big]\ne 0$ onda su **mimoilazne**
> 2. Inače, ako važi $\Big[\overrightarrow{p},\ \overrightarrow{q}\,\Big]\ne \overrightarrow{0}$ $\Big(\text{tj. }\ \ \nexists \lambda\in\mathbb{R} \ \ :\ \ \overrightarrow{p}=\lambda\,\overrightarrow{q}\,\Big)$ onda **se seku**
> 3. Inače, ako $\mathrm{P}\in q$ onda **se poklapaju** u suprotnom su **paralelne**

$\:$

### Uzajamni položaj prave i ravni
$p:\ \mathrm{P},\ \overrightarrow{p}$
$\alpha:\ ax+by+cz+d=0$
- Prava leži u ravni:
  $p \subset \alpha\quad\Leftrightarrow\quad\begin{cases} \overrightarrow{n_{\alpha}}\perp \overrightarrow{p},\quad\Big(\text{tj. }\ \ \overrightarrow{n_{\alpha}}\circ \overrightarrow{p}=0\Big)\\\mathrm{P}\in p\quad\Rightarrow\quad\mathrm{P}\in \alpha\end{cases}$
  $\:$
- Paralelne:
  $p \parallel \alpha\quad\Leftrightarrow\quad\begin{cases} \overrightarrow{n_{\alpha}}\perp \overrightarrow{p},\quad\Big(\text{tj. }\ \ \overrightarrow{n_{\alpha}}\circ \overrightarrow{p}=0\Big)\\\mathrm{P}\in p\quad\Rightarrow\quad\mathrm{P}\notin \alpha\end{cases}$ 
  $\:$
- Prava seče ravan:
  $p\text{ i }\alpha \text{ se seku}\quad\Leftrightarrow\quad\exists \mathrm{M}(x_{0},\,y_{0})\ \ : \ \ \mathrm{M}\in p\ \text{ i }\  \mathrm{M}\in \alpha$

### Rastojanja i uglove

**Stav**. <u>Rastojanje tačke</u> $\mathrm{M}$ <u>od prave</u> $p:\ P,\,\overrightarrow{\rm p}$ $\ \:$ je
$\begin{align}\mathrm{d}(\mathrm{M},\,p)=\frac{|| \overrightarrow{\rm MP}\times\overrightarrow{p}\,||}{||\, \overrightarrow{p}\,||}\end{align}$ 
> Dokaz: Neka je $d=\mathrm{d}(M,\,p)$
> Površinu paralelograma određenog sa $\overrightarrow{p}$ i $\overrightarrow{\rm PM}$ možemo naći na dva načina: $\mathrm{P}=|| \overrightarrow{\rm MP}\times\overrightarrow{p}\,||=d\cdot||\, \overrightarrow{p}\,||$. Odakle sledi tvrđenje.  ^f9c9c9

$\:$
**Stav**. <u>Rastojanje tačke</u> $\mathrm{M}(x_{0},\,y_{0},\,z_{0})$ <u>od ravni</u> $\alpha:\ ax+by+cz+d=0$ je $\begin{align}\mathrm{d}(\mathrm{M},\,\alpha)=\frac{|ax_{0}+by_{0}+cz_{0}+d|}{\sqrt[]{a^{2}+b^{2}+c^{2}}}\end{align}$
> Dokaz je sličan dokazu za [[Analitička geometrija u ravni#^02dde3|rastojanje tačke od prave u ravni]]

$\:$
**Stav**. <u>Rastojanje među mimoilaznih pravih</u> $p:\ \mathrm{P},\ \overrightarrow{p}$ $\ \:$ i $\ \:$ $q:\ \mathrm{Q},\ \overrightarrow{q}$ $\ \:$ je
$\begin{align}\mathrm{d}(p,\,q)=\frac{\Big|[\,\overrightarrow{p},\,\overrightarrow{q},\,\overrightarrow{\rm PQ}\,]\Big|}{||\, \overrightarrow{p} \times \overrightarrow{q}\, ||}\end{align}$
___
**Stav**. <u>Ugao među pravih</u> $p:\ \mathrm{P},\ \overrightarrow{p}$ $\ \:$ i $\ \:$ $q:\ \mathrm{Q},\ \overrightarrow{q}$ $\ \:$ je
$\begin{align}\widehat{(p,\,q)}=\text{oštar }\widehat{(\,\overrightarrow{p},\ \overrightarrow{q}\,)}=\arccos\frac{| \,\overrightarrow{p}\circ \overrightarrow{q}\,|}{||\,\overrightarrow{p}\,||\cdot||\,\overrightarrow{ q}\,||}\end{align}$
$\:$

**Stav**. <u>Ugao među prave</u> $p:\ \mathrm{P},\ \overrightarrow{p}$ $\ \:$ i $\ \:$ <u>ravni</u>  $\alpha:\ \mathrm{A},\ \overrightarrow{n}_{\alpha}$ $\ \:$ je
$\begin{align}\widehat{(p,\,\alpha)}=\widehat{(p,\,p')}=\frac{\pi}{2}-\text{oštar }\widehat{(\,\overrightarrow{p},\ \overrightarrow{n}_{\alpha}\,)}=\end{align}$

$\begin{align}=\frac{\pi}{2}-\arccos\frac{| \,\overrightarrow{p}\circ \overrightarrow{n}_{\alpha}\,|}{||\,\overrightarrow{p}\,||\cdot||\,\overrightarrow{n}_{\alpha}\,||}=\arcsin\frac{| \,\overrightarrow{p}\circ \overrightarrow{n}_{\alpha}\,|}{||\,\overrightarrow{p}\,||\cdot||\,\overrightarrow{n}_{\alpha}\,||}\end{align}$
$\:$

**Stav**. <u>Ugao među ravni</u> $\alpha:\ \mathrm{A},\ \overrightarrow{n}_{\alpha}$ $\ \:$ i $\ \:$ $\beta:\ \mathrm{B},\ \overrightarrow{n}_{\beta}$ $\ \:$ je
$\begin{align}\widehat{(\alpha,\,\beta)}=\text{oštar }\widehat{(\,\overrightarrow{n}_{\alpha},\ \overrightarrow{n}_{\beta}\,)}=\arccos\frac{| \,\overrightarrow{n}_{\alpha}\circ \overrightarrow{n}_{\beta}\,|}{||\,\overrightarrow{n}_{\alpha}\,||\cdot||\,\overrightarrow{ n}_{\beta}\,||}\end{align}$

### Projektovanje 
**Stav**. Projekcija tačke $\mathrm{X}$ <u>na ravan</u> $\alpha$ koja prolazi kroz koordinatni početak je tačka $\mathrm{X}'$, takva da $\boxed{[\mathrm{X}']=(E-n\,n^{\mathrm{T}})[\mathrm{X}]}$, gde je $n$ jedinični vektor normali na ravan $\alpha$. 
Odakle, projektovanje na ravan $\alpha$ je [[Afino preslikavanje|afino preslikavanje]] prostora.
>  Dokaz:
>  $\overrightarrow{\rm OX}=\overrightarrow{\rm OX'}+ \overrightarrow{\rm X'X}=\overrightarrow{\rm OX'}+\lambda\,\overrightarrow{n},\quad \lambda\in\mathbb{R}$
>  Skalarno množimo sa $\overrightarrow{n}$:
>  $\overrightarrow{\rm OX}\circ\overrightarrow{n}=\underbrace{\overrightarrow{\rm OX'}\circ\overrightarrow{n}}_{=\,0}+\lambda\cdot\underbrace{\overrightarrow{n}\circ\overrightarrow{n}}_{=\,{||\,\overrightarrow{n}\,||}^{2}=\,1}=\lambda$
>
>$\begin{align}[\mathrm{X'}]&=\overrightarrow{\rm OX'}=\overrightarrow{\rm OX}-\lambda\,\overrightarrow{n}=\overrightarrow{\rm OX}-\Big(\overrightarrow{\rm OX}\circ\overrightarrow{n}\Big)\,\overrightarrow{n}=\\&\overset{\text{?}}{=}\overrightarrow{\rm OX}-(n\,n^{\rm T})\,\overrightarrow{\rm OX}=(E-n\,n^{\rm T})[\mathrm{X}]\end{align}$
>
>>$\text{?}$ — Neka je $\overrightarrow{\rm OX}=\left(\begin{array}{}x\\y\\z\end{array}\right)$ $\ \:$ i $\ \:$ $\overrightarrow{n} = \left(\begin{array}{}a\\b\\c\end{array}\right)$. Tada 
>>$\Big(\overrightarrow{\rm OX}\circ\overrightarrow{n}\Big)\,\overrightarrow{n}=(ax+by+cz)\left(\begin{array}{}a\\b\\c\end{array}\right)=\left(\begin{array}{}a^{2}x+aby+acz\\abx+b^{2}y+bcz\\acx+bcy+c^{2}z\end{array}\right)=$
>>$=\left(\begin{array}{}a^{2}&ab&ac\\ab&b^{2}&bc\\ac&bc&c^{2}\end{array}\right)\left(\begin{array}{}x\\y\\z\end{array}\right)=(n\,n^{\rm T})\,\overrightarrow{\rm OX}$

$\:$
### Prodor prave kroz trougao 
