#fax #math #a1 [deo poglavlja [[Limes funkcije|"limes funkcije"]]]  
$\:$

### Vertikalna asimptota

**Def**. $x_{0}\in D'_{f}\setminus D_{f}$. Prava $x=x_{0}$ je **vertikalna asimptota** ako
$\lim\limits_{ x \to x_{0}^{-} }f(x)=\pm\infty\ \:$ ili $\:\ \lim\limits_{ x \to x_{0}^{+} }f(x)=\pm\infty$

### Kosa asimptota
**Def**. $\pm\infty\in D_{f}'$. Prava $y = k\,x+n$ je **kosa asimptota** fje $f$, kod $x\to\pm\infty$, $\:$ ako $\boxed{f(x)=k\,x+n+o(1),\quad x\to\pm\infty}$

- Asimptota sa $k=0$ zove se **horizontalna**.

#### Direktno tražimo $k$ i $n$
Tražimo $k$:
Def.$\ \ \Leftrightarrow\ \ \begin{align}\frac{f(x)}{x}=k+\frac{n}{x}+o\Big(\frac{1}{x}\Big),\quad x\to\pm\infty\end{align} \ \ \Leftrightarrow$
$\Leftrightarrow\ \ \begin{align}k = \frac{f(x)}{x}-\frac{n}{x}+o\Big(\frac{1}{x}\Big),\quad x\to\pm\infty\end{align} \ \ \Rightarrow$
$\Rightarrow\ \ \begin{align}k=\lim\limits_{ x \to \pm\infty}\bigg(\frac{f(x)}{x}-\frac{n}{x}+o\Big(\frac{1}{x}\Big)\bigg)=\lim\limits_{ x \to \pm\infty }\frac{f(x)}{x}\end{align}$

Ako $\begin{align}\nexists\lim\limits_{ x \to \pm\infty }\frac{f(x)}{x}\end{align}$ onda $\nexists$ asimptota.
$\:$

Ako $\exists k$ tražimo $n$:
Def. $\ \ \Leftrightarrow\ \ n=f(x)-k\,x+o(1),\quad x\to\pm\infty\ \ \ \Leftrightarrow$
$\Rightarrow\ \ n=\lim\limits_{ x \to \pm\infty}\big(f(x)-k\,x+o(1)\big)=\lim\limits_{ x \to \pm\infty}\big(f(x)-k\,x\big)$

Ako $\nexists\lim\limits_{ x \to \pm\infty}\big(f(x)-k\,x\big)$ onda $\nexists$ asimptota.

#### Tražimo $k$ i $n$ pomoću [[Tejlorov polinom|Tejlorovog polinoma]]

Dobijamo: $\begin{align}f(x)=k\,x+n+\frac{m}{x},\quad x\to\pm\infty\end{align}$
Odakle osim formule asimptote imamo i informaciju o prolazu fje iznad/ispod asimptote:

$\begin{align}f(x)-(k\,x+n)= \frac{m}{x} \underbrace{\big(1+o(1)\big)}_{>0},\quad x\to\pm\infty\end{align}$

Odakle:
$\begin{align}\bigg(f(x)>k\,x+n\quad \Leftrightarrow\quad \frac{m}{x}>0\bigg),\quad x\to\pm\infty\end{align}$
$\begin{align}\bigg(f(x)<k\,x+n\quad \Leftrightarrow\quad \frac{m}{x}<0\bigg),\quad x\to\pm\infty\end{align}$