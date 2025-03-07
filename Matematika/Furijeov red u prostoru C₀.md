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

Nizovi $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$ su **Furijeovi koeficijenti*** (stvarni [[Prostor C₀#^558e23|Furijeovi koeficijenti]]).

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
___
$\:$
**Teorema** (dovoljni uslov konvergencije Furijeovog reda). 
Neka je $f:\ \mathbb{R}\to\mathbb{R}$ $\ \:$ $2\pi$−periodična funkcija koja je deo po deo [[Neprekidnost#^0977f9|(?]][[Izvod#^35db14|?)]] [[Izvod#^72f43e|glatka]] $\Big($tj. $\mathcal{C}^{1}\Big)$ na intervalu $(-\pi,\,\pi)$ i neka su $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$  Furijeovi koeficijenti funkcije $f$. Tada
- $\begin{align}\forall x\in(-\pi,\,\pi)\quad\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos nx+b_{n}\sin nx\big)=\frac{f(x^{+})+f(x^{-})}{2}\end{align}$
- $\begin{align}\forall x\in\{-\pi,\,\pi\}\quad\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos nx+b_{n}\sin nx\big)=\frac{f(-\pi^{+})+f(\pi^{-})}{2}\end{align}$

**Posledica**. Neka je $f:\ \mathbb{R}\to\mathbb{R}$ $\ \:$ <u>neprekidna</u> $2\pi$−periodična funkcija koja je deo po deo  glatka na intervalu $(-\pi,\,\pi)$ i neka su $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$  Furijeovi koeficijenti funkcije $f$. Tada
$\begin{align}\forall x\in(-\pi,\,\pi)\quad\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}\big(a_{n}\cos nx+b_{n}\sin nx\big)=f(x)\end{align}$

___
**Teorema** (Parsevalova jednakost). 
Neka je $f:\ \mathbb{R}\to\mathbb{R}$ $\ \:$ $2\pi$−periodična funkcija koja je deo po deo glatka  na intervalu $(-\pi,\,\pi)$ i neka su $\big(a_{n}\big)_{n\in\mathbb{N}_{0}}$ i $\big(b_{n}\big)_{n\in\mathbb{N}}$  Furijeovi koeficijenti funkcije $f$. Tada ako $\begin{align}\int_{-\pi}^{\pi} \big(f(x)\big)^{2} \, dx \end{align}$ konvergira važi $\boxed{\begin{align}\frac{a^{2}_{0}}{2}+\sum\limits_{n=1}^{\infty}(a^{2}_{n}+b^{2}_{n})=\frac{1}{\pi}\int_{-\pi}^{\pi} \big(f(x)\big)^{2} \, dx \end{align}}$

**Teorema**.  $f,\,g\in\mathcal{C}_{0}[-\pi,\,\pi]$. Tada
- Furijeov red funkcije $f$ [[Prostor C₀#^e4918f|konvergira toj funkciji u srednjem]].
- ako su svi Furijeovi koeficijenti funkcije $f$ jednaki $0$ onda je $f = 0$.
- ako funkcije $f$ i $g$ imaju jednake odgovarajuće Furijeove koeficijente onda je $f = g$.