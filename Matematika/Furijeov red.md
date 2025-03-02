#fax #math #a2 [deo poglavlja [[Funkcionalni red|"funkcionalni red"]]]
$\:$

**Def**. Neka su $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$ [[Niz brojeva|nizovi realnih brojeva]]. Tada [[Funkcionalni red|funkcionalni red]] $\boxed{\begin{align}\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos nx+b_{n}\sin nx\big)\end{align}}$ naziva se **trigonometrijski red**.

> Napomena: ako navedeni red konvergira/divergira u $x=x_{0}$ tada on konvergira/divergira i u $x=x_{0}+2\pi k,\quad k\in\mathbb{Z}$.
> Zbog toga dovoljno je ispitivati konvergenciju u nekom intervalu dužine $2\pi$, na primer $[-\pi,\,\pi]$.

$\:$
**Stav**. Neka trigonometrijski red $\begin{align}\ \:\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos nx+b_{n}\sin nx\big)\ \:\end{align}$ ravnomerno konvergira ka funkciji $f:\ [−\pi, \pi]\to\mathbb{R}$ na intervalu $[−\pi, \pi]$. Tada

$\boxed{\begin{align}&a_{n}=\frac{1}{\pi}\int_{-\pi}^{\pi} f(x)\cos kx \, dx,\quad\forall n\in\mathbb{N}_{0}\\\\&b_{n}=\frac{1}{\pi}\int_{-\pi}^{\pi} f(x)\sin kx \, dx,\quad\forall n\in\mathbb{N}\end{align}}$

$\:$
**Def**. Trigonometrijski red formiran pomoću $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$  dobijenih u prethodnom stavu se naziva **Furijeov red** funkcije $f:\ [-\pi,\,\pi]\to\mathbb{R}$ na intervalu $[-\pi, \pi]$ $\Big($ ili $2\pi$-periodične funkcije $f:\ \mathbb{R}\to\mathbb{R}$ na skupu $\mathbb{R}$ $\Big)$.

Nizovi $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$ su **Furijeovi koeficijenti**.

$\:$
**Sinusni Furijeov red funkcije** $f$ jeste Furijeov red funkcije $g:\ [-\pi, \pi]\to\mathbb{R}$
definisane sa $g(x):=\begin{cases}f (x), &x \in [0, \pi]\\-f(-x), &x\in[-\pi,\,0) \end{cases}$

**Kosinusni Furijeov red funkcije** $f$ jeste Furijeov red funkcije $g:\ [-\pi, \pi]\to\mathbb{R}$
definisane sa $g(x):=\begin{cases}f (x), &x \in [0, \pi]\\f(-x), &x\in[-\pi,\,0) \end{cases}$

$\:$
**Teorema** (dovoljni uslov konvergencije Furijeovog reda). 
Neka je $f:\ \mathbb{R}\to\mathbb{R}$ $\ \:$ $2\pi$−periodična funkcija koja je deo po deo [[Neprekidnost#^0977f9|(?]][[Izvod#^35db14|?)]] $\mathcal{C}^{1}$ na intervalu $(-\pi,\,\pi)$ i neka su $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$  Furijeovi koeficijenti funkcije $f$. Tada
- $\begin{align}\forall x\in(-\pi,\,\pi)\quad\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos nx+b_{n}\sin nx\big)=\frac{f(x^{+})+f(x^{-})}{2}\end{align}$
- $\begin{align}\forall x\in\{-\pi,\,\pi\}\quad\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos nx+b_{n}\sin nx\big)=\frac{f(-\pi^{+})+f(\pi^{-})}{2}\end{align}$

**Posledica**. Neka je $f:\ \mathbb{R}\to\mathbb{R}$ $\ \:$ <u>neprekidna</u> $2\pi$−periodična funkcija koja je deo po deo  $\mathcal{C}^{1}$ na intervalu $(-\pi,\,\pi)$ i neka su $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$  Furijeovi koeficijenti funkcije $f$. Tada
$\begin{align}\forall x\in(-\pi,\,\pi)\quad\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos nx+b_{n}\sin nx\big)=f(x)\end{align}$