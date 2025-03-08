#fax #math #a2 [deo poglavlja [[Funkcionalni red|"funkcionalni red"]] i [[Prostor C₀|"prostor C₀"]]]
$\:$

**Def**. Neka su $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$ [[Niz brojeva|nizovi realnih brojeva]]. Tada [[Funkcionalni red|funkcionalni red]] $\boxed{\begin{align}\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos nx+b_{n}\sin nx\big)\end{align}}$ naziva se **trigonometrijski red**.

> Napomena: ako navedeni red konvergira/divergira u $x=x_{0}$ tada on konvergira/divergira i u $x=x_{0}+2\pi k,\quad k\in\mathbb{Z}$.
> Zbog toga dovoljno je ispitivati konvergenciju u nekom intervalu dužine $2\pi$, na primer $[-\pi,\,\pi]$.

$\:$
**Stav**. Neka trigonometrijski red $\begin{align}\ \:\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos nx+b_{n}\sin nx\big)\ \:\end{align}$ ravnomerno konvergira ka funkciji $f:\ [−\pi, \pi]\to\mathbb{R}$ na intervalu $[−\pi, \pi]$. Tada

$\boxed{\begin{align}&a_{n}=\frac{1}{\pi}\int_{-\pi}^{\pi} f(x)\cos nx \, dx,\quad\forall n\in\mathbb{N}_{0}\\\\&b_{n}=\frac{1}{\pi}\int_{-\pi}^{\pi} f(x)\sin nx \, dx,\quad\forall n\in\mathbb{N}\end{align}}$

$\:$
**Def**. Trigonometrijski red formiran pomoću $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$  dobijenih u prethodnom stavu se naziva **Furijeov red** funkcije $f:\ [-\pi,\,\pi]\to\mathbb{R}$ na intervalu $[-\pi, \pi]$ $\Big($ ili $2\pi$-periodične funkcije $f:\ \mathbb{R}\to\mathbb{R}$ na skupu $\mathbb{R}$ $\Big)$.

Nizovi $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$ su **Furijeovi\* koeficijenti** (stvarni [[Prostor C₀#^558e23|Furijeovi koeficijenti]]).

$\:$

>Furijeov red $2l$-periodične funkcije $f$ je
$\begin{align}\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos \frac{n\pi x}{l}+b_{n}\sin \frac{n\pi x}{l}\big)\end{align}$ 
>
>$\begin{align}&a_{n}=\frac{1}{l}\int_{-l}^{l} f(x)\cos \frac{n\pi x}{l} \, dx,\quad\forall n\in\mathbb{N}_{0}\\\\&b_{n}=\frac{1}{l}\int_{-l}^{l} f(x)\sin \frac{n \pi x}{l} \, dx,\quad\forall n\in\mathbb{N}\end{align}$
___

**Sinusni Furijeov red funkcije** $f$ jeste Furijeov red funkcije $g:\ [-\pi, \pi]\to\mathbb{R}$
definisane sa $g(x):=\begin{cases}f (x), &x \in [0, \pi]\\-f(-x), &x\in[-\pi,\,0) \end{cases}$

**Kosinusni Furijeov red funkcije** $f$ jeste Furijeov red funkcije $g:\ [-\pi, \pi]\to\mathbb{R}$
definisane sa $g(x):=\begin{cases}f (x), &x \in [0, \pi]\\f(-x), &x\in[-\pi,\,0) \end{cases}$

### Konvergencija i svojstva Furijeovog reda
**Teorema** (dovoljni uslov konvergencije Furijeovog reda). 
Neka je $f:\ [-\pi,\,\pi]\to\mathbb{R}$ $\ \:$ deo po deo [[Izvod#^72f43e|glatka]] $\Big($tj. $\mathcal{C}^{1}\Big)$ funkcija i neka su $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$  Furijeovi\* koeficijenti funkcije $f$. Tada
- $\begin{align}\forall x\in(-\pi,\,\pi)\quad\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos nx+b_{n}\sin nx\big)=\frac{f(x^{+})+f(x^{-})}{2}\end{align}$
- $\begin{align}\forall x\in\{-\pi,\,\pi\}\quad\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos nx+b_{n}\sin nx\big)=\frac{f(-\pi^{+})+f(\pi^{-})}{2}\end{align}$

> tj. ako još važi $f\in \mathcal{C}_{0}[-\pi,\,\pi]$ onda Furijeov red funkcije $f$ konvergira ka $f$.

$\:$
**Posledica**. Neka je $f:\ \mathbb{R}\to\mathbb{R}$ $\ \:$ <u>neprekidna</u> $2\pi$−periodična funkcija koja je deo po deo  glatka na intervalu $(-\pi,\,\pi)$ i neka su $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$  Furijeovi* koeficijenti funkcije $f$. Tada
$\begin{align}\forall x\in\mathbb{R}\quad\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos nx+b_{n}\sin nx\big)=f(x)\end{align}$ ^6d2118

___
**Teorema** ([[Beskonačnodimenzioni Euklidski prostor. Niz i red vektora#^927ed4|Parsevalova jednakost]]). 
Neka je $f\in \mathcal{C}_{0}[-\pi,\,\pi]$ i neka su $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$  Furijeovi koeficijenti funkcije $f$. Tada  $\boxed{\begin{align}\frac{a^{2}_{0}}{2}+\sum\limits_{n=1}^{\infty}(a^{2}_{n}+b^{2}_{n})=\frac{1}{\pi}\int_{-\pi}^{\pi} \big(f(x)\big)^{2} \, dx \end{align}}$ ^fe25e7

**Teorema**.  $f,\,g\in\mathcal{C}_{0}[-\pi,\,\pi]$. Tada
- Furijeov red funkcije $f$ [[Prostor C₀#^e4918f|konvergira toj funkciji u srednjem]].
- ako su svi Furijeovi koeficijenti funkcije $f$ jednaki $0$ onda je $f = 0$.
- ako funkcije $f$ i $g$ imaju jednake odgovarajuće Furijeove koeficijente onda je $f = g$.
___
**Teorema** (dovoljni uslov apsolutne i ravnomerne konvergencije Furijeovog reda). Neka je $f:\ \mathbb{R}\to\mathbb{R}$ $\ \:$ neprekidna $2\pi$-periodična funkcija koja je deo po deo glatka na $(-\pi,\,\pi)$. Tada Furijeov red funkcije $f$ apsolutno i ravnomerno konvergira ka funkciji $f$ na $\mathbb{R}$. ^c4c4a9
> Dokaz: 
> Neka je $g:\ [-\pi,\,\pi]\to\mathbb{R}$ definisana sa
> 
> $\begin{align}g(x)=\begin{cases}f'(x),&x\in(-\pi,\,\pi)\ \text{ i postoji } f'(x)\\\\ \frac{f'(x^{+})+f'(x^{-})}{2},&x\in(-\pi,\,\pi)\ \text{ i ne postoji }f'(x)\\\\ \frac{f'(-\pi^{+})+f'(\pi^{-})}{2},&x\in\{-\pi,\,\pi\}\end{cases}\end{align}$
> 
> Iz definicije je jasno da $g\in\mathcal{C}_{0}[-\pi,\,\pi]$ $\quad$ ([[Prostor C₀|**]])
> 
> Neka su $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$ Furijeovi\* koeficijenti funkcije $f$,
> a $\big(a'_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b'_{n}\big)_{n\in\mathbb{N}}$ Furijeovi\* koeficijenti funkcije $g$.
>
> $\begin{align}\forall n\in\mathbb{N} \quad a'_{n}&=\frac{1}{\pi}\int_{-\pi}^{\pi} g(x)\cos nx  \, dx=\left(\begin{array}{}u = \cos nx&du = -n\sin nx\\dv = g(x)\,dx&v=f(x)\end{array}\right)=\\&=\frac{1}{\pi}\left(f(x)\,\cos nx\bigg|_{-\pi}^{\pi} +\int_{-\pi}^{\pi}n\,f(x)\sin nx   \, dx\right)=\\&=\frac{n}{\pi}\int_{-\pi}^{\pi} f(x)\sin nx  \, dx=n\,b_{n}\end{align}$
> 
> $\begin{align}\forall n\in\mathbb{N} \quad b'_{n}&=\frac{1}{\pi}\int_{-\pi}^{\pi} g(x)\sin nx  \, dx=\left(\begin{array}{}u = \sin nx&du = -n\cos nx\\dv = g(x)\,dx&v=f(x)\end{array}\right)=\\&=-\frac{n}{\pi}\int_{-\pi}^{\pi} f(x)\cos nx  \, dx=-n\,a_{n}\end{align}$
>
> $\:$
> >$\begin{align}\forall x,\,y\in\mathbb{R} \quad& (|x|-|y|)^{2}=x^{2}-2|x|\cdot|y|+y^{2}\geqslant0\\&\Rightarrow\quad|xy|\leqslant\frac{1}{2}(x^{2}+y^{2})\quad\quad\quad\quad\quad\quad\quad\quad(1)\end{align}$
>
> $\:$  
> $\begin{align}|a_{n}\cos nx +b_{n}\sin nx|&\leqslant|a_{n}|+|b_{n}|=\Bigg|-\frac{b'_{n}}{n}\Bigg|+\Bigg|\frac{a'_{n}}{n}\Bigg|=\frac{|b'_{n}|}{n}+\frac{|a'_{n}|}{n}\overset{(1)}\leqslant\\&\leqslant\frac{1}{2}\bigg((a'_{n})^{2}+\frac{1}{n^{2}}\bigg)+\frac{1}{2}\bigg((b'_{n})^{2}+\frac{1}{n^{2}}\bigg)=\frac{(a'_{n})^{2}+(b'_{n})^{2}}{2}+\frac{1}{n^{2}}\end{align}$
> 
> Odakle, jer brojevni redovi $\begin{align}\sum\limits_{n=1}^{\infty} \Big((a'_{n})^{2}+(b'_{n})^{2}\Big)\end{align}$  ([[Beskonačnodimenzioni Euklidski prostor. Niz i red vektora#^36e255|?]]) $\:$ i $\:$ $\begin{align}\sum\limits_{n=1}^{\infty} \frac{1}{n^{2}}\end{align}$ konvergiraju iz [[Funkcionalni red#^b72d33|Vajerštrasova kriterijuma]] funkcionalni red $\begin{align}\sum\limits_{n=1}^{\infty} |a_{n}\,\cos nx+b_{n}\,\sin nx|\end{align}$ konvergira ravnomerno, a samim tim Furijeov red apsolutno i ravnomerno konvergira ka $f$ (što konvergira ka $f$ je jasno iz [[Furijeov red u prostoru C₀#^6d2118|posledice]]). 

$\:$
### Diferenciranje i integracija Furijeovog reda

**Teorema** (diferenciranje). Neka je $f:\ \mathbb{R}\to\mathbb{R}$ $\ \:$ glatka $2\pi$-periodična funkcija i neka su $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$  Furijeovi koeficijenti funkcije $f$. Tada ako je $f'$ deo po deo glatka važi

$\begin{align}\forall x\in\mathbb{R}\quad f'(x)=\bigg(\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos nx +b_{n}\sin nx\big)\bigg)'=\sum\limits_{n=1}^{\infty}n\big(-a_{n}\sin nx+b_{n}\cos nx\big)\end{align}$
> Dokaz:
> Prvo ćemo pokazati da desni red ravnomerno konvergira.
>  
> Neka je $g:\ [-\pi,\,\pi]\to\mathbb{R}$ definisana sa
> 
> $\begin{align}g(x)=\begin{cases}f''(x),&x\in(-\pi,\,\pi)\ \text{ i postoji } f''(x)\\\\ \frac{f''(x^{+})+f''(x^{-})}{2},&x\in(-\pi,\,\pi)\ \text{ i ne postoji }f''(x)\\\\ \frac{f''(-\pi^{+})+f''(\pi^{-})}{2},&x\in\{-\pi,\,\pi\}\end{cases}\end{align}$
> 
> Iz definicije je jasno da $g\in\mathcal{C}_{0}[-\pi,\,\pi]$ $\quad$ ([[Prostor C₀|**]])
> 
> Neka su $\big(a''_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b''_{n}\big)_{n\in\mathbb{N}}$ Furijeovi\* koeficijenti funkcije $g$.
>
> Slično kao u prethodnoj teoremi:
> $\begin{align}\forall n\in\mathbb{N} \quad a''_{n}=\frac{1}{\pi}\int_{-\pi}^{\pi} g(x)\cos nx  \, dx=-\frac{n^{2}}{\pi}\int_{-\pi}^{\pi} f(x)\cos nx  \, dx=-n^{2}\,a_{n}\end{align}$
> 
> $\begin{align}\forall n\in\mathbb{N} \quad b''_{n}=\frac{1}{\pi}\int_{-\pi}^{\pi} g(x)\sin nx  \, dx=-\frac{n^{2}}{\pi}\int_{-\pi}^{\pi} f(x)\sin nx  \, dx=-n^{2}\,b_{n}\end{align}$
> 
> $\:$  
> $\begin{align}\Big|n\big(-a_{n}\sin nx+b_{n}\cos nx\big)\Big|&\leqslant n|a_{n}|+n|b_{n}|=n\Bigg|-\frac{a''_{n}}{n^{2}}\Bigg|+n\Bigg|-\frac{b''_{n}}{n^{2}}\Bigg|=\frac{|a''_{n}|}{n}+\frac{|b''_{n}|}{n}\overset{(1)}\leqslant\\&\leqslant\frac{1}{2}\bigg((a''_{n})^{2}+\frac{1}{n^{2}}\bigg)+\frac{1}{2}\bigg((b''_{n})^{2}+\frac{1}{n^{2}}\bigg)=\frac{(a''_{n})^{2}+(b''_{n})^{2}}{2}+\frac{1}{n^{2}}\end{align}$
> 
> Odakle, jer brojevni redovi $\begin{align}\sum\limits_{n=1}^{\infty} \Big((a''_{n})^{2}+(b''_{n})^{2}\Big)\end{align}$ ([[Beskonačnodimenzioni Euklidski prostor. Niz i red vektora#^36e255|?]]) $\:$ i $\:$ $\begin{align}\sum\limits_{n=1}^{\infty} \frac{1}{n^{2}}\end{align}$ konvergiraju iz [[Funkcionalni red#^b72d33|Vajerštrasova kriterijuma]] funkcionalni red $\begin{align}\sum\limits_{n=1}^{\infty} \Big|n\big(-a_{n}\sin nx+b_{n}\cos nx\big)\Big|\end{align}$ konvergira ravnomerno.
> 
> Pomoću [[Svojstva ravnomerno konvergentnih funkcionalnih redova#^717181|teoreme]] dobijamo tvrđenje.


$\:$
**Teorema** (integracija). Neka je $f\in\mathcal{C}_{0}[-\pi,\,\pi]$ $\ \:$  i neka su $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$  Furijeovi koeficijenti funkcije $f$. Tada (nezavisno od toga da li Furijeov red funkcije $f$ konvergira ili ne) važi

$\begin{align}\forall x \in [-\pi,\,\pi]\quad \int_{0}^{x} f(t) \, dt &=\int_{0}^{x} \bigg(\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos nt+b_{n}\sin nt\big) \bigg) \, dt =\\\\&=\int_{0}^{x} \frac{a_{0}}{2} \, dt+\sum\limits_{n=1}^{\infty}\int_{0}^{x} \big(a_{n}\cos nt+b_{n}\sin nt\big) \, dt\\\\&= \frac{a_{0}}{2}x+\sum\limits_{n=1}^{\infty}\frac{1}{n}\big(a_{n}\sin nx+b_{n}(1-\cos nx)\big)\end{align}$
i navedeni red ravnomerno konvergira na $[-\pi,\,\pi]$
> Dokaz: Neka je $F:\ [-\pi,\,\pi]\to\mathbb{R}$ def sa $\begin{align}F(x)=\int_{0}^{x}\bigg( f(x) - \frac{a_{0}}{2}\bigg) \, dx \end{align}$
> $f\in\mathcal{C}_{0}[-\pi,\,\pi]\quad\Rightarrow\quad f\,\mathcal{R}\,[-\pi,\,\pi]\quad\Rightarrow\quad (f-\frac{a_{0}}{2})\,\mathcal{R}\,[-\pi,\,\pi]\quad\Rightarrow\quad$ $F$ je neprekidna ([[Veza između određenog integrala i izvoda. Njutn-Lajbnicova formula#^4ce901|?]]) i deo po deo glatka.
> 
> $\begin{align}F(\pi)-F(-\pi)=\int_{-\pi}^{\pi} f(x) \, dx-\pi a_{0}=0\quad\bigg(\text{jer }\ a_{0}=\frac{1}{\pi}\int_{-\pi}^{\pi} f(x) \, dx\bigg)\end{align}$
> Odakle $F(-\pi)=F(\pi)$, stoga $F\in\mathcal{C}_{0}[-\pi,\,\pi]$
> 
> Iz [[Furijeov red u prostoru C₀#^c4c4a9|teoreme]] imamo da Furijeov red fje $F$ ravnomerno konvergira ka $f$. Neka su $\big(A_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(B_{n}\big)_{n\in\mathbb{N}}$ Furijeovi* koeficijenti od $F$ tada
> $\begin{align}\forall x\in[-\pi,\,\pi]\quad F(x)=\frac{A_{0}}{2}+\sum\limits_{n=1}^{\infty} \big(A_{n}\cos nx+B_{n}\sin nx\big)\end{align}$
> 
> $\begin{align}\forall n\in\mathbb{N} \quad A_{n}&=\frac{1}{\pi}\int_{-\pi}^{\pi} F(x)\cos nx  \, dx=-\frac{1}{\pi n}\int_{-\pi}^{\pi} F'(x)\sin nx  \, dx=\\&=-\frac{1}{\pi n}\int_{-\pi}^{\pi}\bigg( f(x)+\frac{a_{0}}{2} \bigg) \sin nx \, dx=-\frac{b_{n}}{n}\end{align}$
> 
> $\begin{align}\forall n\in\mathbb{N} \quad B_{n}&=\frac{1}{\pi}\int_{-\pi}^{\pi} F(x)\sin nx  \, dx=\frac{1}{\pi n}\int_{-\pi}^{\pi} F'(x)\cos nx  \, dx=\\&=\frac{1}{\pi n}\int_{-\pi}^{\pi} \bigg( f(x)+\frac{a_{0}}{2} \bigg)\cos nx \, dx=\frac{a_{n}}{n}\end{align}$
> 
> $\begin{align}0=F(0)=\frac{A_{0}}{2}+\sum\limits_{n=1}^{\infty} A_{n}\quad\Rightarrow\quad A_{0}=-2\sum\limits_{n=1}^{\infty}A_{n}=2\sum\limits_{n=1}^{\infty}\frac{b_{n}}{n}\end{align}$
>
> Konačno,
> $\begin{align}\forall x\in[-\pi,\,\pi]\quad F(x)&=\frac{A_{0}}{2}+\sum\limits_{n=1}^{\infty} \big(A_{n}\cos nx+B_{n}\sin nx\big)\\&=\sum\limits_{n=1}^{\infty}\frac{b_{n}}{n}+\sum\limits_{n=1}^{\infty}\bigg(-\frac{b_{n}}{n}\cos nx+\frac{a_{n}}{n}\sin nx\bigg)=\\&=\sum\limits_{n=1}^{\infty}\frac{1}{n}\big(a_{n} \sin nx + b_{n}(1-\cos nx)\big)\end{align}$