#fax #math #a2 [deo [[Analiza|analize]]]


### Primitivna funkcija

Napomena: [[Izvod|izvod]]

**Def**. Funkcija $F:\ (a,\,b)\to\mathbb{R}$ je **primitivna funkcija za funkciju $f$ na intervalu** $(a,\,b)$ ako $F \,\mathcal{D}\,(a,\,b)\ \,$ i $\ \, \forall x\in (a,\,b)\quad F'(x)=f(x)$.

**Stav**. Neka je $f:\ (a,\,b)\to \mathbb{R}$; neka je $F:\ (a,\,b)\to \mathbb{R}\:$ primitivna za $f$ na $(a,\,b)$; $C\in\mathbb{R}$ — proizvoljno. Tada je $G:\ (a,\,b)\to \mathbb{R}$ def. sa $G(x):=F(x) + C$ primitivna za $f$ na $(a,\,b)$.
> Dokaz: 
> $G$ je diferencijabilna kao zbir diferencijabilnih.
> $\forall x\in (a,\,b)\to \mathbb{R}\quad G'(x)=\big(F(x)+C\big)'=F'(x)+0=f(x)$

**Teorema**. Neka je $f:\ (a,\,b)\to \mathbb{R}$; neka su $F_{1},\,F_{2}:\ (a,\,b)\to \mathbb{R}$ primitivne za $f$ na $(a,\,b)$. Tada $\exists C\in \mathbb{R}\ \ :\ \ \forall x\in(a,\,b)\quad F_{1}(x)-F_{2}(x)=C$.

>Dokaz: Neka je $G:\ (a,\,b)\to\mathbb{R}$ def. sa $G(x):=F_{1}(x)-F_{2}(x)$, tada $\forall x\in(a,\,b)\quad G'(x)=\big(F_{1}(x)-F_{2}(x)\big)'=f(x)-f(x)=0$
>Iz [[Teoreme o srednjoj vrednosti#^510c8c|posledice]] [[Teoreme o srednjoj vrednosti#^e52da5|Lagranževe teoreme]]: $G\equiv \mathrm{const}$

$\:$

### Definicija i svojstva neodređenog integrala

**Def**. Neka je $f:\ (a,\,b)\to\mathbb{R}$. Neodređeni integral funkcije $f$ na $(a,\,b)$ je skup svih primitivnih funkcija za $f$ na $(a,\,b)$.
$\begin{align}\int f(x)\,dx=\Big\{F\ \ \Big|\ \ F:\ (a,\,b)\to\mathbb{R};\quad\forall x \in (a,\,b)\quad F'(x)=f(x)\Big\}\end{align}$

Iz prethodne teoreme, neka je $F:\ (a,\,b)\to\mathbb{R}$ proizvoljna primitivna za $f:\ (a,\,b)\to\mathbb{R}$ na $(a,\,b)$. Tada:
$\begin{align}\int f(x)\,dx=\Big\{G\ \ \Big|\ \ G:\ (a,\,b)\to\mathbb{R};\quad \forall x\in (a,\,b)\quad G(x)=F(x) + C,\quad C\in\mathbb{R}\Big\}\end{align}$

Kraći zapis:
$\begin{align}\int f(x)\,dx= F(x) + C,\quad C\in\mathbb{R}\end{align}$
Napomena: u kraćem zapisu se ne piše interval, što predstavlja opasnost!

Integral se razmatra samo na **intervalu**: na uniji intervala svaki interval ima sopstvenu konstantu $C_{1},\,C_{2},\,\dots$

> Primer. Naći $\begin{align}\int\frac{1}{x}\,dx.\end{align}$
> $\begin{align}f(x)=\frac{1}{x}\end{align}\quad D_{f}=(-\infty,\,0)\cup(0,\,+\infty)$
> 
> I. $\begin{align}x\in(-\infty,\,0)\quad\int\frac{1}{x}\,dx=\ln (-x) + C_{1}, \ \ C_{1}\in\mathbb{R}\end{align}$
> II. $\begin{align}x\in(0,\,+\infty)\quad\int\frac{1}{x}\,dx=\ln x + C_{2}, \ \ C_{2}\in\mathbb{R}\end{align}$
> 
> Konačno: $\begin{align}\int\frac{1}{x}\,dx=\begin{cases}\ln|x|+C_{1},\quad C_{1}\in\mathbb{R},\ \ x\in(-\infty,\,0)\\\ln|x|+C_{2},\quad C_{2}\in\mathbb{R},\ \ x\in(0,\,+\infty)\end{cases}\end{align}$

$\:$
**Stav**. Neka su $f_{1},\,f_{2}:\ (a,\,b)\to\mathbb{R}$ funkcije koje imaju primitivne na $(a,\,b)$ i neka su $\lambda_{1},\,\lambda_{2}\in\mathbb{R}$. Tada
$\begin{align}\underbrace{\int \Big(\lambda_{1}\,f_{1}(x)+\lambda_{2}\,f_{2}(x)\Big) \, dx}_{L}=\underbrace{\lambda_{1}\int f_{1}(x) \, dx +\lambda_{2}\int f_{2}(x) \, dx}_{D}\end{align}$
> Dokaz: Neka je $F_{1}:\ (a,\,b)\to\mathbb{R}$ primitivna za $f_{1}$ na $(a,\,b)$; $F_{2}:\ (a,\,b)\to\mathbb{R}$ primitivna za $f_{2}$ na $(a,\,b)$
> 
> $\left.\begin{align}\forall x\in (a,\,b)\quad F'_{1}(x)=f_{1}(x)\\\forall x\in(a,\,b)\quad F'_{2}(x)=f_{2}(x)\end{align}\quad\right|\Rightarrow\quad\Big(\lambda_{1}\,F_{1}(x) +\lambda_{2}\,F_{2}(x)\Big)'=\lambda_{1}\,f_{1}(x)+\lambda_{2}\,f_{2}(x)$
> 
> $\Rightarrow \quad\lambda_{1}\,F_{1}(x) +\lambda_{2}\,F_{2}(x)=\Big(\lambda_{1}\,F_{1}+\lambda_{2}\,F_{2}\Big)(x)$ je primitivna za $\lambda_{1}\,f_{1}(x)+\lambda_{2}\,f_{2}(x)$ na $(a,\,b)$ $\quad$ $\Rightarrow\quad L=\lambda_{1}\,F_{1}(x) +\lambda_{2}\,F_{2}(x) + C,\quad C\in\mathbb{R}$
> 
> $D=\lambda_{1}\Big(F_{1}(x)+C_{1}\Big)+\lambda_{2}\Big(F_{2}(x)+C_{2}\Big)=\lambda_{1}\,F_{1}(x) +\lambda_{2}\,F_{2}(x) + \underbrace{\lambda_{1}\,C_{1}+\lambda_{2}\,C_{2}}_{C},\quad C_{1},\,C_{1}\in\mathbb{R}$


$\:$
### Tablica integrala
1. $\alpha\in\mathbb{R}\setminus\{ -1 \},\quad x\in(0,\,+\infty)$
   $\begin{align}\int x^{\alpha} \, dx=\frac{x^{\alpha+1}}{\alpha+1} + C,\quad C\in\mathbb{R}\end{align}$
   $\:$
2. $n\in\mathbb{N},\quad x\in\mathbb{R}$
   $\begin{align}\int x^{n} \, dx=\frac{x^{n+1}}{n+1} + C,\quad C\in\mathbb{R}\end{align}$
   $\:$

$*$ $\ \: \quad x\in \mathbb{R}$
$\ \ \ \, \quad$ $\begin{align}\int 1 \, dx =x+ C,\quad C\in\mathbb{R}\end{align}$
   $\:$
   
3. $n\in\mathbb{Z}\setminus(\mathbb{N}\cup\{ -1 \})=\{ 0,\,-2,\,-3,\,-4,\,\dots \},\quad x\in (-\infty,\,0)\cup(0,\,+\infty)$
   $\begin{align}\int x^{n} \, dx=\begin{cases}\frac{x^{n+1}}{n+1} + C_{1},\quad C_{1}\in\mathbb{R},\ \ x\in(-\infty,\,0)\\\frac{x^{n+1}}{n+1} + C_{2},\quad C_{2}\in\mathbb{R},\ \ x\in(0,\,+\infty)\end{cases}\end{align}$
   $\:$
4. $x\in (-\infty,\,0)\cup(0,\,+\infty)$
   $\begin{align}\int x^{-1} \, dx=\begin{cases}\ln|x|+C_{1},\quad C_{1}\in\mathbb{R},\ \ x\in(-\infty,\,0)\\\ln|x|+C_{2},\quad C_{2}\in\mathbb{R},\ \ x\in(0,\,+\infty)\end{cases}\end{align}$
   $\:$
5. $a > 0,\ \  a\ne 1, \quad x\in\mathbb{R}$
   $\begin{align}\int a^{x} \, dx =\frac{a^{x}}{\ln a}+ C,\quad C\in\mathbb{R}\end{align}$
   $\:$
6. $x\in\mathbb{R}$
   $\begin{align}\int \sin x \, dx =-\cos x + C,\quad C\in\mathbb{R}\end{align}$
   $\:$
7. $x\in\mathbb{R}$
   $\begin{align}\int \cos x \, dx =\cos x + C,\quad C\in\mathbb{R}\end{align}$
 $\:$
8. $\begin{align}x\in\mathbb{R}\setminus\Big\{ \frac{\pi}{2}+\pi k \ \Big|\ k\in\mathbb{Z} \Big\}=\bigcup_{k\,\in\,\mathbb{Z}}\Big(\frac{\pi}{2}+\pi k,\ \frac{3\pi}{2}+\pi k\Big)\end{align}$
   $\begin{align}\int \frac{1}{\cos^{2} x} \, dx =\mathrm{tg}\,x + C_{k},\quad C_{k}\in\mathbb{R},\ x\in\Big(\frac{\pi}{2}+\pi k,\ \frac{3\pi}{2}+\pi k\Big), \quad \forall k \in \mathbb{Z}\end{align}$
   $\:$
9. $\begin{align}x\in\mathbb{R}\setminus\Big\{ \pi k \ \Big|\ k\in\mathbb{Z} \Big\}=\bigcup_{k\,\in\,\mathbb{Z}}\Big(\pi k,\ \pi+\pi k\Big)\end{align}$
   $\begin{align}\int \frac{1}{\sin^{2} x} \, dx =-\mathrm{ctg}\,x + C_{k},\quad C_{k}\in\mathbb{R},\ x\in\Big(\pi k,\ \pi+\pi k\Big), \quad \forall k \in \mathbb{Z}\end{align}$
   $\:$
10. $x\in(-1,\,1)$
$\begin{align}\int \frac{1}{\sqrt[]{1-x^{2}}} \, dx =\arcsin x+C,\quad C\in\mathbb{R}\end{align}$
 $\:$
11. $x\in\mathbb{R}$
$\begin{align}\int \frac{1}{1+x^{2}} \, dx = \mathrm{arctg}\, x+C,\quad C\in\mathbb{R}\end{align}$

Integrali koje se izvode iz prethodnih koristeći smene:

12. $a>0,\quad x\in(-a,\,a)$
$\begin{align}\int \frac{1}{\sqrt[]{a^{2}-x^{2}}} \, dx =\arcsin \frac{x}{a}+C,\quad C\in\mathbb{R}\end{align}$
 $\:$
13. $a\in\mathbb{R}\setminus\{ 0 \},\quad x\in\, \begin{cases}\mathbb{R},& \text{ako } a>0\\(-\infty,\,-\sqrt[]{-a})\cup(\sqrt[]{-a},\,+\infty),&\text{ako } a<0\end{cases}$
$\begin{align}\int \frac{1}{\sqrt[]{x^{2}+ a}} \, dx =\ln\left|x+\sqrt[]{x^{2}+ a}\right|+C,\quad C\in\mathbb{R}\end{align}$
 $\:$
14. $a>0,\quad x\in\mathbb{R}$
$\begin{align}\int \frac{1}{x^{2}+a^{2}} \, dx = \frac{1}{a}\,\mathrm{arctg}\, \frac{x}{a}+C,\quad C\in\mathbb{R}\end{align}$
 $\:$
15. $a>0,\quad x\in\mathbb{R}\setminus\{ -a,\,a \}$
$\begin{align}\int \frac{1}{x^{2}-a^{2}} \, dx = \frac{1}{2a}\ln\left|\frac{x-a}{x+a}\right|+C,\quad C\in\mathbb{R}\end{align}$
(različito $C$ na svakom od tri intervala)

### [[Metode integracije (neodređeni integral)]]

### [[Integracija racionalnih funkcija]]
### [[Integracija racionalnih funkcija od sinusa i kosinusa]]
### [[Integracija nekih iracionalnih funkcija]]
  
