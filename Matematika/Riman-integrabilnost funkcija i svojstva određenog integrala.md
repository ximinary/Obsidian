#fax #math #a2 [deo poglavlja [[Određeni integral|"određeni integral"]]]

### Riman-integrabilnost nekih klasa funkcija

**Teorema** (Kriterijum Riman-integrabilnosti). $f:\ [a,\,b]\to\mathbb{R}$ ograničena fja. Tada
$f\,\mathcal{R}\,[a,\,b]\quad\Leftrightarrow\quad\forall\varepsilon>0\quad\exists\mathcal{P}\in\mathcal{P}[a,\,b]\ \ :\ \ S(f,\,\mathcal{P})-s(f,\,\mathcal{P})<\varepsilon$ ^fdf6e4
> Dokaz: $\boxed{\Rightarrow}$ Neka je $\begin{align}I=\int_{a}^{b} f(x) \, dx \end{align}$
> Iz definicija supremuma i infinuma:
> - $\forall\varepsilon>0\quad\begin{align}\exists\mathcal{P}'\in\mathcal{P}[a,\,b]\ \ :\ \ S(f,\,\mathcal{P}')<I + \frac{\varepsilon}{2}\end{align}$
> - $\forall\varepsilon>0\quad\begin{align}\exists\mathcal{P}''\in\mathcal{P}[a,\,b]\ \ :\ \ s(f,\,\mathcal{P}'')>I - \frac{\varepsilon}{2}\end{align}$
> 
> Neka je $\mathcal{P}$ superpozicija $\mathcal{P}'$ i $\mathcal{P}''$, tada
> - $\begin{align}S(f,\,\mathcal{P})\leqslant S(f,\,\mathcal{P}')<I + \frac{\varepsilon}{2}\quad\Rightarrow\quad S(f,\,\mathcal{P})<I + \frac{\varepsilon}{2}\end{align}$
> - $\begin{align}I - \frac{\varepsilon}{2}< s(f,\,\mathcal{P}'') \leqslant s(f,\,\mathcal{P})\quad\Rightarrow\quad -s(f,\,\mathcal{P})<-I + \frac{\varepsilon}{2}\end{align}$
>  
>  Odakle, $S(f,\,\mathcal{P})-s(f,\,\mathcal{P})<\varepsilon$
>  $\:$
>  $\boxed{\Leftarrow}$ Pretpostavimo $\begin{align}\nexists\int_{a}^{b} f(x) \, dx\quad\Rightarrow\quad I_{*}<I^{*}\end{align}$.
>  
>  Treba naći $\varepsilon>0$, takav da $\forall\mathcal{P}\in\mathcal{P}[a,\,b]\quad S(f,\,\mathcal{P})-s(f,\,\mathcal{P})\geqslant\varepsilon$.
>  
>  $\exists c,\,d\in\mathbb{R}\ \ :\ \ \forall\mathcal{P}\in\mathcal{P}[a,\,b]\quad s(f,\,\mathcal{P})\leqslant I_{*}<c<d<I^{*}\leqslant S(f,\,\mathcal{P})$
>   - $S(f,\,\mathcal{P}) > d$
>  - $-s(f,\,\mathcal{P}) > -c$
>
>Odakle, $S(f,\,\mathcal{P})-s(f,\,\mathcal{P}) > d-c > 0$.
>$\varepsilon:=d-c$

$\:$
**Teorema**. $f:\ [a,\,b]\to \mathbb{R}$ je neprekidna. Tada  $f\,\mathcal{R}\,[a,\,b]$

**Teorema**. $f:\ [a,\,b]\to \mathbb{R}$ je monotona. Tada  $f\,\mathcal{R}\,[a,\,b]$
> Dokaz: neka $f\uparrow$ nije konstantna.
> Tada $\forall x\in[a,\,b]\quad f(a)\leqslant f(x)\leqslant f(b)$. Tj $f$ je ograničena.
> 
> Da bismo dokazali integrabilnost pomoću [[Određeni integral#^fdf6e4|teoreme]], za proizvoljno $\varepsilon>0$ treba naći $\mathcal{P}\in\mathcal{P}[a,\,b]$ takvo da $S(f,\,\mathcal{P})-s(f,\,\mathcal{P})<\varepsilon$.
> 
> $\begin{align}S(f,\,\mathcal{P})-s(f,\,\mathcal{P})=\sum\limits_{i=1}^{n}(M_{i}-m_{i})(x_{i}-x_{i-1})=\end{align}$
> >$M_{i}$ i $m_{i}$ postoje zbog ograničenosti.
> >$f\uparrow\quad\Rightarrow\quad M_{i}=f(x_{i}),\ \ m_{i}=f(x_{i-1})$
>
> $\begin{align}=\sum\limits_{i=1}^{n}\Big(f(x_{i})-f(x_{i-1})\Big)(x_{i}-x_{i-1})\leqslant\sum\limits_{i=1}^{n}\Big(f(x_{i})-f(x_{i-1})\Big)\lambda(\mathcal{P})=\end{align}$
> $=\Big(f(b)-f(a)\Big)\lambda(\mathcal{P})<\varepsilon$
> 
> Konačno, $\begin{align}\exists \mathcal{P}\in\mathcal{P}[a,\,b]\ \ :\ \ \lambda(\mathcal{P})<\frac{\varepsilon}{f(b)-f(a)}\end{align}$

$\:$
**Teorema**. $f:\ [a,\,b]\to \mathbb{R}$ je ograničena i ima konačan skup tačaka prekida. Tada  $f\,\mathcal{R}\,[a,\,b]$

**Teorema**. $f,\,g:\ [a,\,b]\to \mathbb{R}$ su $\mathcal{R}$-integrabilni i razlikuju se na konačnom skupu tačaka. Tada
$\begin{align}\int_{a}^{b} f(x) \, dx = \int_{a}^{b} g(x) \, dx\end{align}$

### Svojstva određenog integrala
**Stav**.  $f,\,g\,\mathcal{R}\,[a,\,b]$; $\ \ \alpha,\,\beta\in\mathbb{R}$. Tada $(\alpha\,f+\beta\,g)\,\mathcal{R}\,[a,\,b]$ i važi
$\begin{align}\int_{a}^{b} (\alpha\,f+\beta\,g)(x) \, dx = \alpha\int_{a}^{b} f(x) \, dx+\beta \int_{a}^{b} g(x) \, dx \end{align}$
> Dokaz:
> 1. Dokazati: $(f+g)\,\mathcal{R}\,[a,\,b]$ i $\begin{align}\int_{a}^{b} (f+g)(x) \, dx = \int_{a}^{b} f(x) \, dx + \int_{a}^{b} g(x) \, dx \end{align}$
>
>Neka je $(\mathcal{P},\,\xi)$ proizvoljna podela sa istaknutim tačkama intervala $[a,\,b]$.
>Tada, $\begin{align}\sigma(f+g,\,\mathcal{P},\,\xi)=\sum\limits_{i=1}^{n}(f+g)(\xi_{i})(x_{i}-x_{i-1})=\end{align}$
>$\begin{align}=\sum\limits_{i=1}^{n}f(\xi_{i})(x_{i}-x_{i-1})+\sum\limits_{i=1}^{n}g(\xi_{i})(x_{i}-x_{i-1})=\sigma(f,\,\mathcal{P},\,\xi)+\sigma(g,\,\mathcal{P},\,\xi)\end{align}$
>
>Odakle, $\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sigma(f+g,\,\mathcal{P},\,\xi) = \lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sigma(f,\,\mathcal{P},\,\xi)+\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sigma(g,\,\mathcal{P},\,\xi)=$
>$=\begin{align}\int_{a}^{b} f(x) \, dx +\int_{a}^{b} g(x) \, dx\quad\Rightarrow\end{align}$
>
>$\begin{align}\Rightarrow\quad\exists\int_{a}^{b} (f+g)(x) \, dx=\int_{a}^{b} f(x) \, dx +\int_{a}^{b} g(x) \, dx\end{align}$ 
>$\:$
>
2. Za $\alpha\in\mathbb{R}$ dokazati: $(\alpha\,f)\,\mathcal{R}\,[a,\,b]$ i $\begin{align}\int_{a}^{b} (\alpha\,f)(x) \, dx = \alpha\int_{a}^{b} f(x) \, dx\end{align}$
>
>Neka je $(\mathcal{P},\,\xi)$ proizvoljna podela sa istaknutim tačkama intervala $[a,\,b]$.
>Tada, $\begin{align}\sigma(\alpha\,f,\,\mathcal{P},\,\xi)=\sum\limits_{i=1}^{n}(\alpha\,f)(\xi_{i})(x_{i}-x_{i-1})=\end{align}$
>$\begin{align}=\alpha\sum\limits_{i=1}^{n}f(\xi_{i})(x_{i}-x_{i-1})=\alpha\cdot\sigma(f,\,\mathcal{P},\,\xi)\end{align}$
>
>Odakle, $\begin{align}\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sigma(\alpha\,f,\,\mathcal{P},\,\xi) = \alpha\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sigma(f,\,\mathcal{P},\,\xi)=\alpha\int_{a}^{b} f(x) \, dx\quad\Rightarrow\end{align}$
>
>$\begin{align}\Rightarrow\quad\exists\int_{a}^{b} (\alpha\,f)(x) \, dx=\alpha\int_{a}^{b} f(x) \, dx\end{align}$ 

$\:$
**Stav**.  $f,\,g\,\mathcal{R}\,[a,\,b]$. Tada
1. $(f\cdot g)\,\mathcal{R}\,[a,\,b]$
2. $|f|\,\mathcal{R}\,[a,\,b]$
3. $\begin{align}\frac{1}{f}\,\mathcal{R}\,[a,\,b],\quad\text{ako}\ \ \exists c\in[a,\,b]\quad\forall x\in[a,\,b]\quad |f(x)|>c\end{align}$
4. $f\,\mathcal{R}\,[c,\,d],\quad\text{za}\ \ [c,\,d]\subset[a,\,b]$

**Stav**. $f:[a,\,b]\to\mathbb{R}$, $\ \:$ $c\in(a,\,b)$. Tada
$f\,\mathcal{R}\,[a,\,b]\quad\Leftrightarrow\quad f\,\mathcal{R}\,[a,\,c]\ \ \text{i}\ \ f\,\mathcal{R}\,[c,\,b]$


**Stav**. Važe:
- $\begin{align}\int_{a}^{a} f(x) \, dx = 0\end{align}$
  $\:$
- za $\begin{align}f\,\mathcal{R}\,[a,\,b]\quad \int_{a}^{b} f(x) \, dx = -\int_{b}^{a} f(x) \, dx \end{align}$
  $\:$
- za $f\,\mathcal{R}\,\big[\min\{ a,\,b,\,c \},\,\max\{ a,\,b,\,c \}]$
  $\begin{align} \int_{a}^{b} f(x) \, dx =\int_{a}^{c} f(x) \, dx+\int_{c}^{b} f(x) \, dx \end{align}$

$\:$
**Stav**. $f\,\mathcal{R}\,[a,\,b] \ \ \ \text{i}\ \ \ \forall x\in[a,\,b]\quad f(x)\geqslant0$.
Tada $\begin{align}\int_{a}^{b} f(x) \, dx \geqslant0\end{align}$
> Dokaz:
> Neka je $(\mathcal{P},\,\xi)$ proizvoljna podela sa istaknutim tačkama intervala $[a,\,b]$.
>Tada, $\begin{align}\sigma(f,\,\mathcal{P},\,\xi)=\sum\limits_{i=1}^{n}f(\xi_{i})(x_{i}-x_{i-1})\geqslant0\end{align}$
>
>Odakle, $\begin{align}\int_{a}^{b} f(x) \, dx=\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sigma(f,\,\mathcal{P},\,\xi) \geqslant0\end{align}$


$\:$
**Posledica 1**. $f,\,g\,\mathcal{R}\,[a,\,b] \ \ \ \text{i}\ \ \ \forall x\in[a,\,b]\quad f(x)\leqslant g(x)$. Tada $\begin{align}\int_{a}^{b} f(x) \, dx \leqslant\int_{a}^{b} g(x) \, dx \end{align}$
> Dokaz: $(g-f)\,\mathcal{R}\,[a,\,b]$ $\ \:$ i $\ \:$ $\forall x\in[a,\,b]\quad g(x)-f(x)\geqslant0$
> 
> Tada, $\begin{align}\int_{a}^{b} g(x) \, dx - \int_{a}^{b} f(x) \, dx = \int_{a}^{b} (g-f)(x) \, dx \geqslant 0\end{align}$


$\:$
**Posledica 2**. $f\,\mathcal{R}\,[a,\,b]$. Tada $\begin{align}\left|\int_{a}^{b} f(x) \, dx \right|\leqslant\int_{a}^{b} \big|f(x)\big| \, dx \end{align}$
> Dokaz: 
> $\forall x\in [a,\,b] \quad -|f(x)|\overset{1.}\leqslant f(x) \overset{2.}\leqslant|f(x)|$
> 
> $\begin{align}1. \quad\Rightarrow\quad-\int_{a}^{b} |f(x)| \, dx \leqslant\int_{a}^{b} f(x) \, dx \quad\Rightarrow\quad-\int_{a}^{b} f(x) \, dx\leqslant \int_{a}^{b} |f(x)| \, dx\end{align}$ 
> 
> $\begin{align}2. \quad\Rightarrow\quad\int_{a}^{b} f(x) \, dx \leqslant\int_{a}^{b} |f(x)| \, dx\end{align}$ 

$\:$
### Predstavljanje određenog integrala proizvodom

$\:$
**Stav**. $\begin{align}f\,\mathcal{R}\,[a,\,b],\quad m= \inf_{x\in[a,\,b]}f(x),\quad M=\sup_{x\in[a,\,b]}f(x)\end{align}$. Tada
$\begin{align}\exists \mu\in[m,\,M]\ \:\ \ \int_{a}^{b} f(x) \, dx = \mu(b-a) \end{align}$
> Dokaz: 
> $\forall x\in[a,\,b]\quad m\leqslant f(x)\leqslant M$
> 
> $\begin{align}\int_{a}^{b} m \, dx  \leqslant \int_{a}^{b} f(x) \, dx\leqslant\int_{a}^{b} M \, dx\end{align}$
> 
> $\begin{align}m(b-a)\leqslant\int_{a}^{b} f(x) \, dx\leqslant M(b-a)\end{align}$
> 
> $\begin{align}m\leqslant\frac{\int_{a}^{b} f(x) \, dx}{b-a}\leqslant M\quad\Rightarrow\quad\frac{\int_{a}^{b} f(x) \, dx}{b-a}=\mu\in[m,\,M]\end{align}$ 

$\:$
**Stav**. $f\,\mathcal{C}\,[a,\,b]$. Tada $\ \:$ $\begin{align}\exists c\in[a,\,b]\ \:\ \ \int_{a}^{b} f(x) \, dx = f(c)(b-a) \end{align}$ ^88105f
> Dokaz: $f\,\mathcal{C}\,[a,\,b]\quad\Rightarrow\quad f\,\mathcal{R}\,[a,\,b]$
> 
> $f\,\mathcal{C}\,[a,\,b]\quad\overset{\text{Vajerštrasova teorema}}{\Rightarrow}$
> $\begin{align}\exists\min_{x\in[a,\,b]} f(x)=\inf_{x\in[a,\,b]} f(x)=m\ \ \text{i}\ \ \exists\max_{x\in[a,\,b]} f(x)=\sup_{x\in[a,\,b]} f(x)=M\end{align}$
>
>Iz prethodnog stava $\begin{align}\exists \mu\in[m,\,M]\quad\int_{a}^{b} f(x) \, dx=\mu(b-a)\end{align}$
> $f\,\mathcal{C}\,[a,\,b]\quad\overset{\text{teorema o međuvrednosti}}{\Rightarrow}\quad\exists c\in[a,\,b]\ \ :\ \ f(c)=\mu$