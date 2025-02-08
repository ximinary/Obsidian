#fax #math #a2 [deo poglavlja [[Nesvojstveni integral|"nesvojstveni integral"]]]

### Gama funkcija
>$\begin{align}1=\int_{0}^{+\infty} e^{-x} \, dx=\left(\begin{array}{l}u = e^{-x}&du=-e^{-x}dx\\dv = dx&v = x\end{array}\right) = \underbrace{xe^{-x}\Bigg|^{+\infty}_{0}}_{=0}+\int_{0}^{+\infty} xe^{-x} \, dx=\end{align}$
>
>$\begin{align}=\left(\begin{array}{l}u = e^{-x}&du=-e^{-x}dx\\dv = xdx&v = \frac{1}{2}x^{2}\end{array}\right) = \underbrace{\frac{1}{2}x^{2}e^{-x}\Bigg|^{+\infty}_{0}}_{=0}+\frac{1}{2}\int_{0}^{+\infty} x^{2}e^{-x} \, dx=\end{align}$
>
>$\begin{align}=\left(\begin{array}{l}u = e^{-x}&du=-e^{-x}dx\\dv = x^{2}dx&v = \frac{1}{3}x^{3}\end{array}\right) = \underbrace{\frac{1}{6}x^{3}e^{-x}\Bigg|^{+\infty}_{0}}_{=0}+\frac{1}{6}\int_{0}^{+\infty} x^{3}e^{-x} \, dx=\end{align}$
>
>$\begin{align}= \dots = \frac{1}{n!}\int_{0}^{+\infty} x^{n}e^{-x} \, dx\end{align}$
>
>$\begin{align}\Rightarrow\quad\int_{0}^{+\infty} x^{n}e^{-x} \, dx=n!,\quad\forall n\in\mathbb{N}_{0}\end{align}$

$\:$
**Stav**. Integral $\begin{align}\int_{0}^{+\infty} x^{\alpha-1}\,e^{-x} \, dx\end{align}$ konvergira za $\alpha>0$

$\:$
**Def**. **Gama funkcija** je funkcija $\Gamma:\ (0,\,+\infty)\to(0,\,+\infty)$ definisana sa $\begin{align}\Gamma(\alpha)=\int_{0}^{+\infty} x^{\alpha-1}\,e^{-x} \, dx\end{align}$

$\:$
**Stav** (svojstva gama funkcije).
- $\Gamma(\alpha+1)=\alpha\,\Gamma(\alpha),\quad\forall\alpha\in(0,\,+\infty)$
$\:$
- $\Gamma(n)=(n-1)!\,,\quad\forall n\in\mathbb{N}$
$\:$
- $\begin{align}\Gamma(\alpha)\cdot\Gamma(1-\alpha)=\frac{\pi}{\sin \pi\alpha},\quad\forall\alpha\in(0,\,1)\end{align}$
$\:$
Specijalno: $\begin{align}\Gamma\left( \frac{1}{2} \right)=\sqrt[]{\pi}\end{align}$

> Dokaz: 
> - $\begin{align}\Gamma(\alpha)=\int_{0}^{+\infty} x^{\alpha-1}\,e^{-x} \, dx=\left(\begin{array}{l}u = e^{-x}&du=-e^{-x}dx\\dv = x^{\alpha-1}dx&v = \frac{1}{\alpha}x^{\alpha}\end{array}\right)\end{align}$
> $\:$
> $\begin{align}= \underbrace{\frac{1}{\alpha}x^{\alpha}e^{-x}\Bigg|^{+\infty}_{0}}_{=0}+\frac{1}{\alpha}\int_{0}^{+\infty} x^{\alpha}e^{-x} \, dx=\frac{1}{\alpha}\Gamma(\alpha+1)\end{align}$
> $\:$
> - $\begin{align}\Gamma(1)=\int_{0}^{+\infty} e^{-x} \, dx=-e^{-x}\Bigg|_{0}^{+\infty}=1\end{align}$
>   $\:$
>   Primenom prethodnog tvrđenja:
>   $\Gamma(n)=(n-1)\cdot\Gamma(n-1)=\dots=(n-1)!\cdot\Gamma(1)= (n-1)!\,,\quad\forall n\in\mathbb{N}$ 

$\:$
**Stav**. $\Gamma\,\mathcal{D}^{\infty}\,(0,\,+\infty)$
### Beta funkcija
**Stav**. Integral $\begin{align}\int_{0}^{1} x^{\alpha-1}\,(1-x)^{\beta-1} \, dx\end{align}$ konvergira za $\alpha,\,\beta>0$

$\:$
**Def**. **Beta funkcija** je funkcija $\mathrm{B}:\ (0,\,+\infty)\times(0,\,+\infty)\to(0,\,+\infty)$ definisana sa $\begin{align}\mathrm{B}(\alpha,\,\beta)=\int_{0}^{1} x^{\alpha-1}\,(1-x)^{\beta-1} \, dx\end{align}$

$\:$
**Stav** (svojstva beta funkcije). $\forall\alpha,\,\beta\in(0,\,+\infty)$
- $\begin{align}\mathrm{B}(\alpha,\,\beta)=\mathrm{B}(\beta,\,\alpha)\end{align}$
$\:$
- $\begin{align}\mathrm{B}(\alpha,\,\beta)=\int_{0}^{+\infty} \frac{x^{\alpha-1}}{(1+x)^{\alpha+\beta}} \, dx\end{align}$
$\:$
-  $\begin{align}\mathrm{B}(\alpha,\,\beta)=\frac{\Gamma(\alpha)\cdot\Gamma(\beta)}{\Gamma(\alpha+\beta)}\end{align}$