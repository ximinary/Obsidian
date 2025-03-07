#fax #math #a2 [deo poglavlja [[Beskonačnodimenzioni Euklidski prostor. Niz i red vektora|"beskonačnodimenzioni Euklidski prostor"]]]
$\:$

**Def**. $\mathcal{C}_{0}[-\pi,\,\pi]$ je prostor deo po deo neprekidnih funkcija $f:\ [-\pi,\,\pi]\to\mathbb{R}$, takvih da 
- $\begin{align}\forall x\in(-\pi,\,\pi)\quad f(x)=\frac{f(x^{+})+f(x^{-})}{2}\end{align}$
- $\begin{align}f(-\pi)=f(\pi)=\frac{f(-\pi^{+})+f(\pi^{-})}{2}\end{align}$

$\mathcal{C}_{0}[-\pi,\,\pi]$ je [[Vektorski prostor|vektorski prostor]] uz operacije:
- $(f+g)(x)=f(x)+g(x),\quad f,\,g,\,f+g\in\mathcal{C}_{0}[-\pi,\,\pi]$
- $(\lambda\cdot f)(x)=\lambda\cdot f(x),\quad f,\,\lambda\cdot f\in\mathcal{C}_{0}[-\pi,\,\pi],\quad\lambda\in\mathbb{R}$

Operacija $f\bullet g$ definisana sa $\begin{align}f\bullet g=\int_{-\pi}^{\pi} f(x)\,g(x) \, dx \end{align}$ je [[Unitarni prostor. Euklidski prostor|skalarni proizvod]] na $\mathcal{C}_{0}[-\pi,\,\pi]$
> Dokaz: SP1-SP4 i leva implikacija SP5 se jednostavno dokazuju. Treba samo pokazati $f\bullet f=0\quad\Rightarrow\quad f=0$.
> $f$ je deo po deo neprekidna, što znači da postoji podela $-\pi=x_{0}<x_{1}<\dots<x_{n}=\pi$ takva da $\forall i\in \overline{1,\,n}\quad f\,\mathcal{C}\,[x_{i-1},\,x_{i}]$
> $\begin{align}0=\int_{-\pi}^{\pi} \big(f(x)\big)^{2} \, dx=\int_{x_{0}}^{x_{1}} \big(f(x)\big)^{2} \, dx+\int_{x_{1}}^{x_{2}} \big(f(x)\big)^{2} \, dx+\dots+\int_{x_{n-1}}^{x_{n}} \big(f(x)\big)^{2} \, dx\end{align}$
> Jer su svi sabirci nenegativni imamo $\begin{align}\forall i\in\overline{1,\,n}\quad\int_{x_{i-1}}^{x_{i}} \big(f(x)\big)^{2} \, dx=0\end{align}$.
> iz neprekidnosti i nenegativnosti $f$ na $[x_{i-1},\,x_{i}]$ imamo $x\in(-\pi,\,\pi)\setminus\{x_{1},\,x_{2},\,\dots,\,x_{n-1}\}\quad f(x)=0$.
> A iz $\forall i\in\overline{1,\,n}\quad f(x_{i-1}\!^{+})=f(x_{i}\!^{-})=0$ pomoću definicije imamo i $\begin{align}\forall i\in\overline{1,\,n-1}\quad f(x_{i})=\frac{f(x_{i}\!^{-})+f(x_{i}\!^{+})}{2}=0\end{align}$
> $\begin{align}f(-\pi)=f(\pi)=\frac{f(x_{0}\!^{+})+f(x_{n}\!^{-})}{2}=0\end{align}$
> tj $f=0$

$\:$
Imamo da je $\mathcal{C}[-\pi,\,\pi]$ [[Unitarni prostor. Euklidski prostor#^e3a11f|pred-Hilbertov prostor]]. 

**Def**. Ako [[Niz funkcija|niz funkcija]] $f_{n}\in\mathcal{C}[-\pi,\,\pi]$ (kao niz vektora) [[Beskonačnodimenzioni Euklidski prostor. Niz i red vektora#^890b7c|konvergira]] ka funkciji $f\in\mathcal{C}[-\pi,\,\pi]$ onda kažemo da niz funkcija $f_{n}$ **konvergira** ka funkciji $f$ **u srednjem**. ^e4918f

$\:$
**Stav**. Niz vektora (funkcija)
$$(e_{n})=\bigg(\frac{1}{\sqrt[]{2\pi}},\ \frac{\cos x}{\sqrt[]{\pi}},\ \frac{\sin x}{\sqrt[]{\pi}},\ \frac{\cos 2x}{\sqrt[]{\pi}},\ \frac{\sin 2x}{\sqrt[]{\pi}},\ \frac{\cos 3x}{\sqrt[]{\pi}},\ \frac{\sin 3x}{\sqrt[]{\pi}},\dots\bigg)$$
jeste [[Beskonačnodimenzioni Euklidski prostor. Niz i red vektora#^e6bffc|ortonormirani niz vektora]] u prostoru $\mathcal{C}_{0}[-\pi,\,\pi]$.

[[Beskonačnodimenzioni Euklidski prostor. Niz i red vektora#^e69126|Furijeov red]] vektora $f\in\mathcal{C}_{0}[-\pi,\,\pi]$ u odnosu na $e_{n}$ je $\begin{align}\sum\limits_{n=1}^{\infty}(f\bullet e_{n})\,e_{n}=\frac{\alpha_{0}}{\sqrt[]{2\pi}}+\sum\limits_{n=1}^{\infty}\bigg(\frac{\alpha_{n}\,\cos nx}{\sqrt[]{\pi}}+\frac{\beta_{n}\,\sin nx}{\sqrt[]{\pi}}\bigg),\end{align}$ gde su ^558e23
- $\begin{align}\alpha_{0}=f\bullet\frac{1}{\sqrt[]{2\pi}}=\int_{-\pi}^{\pi} f(x)\frac{1}{\sqrt[]{2\pi}} \, dx=\frac{1}{\sqrt[]{2\pi}}\int_{-\pi}^{\pi} f(x) \, dx\end{align}$
  $\:$
- $\begin{align}\alpha_{n}=f\bullet\frac{\cos nx}{\sqrt[]{\pi}}=\frac{1}{\sqrt[]{\pi}}\int_{-\pi}^{\pi} f(x)\cos nx \, dx,\quad\forall n\in\mathbb{N}\end{align}$
  $\:$
- $\begin{align}\beta{n}=f\bullet\frac{\sin nx}{\sqrt[]{\pi}}=\frac{1}{\sqrt[]{\pi}}\int_{-\pi}^{\pi} f(x)\sin nx \, dx,\quad\forall n\in\mathbb{N}\end{align}$

### [[Furijeov red u prostoru C₀]]