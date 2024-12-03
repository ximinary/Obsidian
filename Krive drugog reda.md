#fax #math #geom  [deo [[Geometrija|geometrije]]]


### Konus i konusni preseci

**Def**. Neka prave $s$ i $i$ se seku u tački $\mathrm{T}$. Površ dobijena rotacijom $i$ oko prave $s$ se zove **kružni konus**. 
$\mathrm{T}$ je **teme** konusa, $i$ je **izvodnica** konusa, a $s$ je **osa** konusa.

**Def**. **Konusni presek** je presek kružnog konusa i bilo koje ravni.

- Ako ravan sadrži teme konusa, presek je **degenerisan**: može da bude tačka, prava ili dve prave koje se seku.
- Ako ravan ne sadrži teme konusa, presek je **konika**: može da bude krug, elipsa, parabola ili hiperbola.
![[konusni preseci.png]]


**Teorema**. Za svaku koniku postoje tačka $\mathrm{F}$ i prava $d$ takva da broj $\begin{align}e = \frac{\mathrm{MF}}{\mathrm{d}(\mathrm{M},\,d)}\end{align}$ konstantan za svaku tačku $\mathrm{M}$ konike.

$\mathrm{F}$ je **žiža**, $d$ je **direktrisa**, a $e\geqslant0$ je **ekscentritet** konike. 

- krug $(e=0)$, $F$ je centar kruga, $d$ je beskonačno daleka prava.
- elipsa $(0<e<1)$, ima dve pare žiže i direktrise.
- parabola $(e=1)$, ima jednu paru žiže i direktrise.
- hiperbola $(e>1)$, ima dve pare žiže i direktrise.

### Krug
Krug $k(\mathrm{C},\,r)$ sa centrom u $\mathrm{C}(x_{0},\,y_{0})$ u poluprečnikom $r$ je skup tačaka $\mathrm{M}(x,\,y)$ za koje $|| \overrightarrow{\rm CM}||=r$

Odakle sledi implicitna jednačina kruga:
$(x-x_{0})^{2}+(y-y_{0})^{2}=r^{2}$

I parametarska jednačina kruga:
$\begin{align}\mathrm{M} = \mathrm{C} + \overrightarrow{\rm CM}\quad\Leftrightarrow\quad\binom{x}{y}=\binom{x_{0}}{y_{0}}+\binom{r\,\cos\varphi}{r\,\sin\varphi}\end{align}$,
gde je $\varphi\in[0,\,2\pi)$ ugao između $\overrightarrow{\rm CM}$ i ose $\mathrm{O}x$



### Elipsa
Elipsa sa poluosama $a$ i $b$ ($0<a\leqslant b$) je određena jednačinom $\begin{align}\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}=1\end{align}$

![[elipsa.png]]

$c=\mathrm{OF}_{1}=\mathrm{OF}_{2}=\sqrt[]{a^{2}-b^{2}}$

Žiže: $\mathrm{F}_{1}(c,\,0)$ $\ \:$ i $\ \:$ $\mathrm{F}_{2}(-c,\, 0)$

Direktrise: $\begin{align}d_{1}:\,x=\frac{a^{2}}{c}\end{align}$ $\ \:$ i $\ \:$ $\begin{align}d_{2}:\,x=-\frac{a^{2}}{c}\end{align}$

Ekscentritet: $\begin{align}e=\frac{c}{a}\end{align}$

> Specijalni slučajevi:
> $a=b$, dobija se krug $e= 0$
> $a\to+\infty$, dobija se parabola $e=1$

$\:$
Parametarska jednačina:
Iz implicitne $\begin{align}\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}=1\end{align}$ $\ \:$ smenom $\ \:$ $\begin{align}\frac{x}{a}=\cos\varphi\quad\ \bigg(\frac{y}{b}=\sin\varphi\bigg)\end{align}$
Dobija se jednačina $\begin{align}\mathrm{M}=\binom{a\,\cos\varphi}{b\,\sin\varphi}\end{align}$

**Teorema**. Za svaku tačku $\mathrm{M}$ elipse važi $\mathrm{MF}_{1}+\mathrm{MF}_{2}=2a$
> Dokaz:
> $\mathrm{MF}_{1}+\mathrm{MF}_{2}=e\cdot\mathrm{d}(\mathrm{M},\,d_{1})+e\cdot\mathrm{d}(\mathrm{M},\,d_{2})=e\cdot\mathrm{d}(d_{1},\,d_{2})=$
> $\begin{align}=e\cdot2\frac{a^{2}}{c}=e\cdot2\frac{a}{e}=2a\end{align}$

### Parabola

##### Kosi hitac

### Hiperbola
