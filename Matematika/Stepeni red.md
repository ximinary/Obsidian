#fax #math #a2 [deo poglavlja [[Funkcionalni red|"funkcionalni red"]]]
$\:$

**Def**. Neka je $\big(c_{n}\big)_{n\in\mathbb{N}_{0}}$ [[Niz brojeva|niz brojeva]] i $x_{0}\in\mathbb{R}$. Tada se funkcionalni red $\begin{align}\sum\limits_{n=0}^{\infty} c_{n}(x-x_{0})^{n} \end{align}$ naziva **stepeni red**.

Za $x_{0}=0$ stepeni red ima oblik $\begin{align}\sum\limits_{n=0}^{\infty}c_{n}\,x^{n} \end{align}$

Jasno je, $\begin{align}\sum\limits_{n=0}^{\infty}c_{n}\,x^{n} \end{align}$ ravnomerno/TPT konvergira ka $f(x)$ na $[a,\,b]$ akko  $\begin{align}\sum\limits_{n=0}^{\infty}c_{n}(x-x_{0})^{n} \end{align}$ ravnomerno/TPT konvergira ka $f(x-x_{0})$ na $[a+x_{0},\,b+x_{0}]$.

$\:$
**Stav**. Ako stepeni red $\begin{align}\sum\limits_{n=0}^{\infty}c_{n} \,x^{n} \end{align}$
- konvergira za $x=x_{1}$ onda on apsolutno konvergira za svako $x$ takvo da $|x|<|x_{1}|$ ^8fd158
- divergira za $x=x_{2}$ onda on divergira za svako $x$ takvo da $|x|>|x_{2}|$

> Dokaz:
>
> $\begin{align}\sum\limits_{n=0}^{\infty} c_{n}\,x_{1}^{n}\ \ \text{konvergira}\quad\Rightarrow\quad\lim\limits_{ n \to \infty } c_{n}\,x_{1}^{n}=0\quad\Rightarrow\quad\exists M>0\quad\forall n\in\mathbb{N} \quad |c_{n}\,x_{1}^{n}|<M\quad\end{align}$
>
> Važi: 
> $\begin{align}|c_{n}\,x^{n}|=|c_{n}\,x_{1}^{n}|\cdot\bigg|\frac{x}{x_{1}}\bigg|^{n}\leqslant M\,q^{n},\quad\quad\bigg|\frac{x}{x_{1}}\bigg|=q<1\end{align}$
> I jer $\begin{align}\sum\limits_{n=0}^{\infty}M\,q^{n}\ \ \end{align}$ [[Konvergencija nekih brojevnih redova#^20d439|konvergira]] za $0<q<1$ iz [[Kriterijumi konvergencije brojevnih redova#^4d14b2|teoreme]] sledi prvo tvrđenje.
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
**Teorema**. Neka $\big(c_{n}\big)_{n\in\mathbb{N}_{0}}$ niz brojeva takav da važi jedno od tvrđenja:
- $\begin{align}\lim\limits_{ n \to \infty }\frac{|c_{n+1}|}{|c_{n}|}=A\in[0,\,+\infty]\end{align}$
- $\lim\limits_{ n \to \infty }\sqrt[n]{|c_{n}|}=A\in[0,\,+\infty]$

Tada je poluprečnik konvergencije reda $\begin{align}\sum\limits_{n=0}^{\infty}c_{n}\,x^{n} \end{align}$ jednak $\begin{align}R=\frac{1}{A}\in[0,\,+\infty]\end{align}$
> Dokaz:
> Razmatramo konvergenciju reda $\begin{align}\sum\limits_{n=0}^{\infty}c_{n}\,x^{n}\end{align}$ za $x>0$
> - $\begin{align}\lim\limits_{ n \to \infty }\frac{|c_{n+1}\,x^{n+1}|}{|c_{n}\,x^{n}|}=A\,x\quad\quad\lim\limits_{ n \to \infty }\frac{|c_{n+1}|\,x^{n+1}}{|c_{n}|\,x^{n}}=A\,x\end{align}$
>   $\:$
> iz [[Kriterijumi konvergencije brojevnih redova#^cf63a2|Dalamberova kriterijuma]] red apsolutno konvergira za $A\,x<1$ i divergira za $A\,x>1$
> $\:$
> - $\begin{align}\lim\limits_{ n \to \infty }\sqrt[n]{|c_{n}\,x^{n}|}=A\,x\quad\quad\lim\limits_{ n \to \infty }\sqrt[n]{|c_{n}|\,x^{n}}=A\,x\end{align}$
>   $\:$
> iz [[Kriterijumi konvergencije brojevnih redova#^d13f64|Košijevog korenog kriterijuma]] red apsolutno konvergira za $A\,x<1$ i divergira za $A\,x>1$
> 
> Odakle imamo, 
> ako $A=+\infty$, red divergira za $\forall x\in\mathbb{R}\setminus\{0\}$, tj. $\begin{align}R=0=\frac{1}{A}\end{align}$
> ako $A=0$, red konvergira za $\forall x\in\mathbb{R}$, tj. $\begin{align}R=+\infty=\frac{1}{A}\end{align}$ 
> ako $A\in(0,\,+\infty)$, red konvergira za $\begin{align}0<x<\frac{1}{A}\end{align}$ i divergira za $\begin{align}x > \frac{1}{A}\end{align}$, tj $\begin{align}R=\frac{1}{A}\end{align}$

$\:$
### Svojstva stepenih redova

**Stav**. Za $0<r<R$ red $\ \:$ $\begin{align}\sum\limits_{n=1}^{\infty}c_{n}\,x^{n}\ \ \end{align}$ ravnomerno konvergira na $[-r,\,r]$.
> Dokaz: kako $\forall n\in\mathbb{N}_{0}\quad\forall x\in[-r,\,r]\quad|c_{n}\,x^{n}|\leqslant|c_{n}\,r^{n}|$ i kako brojevni red $\begin{align}\sum\limits_{n=0}^{\infty} |c_{n}\,r^{n}| \end{align}$ konvergira ([[Stepeni red#^8fd158|jer]] $r<R$) iz [[Funkcionalni red#^b72d33|Vajerštrasova kriterijuma]] sledi tvrđenje.

**Posledica**. Neka je $\begin{align}\sum\limits_{n=0}^{\infty}c_{n}\,x^{n} \end{align}$ stepeni red sa poluprečnikom konvergencije $R>0$. Tada za svako $x\in(-R,\,R)$ važi
- $\begin{align}\bigg(\sum\limits_{n=0}^{\infty}c_{n}\,x^{n} \bigg)\,\mathcal{C}\, x\end{align}$
- $\begin{align}\int_{0}^{x} \bigg(\sum\limits_{n=0}^{\infty}c_{n}\,t^{n}\bigg)  \, dt = \sum\limits_{n=0}^{\infty}\bigg(\int_{0}^{x} c_{n}\,t^{n} \, dt\bigg)=\sum\limits_{n=0}^{\infty}\frac{c_{n}}{n+1}x^{n+1}=\sum\limits_{n=1}^{\infty}\frac{c_{n-1}}{n}x^{n}\quad\quad(1)\end{align}$
- $\begin{align}\bigg(\sum\limits_{n=0}^{\infty}c_{n}\,x^{n}\bigg)'=\sum\limits_{n=0}^{\infty}(c_{n}\,x^{n})'=\sum\limits_{n=1}^{\infty}n\,c_{n}\,x^{n-1}=\sum\limits_{n=0}^{\infty}(n+1)\,c_{n+1}\,x^{n}\quad\quad\quad\quad\quad\ \ (2)\end{align}$

Štaviše, poluprečnici redova $(1)$ i $(2)$ su jednaki $R$
> Dokaz: 
> $\forall x\in(-R,\,R)\quad\exists r\in R\ \  :\ \ |x|<r<R$. Tada polazni red (kao i red $(2)$) ravnomerno konvergira na $[-r,\,r]$. Odakle, pomoću stavova o svojstvima ravnomerno konvergentnih funkcionalnih redova ([[Svojstva ravnomerno konvergentnih funkcionalnih redova#^aa2a53|0]], [[Svojstva ravnomerno konvergentnih funkcionalnih redova#^205ccf|1]], [[Svojstva ravnomerno konvergentnih funkcionalnih redova#^717181|2]]) dobijamo tvrđenja.
> 
> Poluprečnici:
> $(1)$ Pod pretpostavkom da važi $\begin{align}\lim\limits_{ n \to \infty }\sqrt[n]{|c_{n}|}=\frac{1}{R}\end{align}$.
> Tada $\begin{align}\lim\limits_{ n \to \infty }\sqrt[n]{\frac{|c_{n-1}|}{n}}=\frac{1}{R}\end{align}$
> 
> $(2)$ Pod pretpostavkom da važi $\begin{align}\lim\limits_{ n \to \infty }\frac{|c_{n+1}|}{|c_{n}|}=\frac{1}{R}\end{align}$.
> Tada $\begin{align}\lim\limits_{ n \to \infty }\frac{(n+2)c_{n+2}}{(n+1)c_{n+1}}=\frac{1}{R}\end{align}$


$\:$
**Teorema** (Abelova). Ako je $R < +\infty$ i ako red $\begin{align}\sum\limits_{n=0}^{\infty}c_{n}\,R^{n} \end{align}$ konvergira, onda red $\begin{align}\sum\limits_{n=0}^{\infty}c_{n}\,x^{n} \end{align}$ ravnomerno konvergira na $[0, R]$ i važi $\begin{align}\lim\limits_{ x \to R^{-} }\sum\limits_{n=0}^{\infty}c_{n}\,x^{n}=\sum\limits_{n=0}^{\infty}c_{n}\,R^{n}\end{align}$

$\:$
**Stav**. Neka je $\begin{align}\sum\limits_{n=0}^{\infty}c_{n}\,x^{n} \end{align}$ stepeni red sa poluprečnikom konvergencije $R$ i neka je $s:\ (-R,\,R)\to\mathbb{R}$  definisana sa $\begin{align}s(x)=\sum\limits_{n=0}^{\infty}c_{n}\,x^{n} \end{align}$. Tada $s\,\mathcal{C}^{\infty}\,(-R,\,R)$.

>$\forall n\in\mathbb{N}\quad s^{(n)}(0)=n!\,c_{n}$
odakle, $\begin{align}s(x)=\sum\limits_{n=0}^{\infty}\frac{s^{(n)}(0)}{n!}x^{n} \end{align}$

$\:$
### Tejlorov red
Napomena: [[Tejlorov polinom]]

**Def**. Neka je $f:\ (a,\,b)\to\mathbb{R}$ takva da $f\,\mathcal{C}^{\infty}\,(a,\,b)$ i neka je $x_{0}\in(a,\,b)$. Tada stepeni red $\boxed{\begin{align}\sum\limits_{n=0}^{\infty}\frac{f^{(n)}(x_{0})}{n!}(x-x_{0})^{n} \end{align}}$ je **Tejlorov red** funkcije $f$ u tački $x_{0}$. (**Maklorenov red** funkcije $f$ ako $x_{0}=0$).

> Napomena: Tejlorov red može da konvergira kao i divergira na nekim delovima $(a,\,b)$. Iako konvergira na nekom intervalu, ne mora da konvergira ka $f$

$\:$
**Stav**. Neka je $f:\ (-R,\,R)\to\mathbb{R}$ takva da $f\,\mathcal{C}^{\infty}\,(-R,\,R)$. Tada
$\begin{align}\forall x\in(-R,\,R)\quad f(x)=\sum\limits_{n=0}^{\infty}\frac{f^{(n)}(0)}{n!}x^{n} \quad\Leftrightarrow\quad\forall x\in(-R,\,R)\quad\lim\limits_{ n \to \infty }R_{n}(x,\,0;\,f)=0\end{align}$, 
gde je $R_{n}(x,\,0;\,f)$ [[Tejlorov polinom#Ostatak Tejlorovog polinoma|ostatak Tejlorovog (Maklorenovog) polinoma]]

> Dokaz: levi deo ekvivalencije prepišemo kao
> $\forall x\in(-R,\,R)\quad \lim\limits_{ n \to \infty }P_{n}(x,\,0;\,f)=f(x)$,
> gde je $P_{n}(x,\,0;\,f)$ [[Tejlorov polinom|Maklorenov polinom]] fje $f$, odnosno parcijalna suma Maklorenovog reda.
> 
> Tada ekvivalencija sledi iz jednačine $\forall n\in\mathbb{N}\quad\forall x\in(-R,\,R)\quad f(x)=P_{n}(x,\,0;\,f)+R_{n}(x,\,0;\,f)$

$\:$
**Stav**. Neka je $f:\ (-R,\,R)\to\mathbb{R}$ takva da $f\,\mathcal{C}^{\infty}\,(-R,\,R)$. Tada ako $\forall r\in(0,\,R)\quad\exists M>0\quad\forall n\in\mathbb{N}_{0}\quad\forall x\in[-r,\,r]\quad|f^{(n)}(x)|\leqslant M$ 
onda $\forall x\in(-R,\,R)\quad\lim\limits_{ n \to \infty }R_{n}(x,\,0;\,f)=0$
> Dokaz:
> [[Tejlorov polinom#^ddcb73|Lagranžev oblik ostatka]] Maklorenovog polinoma:
> $\begin{align}R_{n}(x,\,0;\,f)=\frac{f^{(n+1)}(\xi)\cdot x^{n+1}}{(n+1)!},\quad\quad\end{align}$ gde je $\xi$ između $0$ i $x$.
>
> Tada, za svako $x\in(-R,\,R)$ postoji $r\in(|x|,\,R)$ za takvo $r$ is pretpostavke $\:\exists M>0\:$ tako da $\:\forall n\in\mathbb{N}_{0}\:$ važi $\:|f^{(n)}(\xi)|\leqslant M\:$ (jer $|\xi|<|x|<r$)
> 
> Imamo,
> $\begin{align}\forall x\in(-R,\,R)\quad\forall n\in\mathbb{N}_{0}\quad&\big|R_{n}(x,\,0;\,f)\big|=\Bigg|\frac{f^{(n+1)}(\xi)\cdot x^{n+1}}{(n+1)!}\Bigg|\leqslant\frac{M\,r^{n+1}}{(n+1)!}\\&-\frac{M\,r^{n+1}}{(n+1)!}\leqslant R_{n}(x,\,0;\,f)\leqslant \frac{M\,r^{n+1}}{(n+1)!}\end{align}$
> 
> Kako $\begin{align}\lim\limits_{ n \to \infty }\frac{M\,r^{n+1}}{(n+1)!}=0\end{align}$ iz [[Limes funkcije#^dd4e68|teoreme o dva policajaca]] važi $\lim\limits_{ n \to \infty }R_{n}(x,\,0;\,f)=0$.

$\:$
#### Maklorenov red osnovnih funkcija:
- $\begin{align}e^{x}=\sum\limits_{n=0}^{\infty}\frac{x^{n}}{n!},\quad\quad x\in\mathbb{R}\end{align}$
- $\begin{align}\ln(1+x)=\sum\limits_{n=1}^{\infty}(-1)^{n-1}\frac{x^{n}}{n},\quad\quad x\in(-1,\,1]\end{align}$
- $\begin{align}(1+x)^{\alpha}=\sum\limits_{n=0}^{\infty}\binom{\alpha}{n}x^{n},\quad\quad x\in\begin{cases}(-1,\,1),&\alpha\leqslant-1\\(-1,\,1],&-1<\alpha\leqslant0\\ [-1,\,1],&\alpha>0\end{cases}\end{align}$
- $\begin{align}\sin x =\sum\limits_{n=0}^{\infty}(-1)^{n}\frac{x^{2n+1}}{(2n+1)!},\quad\quad x\in\mathbb{R}\end{align}$
- $\begin{align}\cos x =\sum\limits_{n=0}^{\infty}(-1)^{n}\frac{x^{2n}}{(2n)!},\quad\quad x\in\mathbb{R}\end{align}$

> Dokaz: Maklorenove redove navedenih fja dobijamo iz [[analiza1_2_Tejlor.png|Maklorenovih polinoma fja]]. Razmotrimo tačka po tačku konvergenciju redova:
> - $f(x)=e^{x}, \quad\quad x\in(-\infty,\,+\infty)$
>   $\forall r\in(0,\,+\infty)\quad\forall n \in\mathbb{N}\quad \forall x \in[-r,\,r]\quad|f^{(n)}(x)|=e^{x}\leqslant e^{r}=:M$
>   iz prethodna dva stava red TPT konvergira ka $f$ na $\mathbb{R}$
> $\:$
> - za $\sin x$ i $\cos x$ slično, pri tome $M=1$
>   $\:$
> -  $f(x)=(1+x)^{\alpha}, \quad\quad x\in(-\infty,\,+\infty)$
>   Nađemo poluprečnik konvergencije reda (za $\alpha<0$):
>   $\begin{align}\frac{1}{R}=\lim\limits_{ n \to \infty }\bigg|\frac{a_{n+1}}{a_{n}}\bigg|=\lim\limits_{ n \to \infty }\Bigg|\frac{\binom{\alpha}{n+1}}{\binom{\alpha}{n}}\Bigg|=\lim\limits_{ n \to \infty }\bigg|\frac{\alpha-n}{n+1}\bigg|=1\quad\Rightarrow\quad R=1\end{align}$
>   Odakle red konvergira za $x\in(-1,\,1)$
> $\:$
> - $f(x)=\ln(1+x)$
>   $\begin{align}f'(x)=\frac{1}{1+x}\quad\Rightarrow\quad f(x)&=\underbrace{f(0)}_{=0}+\int_{0}^{x} \frac{1}{1+t} \, dt=\int_{0}^{x} \bigg(\sum\limits_{n=0}^{\infty}\underbrace{\binom{-1}{n}}_{=(-1)^{n}}t^{n} \bigg)\, dt\\&=\sum\limits_{n=0}^{\infty}(-1)^{n}\frac{t^{n+1}}{n+1}=\sum\limits_{n=1}^{\infty}(-1)^{n-1}\frac{t^{n}}{n}\end{align}$
>   sa istim poluprečnikom $R=1$.
>  za $x=1$ konvergira po Lajbnicovu kriterijumu,
>  za $x=-1$ imamo $\begin{align}-\sum\limits_{n=0}^{\infty} \frac{1}{n}\end{align}$ divergira
>  