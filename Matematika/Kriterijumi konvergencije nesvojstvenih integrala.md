#fax #math #a2 [deo poglavlja [[Nesvojstveni integral|"nesvojstveni integral"]]]
$\:$
>Sledeći stavovi/teoreme su navedeni samo za interval $[a,\,b)$, gde je $b$ singularitet. Analogno postoje i odgovarajući stavovi/teoreme za interval $(a,\,b]$, gde je $a\in\mathbb{R}\cup\{-\infty\}$ singularitet.

$\:$
**Teorema** (Košijev kriterijum).
 $f:\ [a,\,b)\to\mathbb{R}$, $\ \:$ $b\in\mathbb{R}\cup\{+\infty\}$, $\ \:$ $\forall \beta\in [a,\,b)\quad f\,\mathcal{R}\,[a,\,\beta]$. Tada 
$\begin{align}\int_{a}^{b} f(x) \, dx\ \ \text{konvergira}\quad\Leftrightarrow\quad\forall\varepsilon>0\quad\exists\delta>0\quad\forall c,\,d\in \mathring{\mathrm{O}}_{\delta}^{-}(b)\quad\left|\int_{c}^{d} f(x) \, dx\right| < \varepsilon\end{align}$
> Dokaz: 
> $\begin{align}\int_{a}^{b} f(x) \, dx=\lim\limits_{ \beta \to b^{-} }\underbrace{\int_{a}^{\beta} f(x) \, dx}_{\varphi(\beta)}\end{align}$
> Integral konvergira akko  $\lim\limits_{ \beta \to b^{-} }\varphi (\beta)\in\mathbb{R}$
> 
> Iz [[Limes funkcije#^56c84c|Košijevog kriterijuma za postojanje limesa funkcije]]:
> $\begin{align}\lim\limits_{ \beta \to b^{-} }\varphi(\beta)\in\mathbb{R}\quad\Leftrightarrow\quad\forall\varepsilon>0\quad\exists\delta>0\quad\forall c,\,d\in \mathring{\mathrm{O}}_{\delta}^{-}(b)\quad&\left|\varphi(c)-\varphi(d)\right| < \varepsilon\\&\left|\int_{a}^{c} f(x) \, dx-\int_{a}^{d} f(x) \, dx\right| < \varepsilon\\&\left|\int_{c}^{d} f(x) \, dx\right| < \varepsilon\end{align}$

$\:$

**Stav**. $f,\,g:\ [a,\,b)\to\mathbb{R}$, $\ \:$ $b\in\mathbb{R}\cup\{+\infty\}$, $\ \:$ $\forall \beta\in [a,\,b)\quad f,\,g\,\mathcal{R}\,[a,\,\beta]$ i važi $\exists\delta>0\quad\forall x\in\mathring{\mathrm{O}}_{\delta}^{-}(b)\quad\boxed{|f(x)|\leqslant g(x)}$. Tada 
$\begin{align}\int_{a}^{b} g(x) \, dx\ \ \text{konvergira}\quad\Rightarrow\quad\int_{a}^{b} f(x) \, dx\ \ \text{konvergira}\end{align}$ ^a8ab77
> Dokaz:
> Iz Košijevog kriterijuma:
> $\begin{align}\int_{a}^{b} g(x) \, dx\ \ \text{konvergira}\quad\Rightarrow\quad\forall\varepsilon>0\quad\exists\delta_{1}>0\quad\forall c,\,d\in \mathring{\mathrm{O}}_{\delta_{1}}^{-}(b)\quad\left|\int_{c}^{d} g(x) \, dx\right| < \varepsilon\end{align}$
> 
> Iz svojstava određenog integrala ([[Riman-integrabilnost funkcija i svojstva određenog integrala#^e67347|1]], [[Riman-integrabilnost funkcija i svojstva određenog integrala#^ec936b|2]]):
> $\begin{align}\forall x\in\mathring{\mathrm{O}}_{\delta}^{-}(b)\quad\left|\int_{c}^{d} f(x) \, dx\right|\leqslant \int_{c}^{d} |f(x)| \, dx\leqslant\int_{c}^{d} g(x) \, dx <\varepsilon\end{align}$
> 
> Konačno:
> $\begin{align}\forall\varepsilon>0\quad\exists\delta_{2}:=\min\{\delta,\,\delta_{1}\}\quad\forall c,\,d\in \mathring{\mathrm{O}}_{\delta_{2}}^{-}(b)\quad\left|\int_{c}^{d} f(x) \, dx\right| < \varepsilon\quad\Rightarrow\end{align}$
> $\begin{align}\Rightarrow\quad\int_{a}^{b} f(x) \, dx\ \ \text{konvergira}\end{align}$

$\:$
**Teorema** (posledica stava). $f,\,g:\ [a,\,b)\to\mathbb{R}$, $\ \:$ $b\in\mathbb{R}\cup\{+\infty\}$, $\ \:$ $\forall \beta\in [a,\,b)\quad f,\,g\,\mathcal{R}\,[a,\,\beta]$ i važi $\exists\delta>0\quad\forall x\in\mathring{\mathrm{O}}_{\delta}^{-}(b)\quad\boxed{0\leqslant f(x)\leqslant g(x)}$. Tada 
- $\begin{align}\int_{a}^{b} g(x) \, dx\ \ \text{konvergira}\quad\Rightarrow\quad\int_{a}^{b} f(x) \, dx\ \ \text{konvergira}\end{align}$
- $\begin{align}\int_{a}^{b} f(x) \, dx\ \ \text{divergira}\quad\Rightarrow\quad\int_{a}^{b} g(x) \, dx\ \ \text{divergira}\end{align}$

$\:$
**Teorema**. $f,\,g:\ [a,\,b)\to\underbrace{[0,\,+\infty)}_{!!!}$, $\ \:$ $b\in\mathbb{R}\cup\{+\infty\}$, $\ \:$ $\forall \beta\in [a,\,b)\quad f,\,g\,\mathcal{R}\,[a,\,\beta]$ i $\begin{align}\exists\lim\limits_{ x \to b^{-} }\frac{f(x)}{g(x)}=A\end{align}$. Tada 
- Ako je $A=0$ onda $\begin{align}\int_{a}^{b} g(x) \, dx\ \ \text{konvergira}\quad\Rightarrow\quad\int_{a}^{b} f(x) \, dx\ \ \text{konvergira}\end{align}$
- Ako je $a = +\infty$ onda $\begin{align}\int_{a}^{b} f(x) \, dx\ \ \text{konvergira}\quad\Rightarrow\quad\int_{a}^{b} g(x) \, dx\ \ \text{konvergira}\end{align}$
- Ako je $0<A<+\infty$ onda su $\begin{align}\int_{a}^{b} g(x) \, dx\end{align}$ i $\begin{align}\int_{a}^{b} f(x) \, dx\end{align}$ ekvikonvergentni
(tj. ili oba konvergiraju ili oba divergiraju).

> Dokaz:
> Prvo tvrđenje.
>>$\begin{align}\lim\limits_{ x \to b^{-} }\frac{f(x)}{g(x)}=0\quad\Rightarrow\quad\forall\varepsilon>0\quad\exists\delta>0\quad\forall x\in\mathring{\mathrm{O}}_{\delta}^{-}(b)\quad\left|\frac{f(x)}{g(x)}\right|<\varepsilon\end{align}$
>> Uzimamo $\varepsilon = 1$ i jer fje su pozitivne  važi $\exists\delta>0\quad\forall x\in\mathring{\mathrm{O}}_{\delta}^{-}(b)\quad f(x)<g(x)$
>> i iz prethodne teoreme slede tvrđenje.
> 
> Drogo tvrđenje dobijamo iz prvog zamenom mesta fja $f$ i $g$.
> Treće tvrđenje.
>>$\begin{align}\lim\limits_{ x \to b^{-} }\frac{f(x)}{g(x)}=A\quad\Rightarrow\quad\forall\varepsilon>0\quad\exists\delta>0\quad\forall x\in\mathring{\mathrm{O}}_{\delta}^{-}(b)\quad&\left|\frac{f(x)}{g(x)}-A\right|<\varepsilon\\&A-\varepsilon<\frac{f(x)}{g(x)}< A+\varepsilon\end{align}$
>>
>>Iz pozitivnosti fja $f$ i $g$ i koristeći prethodnu teoremu dobijamo:
>> 1. Uzimamo $\varepsilon = \varepsilon_{1}$ tada važi 
>>  $\exists\delta>0\quad\forall x\in\mathring{\mathrm{O}}_{\delta}^{-}(b)\quad f(x)<(A+\varepsilon_{1})\cdot g(x)$
>> Odakle ako $\begin{align}\int_{a}^{b} (A+\varepsilon_{1})g(x) \, dx = (A+\varepsilon_{1})\int_{a}^{b} g(x) \, dx\end{align}$ konvergira onda i $\begin{align}\int_{a}^{b} f(x) \, dx \end{align}$ konvergira
>> 2. Uzimamo $\varepsilon = \varepsilon_{2} < A$ tada važi 
>>  $\begin{align}\exists\delta>0\quad\forall x\in\mathring{\mathrm{O}}_{\delta}^{-}(b)\quad g(x)<\frac{f(x)}{A-\varepsilon_{2}}\end{align}$
>> Odakle ako $\begin{align}\int_{a}^{b} \frac{f(x)}{A-\varepsilon_{2}} \, dx = \frac{1}{A-\varepsilon_{2}}\int_{a}^{b} f(x) \, dx\end{align}$ konvergira onda i $\begin{align}\int_{a}^{b} g(x) \, dx \end{align}$ konvergira