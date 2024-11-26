#fax #math #a2 [deo [[Analiza|analize]]]


### Veza površine figure između $f(x)$ i $\mathrm{O}x$ i  [[Neodređeni integral#Primitivna funkcija|primitivne funkcije]] $F(x)$

Neka je $f:(c,\,d)\to[0,\,+\infty)$ neprekidna funkcija. $[a,\,b]\subset(c,\,d)$.
$\Phi = \big\{ (x,\,y)\in\mathbb{R}^{2}\ \big|\ a\leqslant x\leqslant b,\ \ 0\leqslant y \leqslant f(x) \big\}$ — figura ograničena sa $f(x)$ i $\mathrm{O}x$ na intervalu $[a,\,b]$.
$P(\Phi)$ — površina figure.

$t\in[a,\,b]$
$A(t)=\big\{ (x,\,y)\in\mathbb{R}^{2}\ \big|\ a\leqslant x\leqslant t,\ \ 0\leqslant y \leqslant f(x) \big\}$ — figura na intervalu $[a,\,t]$, deo figure $\Phi$.
$P(t)$ — površina figure $A(t)$.

$P: (a,\,b)\to[0,\,+\infty)$ $\quad\quad$ $P(a)=0$ $\quad\quad$ $P(b)=P(\Phi)$

$\:$
$\forall t\in[a,\,b)\quad\exists h>0\quad (t+h)\in[a,\,b)$

$\begin{align}M = \max_{t\,<\,x\,<\,t+h} f(x).\quad \exists 0\leqslant\theta_{1}\leqslant1\ \ : \ \ M=f(t+\theta_{1}h)\end{align}$
$\begin{align}m = \min_{t\,<\,x\,<\,t+h} f(x).\quad \exists 0\leqslant\theta_{2}\leqslant1\ \ : \ \ m=f(t+\theta_{2}h)\end{align}$

Površina figure na intervalu $[t,\,t+h]$ je $P(t+h)-P(t)$. I važi:

$m\,h\leqslant P(t+h)-P(t) \leqslant M\,h\quad\big|:h$

$\begin{align}f(t+\theta_{2}h)\leqslant \frac{P(t+h)-P(t)}{h} \leqslant f(t+\theta_{1}h)\end{align}\quad\big|\,h\to0$

$f(t)\leqslant P'(t)\leqslant f(t)$

Dakle, $\forall t\in[a,\,b)\quad P'(t)=f(t)$,
tj $P$ je primitivna za $f$ na $(a,\,b)$

Neka je $F:(c,\,d)\to\mathbb{R}$ proizvoljna primitivna za $f$ na $(c,\,d)\supset[a,\,b]$,
tada $\forall t \in [a,\,b)\quad P(t)=F(t)+C,\quad C\in\mathbb{R}$

$P(a)= 0\quad \Rightarrow\quad C=- F(a)\quad \Rightarrow\quad P(t)=F(t)-F(a)$

Konačno, površina figure ograničene sa $f(x)$ i $\mathrm{O}x$ na intervalu $[a,\,b]\subset(c,\,d)$ je $F(b)-F(a)$, gde je $F$ proizvoljna primitivna za $f$ na $(c,\,d)$

### Definicija određenog integrala
$f:\ [a,\,b]\to\mathbb{R}$

**Def**. Neka su $a=x_{0}<x_{1}<\dots<x_{n}=b$. Skup $\mathcal{P}=\Big\{ [x_{i-1},\,x_{i}]\ \Big|\ i=\overline{1,n} \Big\}$ je **podela** intervala $[a,\,b]$.

$x_{0},\,x_{1},\,\dots,\,x_{n}$ su **podeove tačke** podele $\mathcal{P}$.

$\begin{align}\lambda(\mathcal{P})=\max_{i=\overline{1,\,n}}(x_{i}-x_{i-1})\end{align}\ \:$ je **parametar podele** $\mathcal{P}$.

$\mathcal{P}[a,\,b]$ — skup svih podela intervala $[a,\,b]$.

$\mathcal{P},\,\mathcal{P}'\in\mathcal{P}[a,\,b]$. $\ \:$ $\mathcal{P}'$ je **finija** (**grublja**) podela od $\mathcal{P}$ ako je skup podeovih tačaka podele $\mathcal{P}'$ nadskup (podskup) skupa podeovih tačaka podele $\mathcal{P}$.

**Stav**. $\forall\mathcal{P}',\,\mathcal{P}''\in\mathcal{P}[a,\,b]\quad\exists\mathcal{P}\in\mathcal{P}[a,\,b]\ \ :\ \ \mathcal{P}$ je finija i od $\mathcal{P}'$ i od $\mathcal{P}''$
(Skup podeonih tačaka $\mathcal{P}$ je unija podeonih tačaka $\mathcal{P}'$ i $\mathcal{P}''$).
Tada $\mathcal{P}$ je **superpozicija podela** $\mathcal{P}'$ i $\mathcal{P}''$.

$\xi_{i}\in[x_{i-1},\,x_{i}],\quad \forall i=\overline{1,n}$. Tada su
$\xi=(\xi_{1},\,\xi_{2},\,\dots,\,\xi_{n})$ istaknute tačke podele $\mathcal{P}$.

$(\mathcal{P},\,\xi)$ — podela sa istaknutim tačkama intervala $[a,\,b]$

**Def**. Neka je $f:\ [a,\,b]\to\mathbb{R}\ \:$ i $\ \:(\mathcal{P},\,\xi)$ podela sa istaknutim tačkama intervala $[a,\,b]$. Zbir $\begin{align}\sigma(f,\,\mathcal{P},\,\xi)=\sum\limits_{i=1}^{n}(x_{i}-x_{i-1})\,f(\xi_{i})\end{align}$ je **integralna suma**.

---
**Definicija** (pomoću integralnih suma). Neka je $f:\ [a,\,b]\to\mathbb{R}$. $\ \:$ $I\in\mathbb{R}$ je limes integralnih suma $\sigma(f,\,\mathcal{P},\,\xi)$ kad $\lambda(\mathcal{P})\to0$, ako
$\begin{align}\forall\varepsilon>0\quad\exists\delta>0\quad\forall\binom{(\mathcal{P,\,\xi} )\ \text{— podela sa istaknutim tačkama}}{\text{ intervala }[a,\,b]\text{ takva da } \mathcal{P}(\lambda)<\delta}\quad \Big|I-\sigma(f,\,\mathcal{P},\,\xi)\Big|<\varepsilon\end{align}$
$\:$
Tada je $\begin{align}I=\int_{a}^{b} f(x) \, dx \end{align}$ $\:$ Rimanov (određeni) integral fje $f$ na $[a,\,b]$.

Ako postoji Rimanov integral (odnosno limes), $f$ je Riman-integrabilna ($\mathcal{R}$-integrabilna) na $[a,\,b]$. Oznaka $f\,\mathcal{R}\,[a,\,b]$

**Stav**. Ako $f:\ [a,\,b]\to\mathbb{R}$ nije ograničena na $[a,\,b]$ onda $\begin{align}\nexists\int_{a}^{b} f(x) \, dx \end{align}$
___
Neka je $f:\ [a,\,b]\to\mathbb{R}$ ograničena i $\mathcal{P}$ je podela intervala $[a,\,b]$.
$\forall i=\overline{1,n}\quad\quad\begin{array}{}m_{i}:=\inf\{ f(x)\ \big|\ x_{i-1}\leqslant x\leqslant x_{i} \}\\M_{i}:=\sup\{ f(x)\ \big|\ x_{i-1}\leqslant x\leqslant x_{i} \}\end{array}$

**Def**. 
$\begin{align}s(f,\,\mathcal{P})=\sum\limits_{i=1}^{n}m_{i}(x_{i}-x_{i-1})\end{align}$ $\quad$ je **donja Darbuova suma**;
$\begin{align}S(f,\,\mathcal{P})=\sum\limits_{i=1}^{n}M_{i}(x_{i}-x_{i-1})\end{align}$ $\quad$ je **gornja Darbuova suma**.

**Stav**. $\forall\mathcal{P}',\,\mathcal{P}''\in\mathcal{P}[a,\,b]\quad s(f,\,\mathcal{P'})\leqslant S(f,\,\mathcal{P''})$
> Dokaz: Neka je $\mathcal{P}$ superpozicija podela $\mathcal{P}'$ i $\mathcal{P}''$,
> tada treba pokazati: $s(f,\,\mathcal{P'})\overset{1.}{\leqslant} s(f,\,\mathcal{P})\overset{2.}{\leqslant} S(f,\,\mathcal{P})\overset{3.}{\leqslant} S(f,\,\mathcal{P''})$
>1. Neki interval podele $\mathcal{P'}$ može da sadrži dve ili više podeone tačke podele $\mathcal{P}$.
>   Neka je $\hat{x}_{i}$ podeona tačka podele $\mathcal{P}$ takva da $\hat{x}_{i}\in[x_{i-1},\,x_{i}]\in\mathcal{P}'$.
>   Tada sabirku $m_{i}(x_{i}-x_{i-1})$ sume $s(f,\,\mathcal{P}')$ odgovaraju dva sabirka $m'_{i}(\hat{x}_{i}-x_{i-1})$, $m''_{i}(x_{i}-\hat{x}_{i})$ sume $s(f,\,\mathcal{P})$.
>   i jer je $m_{i}$ infinum na celom intervalu, važi $m_{i}\leqslant m'_{i},\,m''_{i}$, odakle
>   $m_{i}(x_{i}-x_{i-1})\ \leqslant\ m'_{i}(\hat{x}_{i}-x_{i-1})\ +\ m''_{i}(x_{i}-\hat{x}_{i})$
>   Slično za intervale sa više tačaka. Dakle, važi 1.
>  2. $m_{i}\leqslant M_{i}$. Odakle sledi 2.
>  3. 3\. je slično kao i 1.

$\:$

Odakle,
- $\{ s(f,\,\mathcal{P})\ |\ \mathcal{P}\in\mathcal{P}[a,\,b] \}$ je neprazan i ograničen odozgo sa $S(f,\,\mathcal{P''})$
  $\Rightarrow\quad\exists\sup\{ s(f,\,\mathcal{P})\ |\ \mathcal{P}\in\mathcal{P}[a,\,b] \}=:I_{*}$ — **donji Rimanov integral**.
  $\:$
- $\{ S(f,\,\mathcal{P})\ |\ \mathcal{P}\in\mathcal{P}[a,\,b] \}$ je neprazan i ograničen odozdo sa $s(f,\,\mathcal{P'})$
  $\Rightarrow\quad\exists\inf\{ S(f,\,\mathcal{P})\ |\ \mathcal{P}\in\mathcal{P}[a,\,b] \}=:I^{*}$ — **gornji Rimanov integral**.

Važi $I_{*}\leqslant I^{*}$.

**Teorema** (Definicija pomoću Darbuovih suma). Ako $I_{*}=I^{*}=I$ onda je $I=\begin{align}\int_{a}^{b} f(x) \, dx \end{align}$ Rimanov integral fje $f$ na $[a,\,b]$.

### $\mathcal{R}$-integrabilnost i svojstva određenog integrala

**Teorema**. $f:\ [a,\,b]\to\mathbb{R}$ ograničena fja. Tada
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
Teorema. $f:\ [a,\,b]\to \mathbb{R}$ je neprekidna. Tada  $f\,\mathcal{R}\,[a,\,b]$

Teorema. $f:\ [a,\,b]\to \mathbb{R}$ je monotona. Tada  $f\,\mathcal{R}\,[a,\,b]$
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
Teorema. $f:\ [a,\,b]\to \mathbb{R}$ je ograničena i ima konačan skup tačaka prekida. Tada  $f\,\mathcal{R}\,[a,\,b]$

Teorema. $f,\,g:\ [a,\,b]\to \mathbb{R}$ su $\mathcal{R}$-integrabilni i razlikuju se na konačnom skupu tačaka. Tada
$\begin{align}\int_{a}^{b} f(x) \, dx = \int_{a}^{b} g(x) \, dx\end{align}$
___
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
- $\begin{align}\int_{a}^{a} f(x) \, dx \end{align}$
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
>Tada, $\begin{align}\sigma(f,\,\mathcal{P},\,\xi)=\sum\limits_{i=1}^{n}(f)(\xi_{i})(x_{i}-x_{i-1})\geqslant0\end{align}$
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
**Stav**. $f\,\mathcal{C}\,[a,\,b]$. Tada $\ \:$ $\begin{align}\exists c\in[a,\,b]\ \:\ \ \int_{a}^{b} f(x) \, dx = f(c)(b-a) \end{align}$
> Dokaz: $f\,\mathcal{C}\,[a,\,b]\quad\Rightarrow\quad f\,\mathcal{R}\,[a,\,b]$
> 
> $f\,\mathcal{C}\,[a,\,b]\quad\overset{\text{Vajerštrasova teorema}}{\Rightarrow}$
> $\begin{align}\exists\min_{x\in[a,\,b]} f(x)=\inf_{x\in[a,\,b]} f(x)=m\ \ \text{i}\ \ \exists\max_{x\in[a,\,b]} f(x)=\sup_{x\in[a,\,b]} f(x)=M\end{align}$
>
>Iz prethodnog stava $\begin{align}\exists \mu\in[m,\,M]\quad\int_{a}^{b} f(x) \, dx=\mu(b-a)\end{align}$
> $f\,\mathcal{C}\,[a,\,b]\quad\overset{\text{teorema o međuvrednosti}}{\Rightarrow}\quad\exists c\in[a,\,b]\ \ :\ \ f(c)=mu$

$\:$
### Njutn-Lajbnicova formula
Oznake za sledeće teoreme:
$f\,\mathcal{R}\,[a,\,b]$;$\quad$ $\varphi:[a,\,b]\to\mathbb{R}$ def. sa $\begin{align}\varphi(x)=\int_{a}^{x} f(t) \, dt \end{align}$

**Teorema**. $\varphi\,\mathcal{C}\,[a,\,b]$.
> Dokaz: Neka je $\ \:$ $\begin{align}M=\sup_{x\in[a,\,b]}|f(x)|>0\end{align}$
> $x_{0}\in[a,\,b]$ — proizvoljno. Treba dokazati $f\,\mathcal{C}\,x_{0}$, tj.
> $\forall \varepsilon>0\quad\exists\delta>0\quad\forall x\in[a,\,b]\cap (x_{0}-\delta,\,x_{0}+\delta)\quad|\varphi(x)-\varphi(x_{0})|<\varepsilon$
> 
> Za proizvoljno $\varepsilon>0$ naći $\delta>0$.
> 
> $\begin{align}|\varphi(x)-\varphi(x_{0})|<\left|\int_{a}^{x} f(t) \, dt-\int_{a}^{x_{0}} f(t) \, dt\right|=\end{align}$
> $\begin{align}=\left|\int_{x_{0}}^{x} f(t) \, dt\right|\leqslant\left|\int_{x_{0}}^{x} \big|f(t)\big| \, dt\right|\leqslant M\cdot|x-x_{0}|<\varepsilon\end{align}$
> 
> $\begin{align}|x-x_{0}|<\frac{\varepsilon}{M}=:\delta\end{align}$

$\:$
Teorema. $f\,\mathcal{C}\,[a,\,b]\quad\Rightarrow\quad\varphi\,\mathcal{D}\,(a,\,b)\ \ \text{i}\ \ f\,\mathcal{C}\,[a,\,b]$, i važi
$\forall x\in(a,\,b)\quad\varphi'(x)=f(x)$; $\quad$ $\varphi'_{+}(a)=f(a)$; $\quad$ $\varphi'_{-}(b)=f(b)$
> Dokaz:

$\:$