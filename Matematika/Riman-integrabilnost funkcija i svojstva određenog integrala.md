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
>  $\forall\mathcal{P}\in\mathcal{P}[a,\,b]\quad s(f,\,\mathcal{P})\leqslant I_{*}<I^{*}\leqslant S(f,\,\mathcal{P})$
>   - $S(f,\,\mathcal{P}) \geqslant I^{*}$
>  - $-s(f,\,\mathcal{P}) \geqslant -I_{*}$
>
>Odakle, $S(f,\,\mathcal{P})-s(f,\,\mathcal{P}) \geqslant I^{*}-I_{*} > 0$.
>$\varepsilon:=I^{*}-I_{*}$

$\:$
**Teorema**. $f:\ [a,\,b]\to \mathbb{R}$ je neprekidna. Tada  $f\,\mathcal{R}\,[a,\,b]$

**Teorema**. $f:\ [a,\,b]\to \mathbb{R}$ je monotona. Tada  $f\,\mathcal{R}\,[a,\,b]$
> Dokaz: neka $f\uparrow$ nije konstantna.
> Tada $\forall x\in[a,\,b]\quad f(a)\leqslant f(x)\leqslant f(b)$. Tj $f$ je ograničena.
> 
> Da bismo dokazali integrabilnost pomoću [[Određeni integral#^fdf6e4|teoreme]], za proizvoljno $\varepsilon>0$ treba naći $\mathcal{P}\in\mathcal{P}[a,\,b]$ takvu da $S(f,\,\mathcal{P})-s(f,\,\mathcal{P})<\varepsilon$.
> 
> $\begin{align}S(f,\,\mathcal{P})-s(f,\,\mathcal{P})=\end{align}$
> > $m_{i}=\min\limits_{x\in[x_{i-1},\,x_{i}]}f(x)\quad M_{i}=\max\limits_{x\in[x_{i-1},\,x_{i}]}f(x),\quad \forall i=\overline{1,n}$
> > (postoje zbog ograničenosti)
> 
> $\begin{align}=\sum\limits_{i=1}^{n}(M_{i}-m_{i})(x_{i}-x_{i-1})=\end{align}$
> >$\forall i=\overline{1,n}\quad x_{i}-x_{i-1}\leqslant\lambda(\mathcal{P})$
>
> $\begin{align}\leqslant\sum\limits_{i=1}^{n}\Big(M_{i}-m_{i}\Big)\lambda(\mathcal{P})=\end{align}$
>
> >$f\uparrow\quad\Rightarrow\quad M_{i}= m_{i+1},\quad \forall i=\overline{1,n-1}$
> 
> $=\Big(M_{n}-m_{1}\Big)\lambda(\mathcal{P}) =\Big(f(b)-f(a)\Big)\lambda(\mathcal{P})<\varepsilon$
> 
> Konačno, $\begin{align}\exists \mathcal{P}\in\mathcal{P}[a,\,b]\ \ :\ \ \lambda(\mathcal{P})<\frac{\varepsilon}{f(b)-f(a)}\end{align}$

$\:$
**Teorema**. $f:\ [a,\,b]\to \mathbb{R}$ je ograničena i ima konačan skup tačaka prekida. Tada  $f\,\mathcal{R}\,[a,\,b]$

**Teorema**. $f,\,g:\ [a,\,b]\to \mathbb{R}$ su $\mathcal{R}$-integrabilni i razlikuju se na konačnom skupu tačaka. Tada
$\begin{align}\int_{a}^{b} f(x) \, dx = \int_{a}^{b} g(x) \, dx\end{align}$

### Svojstva određenog integrala
**Stav**.  $f,\,g\,\mathcal{R}\,[a,\,b]$; $\ \ \alpha,\,\beta\in\mathbb{R}$. Tada $(\alpha\,f+\beta\,g)\,\mathcal{R}\,[a,\,b]$ i važi
$\begin{align}\int_{a}^{b} (\alpha\,f+\beta\,g)(x) \, dx = \alpha\int_{a}^{b} f(x) \, dx+\beta \int_{a}^{b} g(x) \, dx \end{align}$ ^331d1c
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
3. $\begin{align}\frac{1}{f}\,\mathcal{R}\,[a,\,b],\quad\text{ako}\ \ \exists c>0\quad\forall x\in[a,\,b]\quad |f(x)|>c\end{align}$
4. $f\,\mathcal{R}\,[c,\,d],\quad\text{za}\ \ [c,\,d]\subset[a,\,b]$

**Stav**. $f:[a,\,b]\to\mathbb{R}$, $\ \:$ $c\in(a,\,b)$. Tada
$f\,\mathcal{R}\,[a,\,b]\quad\Leftrightarrow\quad f\,\mathcal{R}\,[a,\,c]\ \ \text{i}\ \ f\,\mathcal{R}\,[c,\,b]$


**Stav**. Važe:
- $\begin{align}\int_{a}^{a} f(x) \, dx = 0\end{align}$
  $\:$
- za $\begin{align}f\,\mathcal{R}\,[a,\,b]\quad \int_{a}^{b} f(x) \, dx = -\int_{b}^{a} f(x) \, dx \end{align}$
  $\:$
- za $f\,\mathcal{R}\,\big[\min\{ a,\,b,\,c \},\,\max\{ a,\,b,\,c \}]$
  $\begin{align} \int_{a}^{b} f(x) \, dx =\int_{a}^{c} f(x) \, dx+\int_{c}^{b} f(x) \, dx \end{align}$ ^58dd87

$\:$
**Stav**. $f\,\mathcal{R}\,[a,\,b] \ \ \ \text{i}\ \ \ \forall x\in[a,\,b]\quad f(x)\geqslant0$.
Tada $\begin{align}\int_{a}^{b} f(x) \, dx \geqslant0\end{align}$ ^606956
> Dokaz:
> Neka je $(\mathcal{P},\,\xi)$ proizvoljna podela sa istaknutim tačkama intervala $[a,\,b]$.
>Tada, $\begin{align}\sigma(f,\,\mathcal{P},\,\xi)=\sum\limits_{i=1}^{n}f(\xi_{i})(x_{i}-x_{i-1})\geqslant0\end{align}$
>
>Odakle, $\begin{align}\int_{a}^{b} f(x) \, dx=\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sigma(f,\,\mathcal{P},\,\xi) \geqslant0\end{align}$


$\:$
**Posledica 1**. $f,\,g\,\mathcal{R}\,[a,\,b] \ \ \ \text{i}\ \ \ \forall x\in[a,\,b]\quad f(x)\leqslant g(x)$. Tada $\begin{align}\int_{a}^{b} f(x) \, dx \leqslant\int_{a}^{b} g(x) \, dx \end{align}$ ^e67347
> Dokaz: $(g-f)\,\mathcal{R}\,[a,\,b]$ $\ \:$ i $\ \:$ $\forall x\in[a,\,b]\quad g(x)-f(x)\geqslant0$
> 
> Tada, $\begin{align}\int_{a}^{b} g(x) \, dx - \int_{a}^{b} f(x) \, dx = \int_{a}^{b} (g-f)(x) \, dx \geqslant 0\end{align}$


$\:$
**Posledica 2**. $f\,\mathcal{R}\,[a,\,b]$. Tada $\begin{align}\left|\int_{a}^{b} f(x) \, dx \right|\leqslant\int_{a}^{b} \big|f(x)\big| \, dx \end{align}$ ^ec936b
> Dokaz:  
> $\begin{align}\forall x\in [a,\,b] \quad -f(x)\leqslant |f(x)| \quad\Rightarrow\quad-\int_{a}^{b} f(x) \, dx\leqslant \int_{a}^{b} |f(x)| \, dx\end{align}$ 
> 
> $\begin{align}\forall x\in [a,\,b] \quad f(x)\leqslant|f(x)| \quad\Rightarrow\quad\int_{a}^{b} f(x) \, dx \leqslant\int_{a}^{b} |f(x)| \, dx\end{align}$ 

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