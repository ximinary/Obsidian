#fax #math #a2 [deo poglavlja [[Funkcionalni red|"funkcionalni red"]]]
$\:$

**Def**. Neka je $\big(c_{n}\big)_{n\in\mathbb{N}_{0}}$ [[Red brojeva|red brojeva]] i $x_{0}\in\mathbb{R}$. Tada se funkcionalni red $\begin{align}\sum\limits_{n=0}^{\infty} c_{n}(x-x_{0})^{n} \end{align}$ naziva **stepeni red**.

Za $x_{0}=0$ stepeni red ima oblik $\begin{align}\sum\limits_{n=0}^{\infty}c_{n}\,x^{n} \end{align}$

Jasno je, $\begin{align}\sum\limits_{n=0}^{\infty}c_{n}\,x^{n} \end{align}$ ravnomerno/TPT konvergira ka $f(x)$ na $[a,\,b]$ akko  $\begin{align}\sum\limits_{n=0}^{\infty}c_{n}(x-x_{0})^{n} \end{align}$ ravnomerno/TPT konvergira ka $f(x-x_{0})$ na $[a+x_{0},\,b+x_{0}]$.

$\:$
**Stav**. Ako stepeni red $\begin{align}\sum\limits_{n=0}^{\infty}c_{n} \,x^{n} \end{align}$
- konvergira za $x=x_{1}$ onda on apsolutno konvergira za svako $x$ takvo da $|x|<|x_{1}|$
- divergira za $x=x_{2}$ onda on divergira za svako $x$ takvo da $|x|>|x_{2}|$

> Dokaz:
>
> $\begin{align}\sum\limits_{n=0}^{\infty} c_{n}\,x_{1}^{n}\ \ \text{konvergira}\quad\Rightarrow\quad\lim\limits_{ n \to \infty } c_{n}\,x_{1}^{n}=0\quad\Rightarrow\quad\exists M>0\quad\forall n\in\mathbb{N} \quad |c_{n}\,x_{1}^{n}|<M\quad\end{align}$
>
> Važi: 
> $\begin{align}|c_{n}\,x^{n}|=|c_{n}\,x_{1}^{n}|\cdot\bigg|\frac{x}{x_{1}}\bigg|^{n}\leqslant M\,q^{n},\quad\quad\bigg|\frac{x}{x_{1}}\bigg|=q<1\end{align}$
> I jer $\begin{align}\sum\limits_{n=0}^{\infty}M\,q^{n}\ \ \end{align}$ [[Konvergencija nekih redova#^20d439|konvergira]] za $0<q<1$ iz [[Kriterijumi konvergencije redova brojeva#^4d14b2|teoreme]] sledi prvo tvrđenje.
> ___
> $\begin{align}\sum\limits_{n=0}^{\infty} c_{n}\,x_{2}^{n}\ \ \text{divergira}\end{align}$.
> Pretpostavimo suprotno, tj. postoji $\widehat{x}$ za koje važi $|\widehat{x}|>|x_{2}|$ i $\begin{align}\sum\limits_{n=0}^{\infty} c_{n}\,\widehat{x}^{n}\ \ \text{konvergira} \end{align}$. Tada iz prvog tvrđenja za svako $x$ za koje važi $|x|<|\widehat{x}|$ (što važi i za $x= x_{2}$) red $\begin{align}\sum\limits_{n=0}^{\infty} c_{n}\,x^{n}\ \ \text{konvergira}\end{align}$. Kontradikcija.

$\:$
**Def**. Neka je $X$ skup vrednosti promenljive $x$ za koje red $\begin{align}\sum\limits_{n=0}^{\infty} c_{n}\,x^{n}\ \  \end{align}$ konvergira.
$\ \:$ ako $X$ nije ograničen (tj. $X=\mathbb{R}$) onda $R:=+\infty$
$\ \:$ inače je $X$ ograničen i $\exists \sup\limits_{x\in X}|x|=:R$
Tada je $R\in[0,\,+\infty]$ **poluprečnik konvergencije** stepenog reda $\begin{align}\sum\limits_{n=0}^{\infty}c_{n}\,x^{n}\end{align}$.

$\:$
**Stav**. Stepeni red $\begin{align}\sum\limits_{n=0}^{\infty}c_{n}\,x^{n}\end{align}$ apsolutno konvergira na $(-R,\,R)$ i divergira na $(-\infty,\,-R)\cup(R,\,+\infty)$.
> Dokaz: tvrđenje sledi iz definicije poluprečnika konvergencije i prethodne teoreme.

$\:$
**Teorema**. Neka $\big(c_{n}\big)_{n\in\mathbb{N}_{0}}$ niz pozitivnih brojeva takav da važi jedno od tvrđenja:
- $\begin{align}\lim\limits_{ n \to \infty }\frac{c_{n+1}}{c_{n}}=A\in[0,\,+\infty]\end{align}$
- $\lim\limits_{ n \to \infty }\sqrt[n]{c_{n}}=A\in[0,\,+\infty]$

Tada je poluprečnik konvergencije reda $\begin{align}\sum\limits_{n=0}^{\infty}c_{n}\,x^{n} \end{align}$ jednak $\begin{align}R=\frac{1}{A}\in[0,\,+\infty]\end{align}$
> Dokaz:
> 