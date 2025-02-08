#fax #math #a2 [deo [[Analiza|analize]]]
$\:$

**Def**. 
- Neka su $a\in\mathbb{R},\ \ b\in\mathbb{R}\cup\{+\infty\}$ i neka je $f:\ [a,\,b)\to\mathbb{R}$ takva da $\forall \beta\in[a,\,b)\quad f\,\mathcal{R}\,[a,\,\beta]$. Tada se  **nesvojstveni integral** fje $f$ na $[a,\,b)$ definiše kao
$\begin{align}\int_{a}^{b} f(x) \, dx=\lim\limits_{ \beta \to b^{-} }\int_{a}^{\beta} f(x) \, dx\end{align}$
$b$ je singularitet.
$\:$
- Neka su $a\in\mathbb{R}\cup\{-\infty\},\ \ b\in\mathbb{R}$ i neka je $f:\ (a,\,b]\to\mathbb{R}$ takva da $\forall \alpha\in(a,\,b]\quad f\,\mathcal{R}\,[\alpha,\,b]$. Tada se  **nesvojstveni integral** fje $f$ na $(a,\,b]$ definiše kao
$\begin{align}\int_{a}^{b} f(x) \, dx=\lim\limits_{ \alpha \to a^{+} }\int_{\alpha}^{b} f(x) \, dx\end{align}$
$a$ je singularitet.

Ako limes postoji i konačan je onda nesvojstveni integral **konvergira**, inače **divergira**.
$\:$

>Sledeći stavovi su navedeni samo za interval $[a,\,b)$, gde je $b$ singularitet. Analogno postoje i odgovarajući stavovi za interval $(a,\,b]$, gde je $a\in\mathbb{R}\cup\{-\infty\}$ singularitet.

$\:$
**Stav**. $f:\ [a,\,b)\to\mathbb{R}$, $\ \:$ $b\in\mathbb{R}$, $\ \:$ $\forall \beta\in [a,\,b)\quad f\,\mathcal{R}\,[a,\,\beta]$. Tada 
ako $\lim\limits_{ \beta \to b^{-} }f(x)\in\mathbb{R}$ onda $\begin{align}\int_{a}^{b} f(x) \, dx\ \ \end{align}$ konvergira.
$\:$
**Stav**. $f:\ [a,\,+\infty)\to\mathbb{R}$, $\ \:$ $\forall \beta\in [a,\,+\infty)\quad f\,\mathcal{R}\,[a,\,\beta]$ i postoji $\begin{align}\lim\limits_{ \beta \to +\infty }f(x)=A\in\overline{\mathbb{R}}\end{align}$.
Tada ako $A\ne0$ onda $\ \:$ $\begin{align}\int_{a}^{+\infty} f(x) \, dx\ \ \end{align}$ divergira.
$\:$

**Stav**.  $f,\,g:\ [a,\,b)\to\mathbb{R}$, $\ \:$ $\forall \beta\in [a,\,b)\quad f\,\mathcal{R}\,[a,\,\beta]$. Tada
- Ako konvergiraju $\begin{align}\int_{a}^{b} f(x) \, dx \end{align}$ i $\begin{align}\int_{a}^{b} g(x) \, dx \end{align}$ onda konvergira $\begin{align}\int_{a}^{b} \big(\lambda f(x) + \mu g(x)\big) \, dx \end{align}$
i važi $\begin{align}\int_{a}^{b} \big(\lambda f(x) + \mu g(x)\big) \, dx = \lambda\int_{a}^{b} f(x) \, dx +\mu\int_{a}^{b} g(x) \, dx \end{align}$
$\:$
- Za $a<c<b$ ako konvergira $\begin{align}\int_{c}^{b} f(x) \, dx \end{align}$ onda konvergira $\begin{align}\int_{a}^{b} f(x) \, dx \end{align}$
i važi $\begin{align}\int_{a}^{b} f(x) \, dx = \underbrace{\int_{a}^{c} f(x) \, dx}_{\text{određeni integral}} +\int_{a}^{b} f(x) \, dx \end{align}$
$\:$
- Ako važi $f,\,g \,\mathcal{D}\,(a,\,b)$ i ako postoji i konačan je limes  $\begin{align}\lim\limits_{ \beta \to b^{-} }f(x)g(x) \end{align}$ onda 
 $\begin{align}\int_{a}^{b} f'(x)g(x) \, dx \ \ \text{konvergira}\quad \Leftrightarrow\quad \int_{a}^{b} f(x)g'(x) \, dx\ \ \text{konvergira} \end{align}$.
 
 > Dokaz:
 > Navedena svojstva direktno slede iz svojstava određenog integrala ([[Riman-integrabilnost funkcija i svojstva određenog integrala#^331d1c|1]], [[Riman-integrabilnost funkcija i svojstva određenog integrala#^58dd87|2]], [[Metode integracije (određeni integral)#^2e2625|3]]) i svojstava limesa.

$\:$
 **Def**. **Nesvojstveni integrali** sa više singulariteta:
 - Neka su $a\in\mathbb{R}\cup\{-\infty\},\ \ b\in\mathbb{R}\cup\{+\infty\}$ i neka je $f:\ (a,\,b)\to\mathbb{R}$ takva da $\forall \alpha,\,\beta\in(a,\,b)\quad f\,\mathcal{R}\,[\alpha,\,\beta]$. Tada ako za neko $c\in(a,\,b)$ konvergiraju $\begin{align}\int_{a}^{c} f(x) \, dx\end{align}$ i $\begin{align}\int_{c}^{b} f(x) \, dx\end{align}$ onda konvergira   $\begin{align}\int_{a}^{b} f(x) \, dx\end{align}$
   i važi $\boxed{\begin{align}\int_{a}^{b} f(x) \, dx=\int_{a}^{c} f(x) \, dx+\int_{c}^{b} f(x) \, dx\end{align}}$
$a$ i $b$ su singulariteti.
$\:$
 - Neka su $a<c<b$ realni i neka je $f:\ [a,\,c)\cup(c,\,b]\to\mathbb{R}$ takva da $\forall \beta\in[a,\,c)\quad f\,\mathcal{R}\,[a,\,\beta]$ $\ \:$ i $\ \:$ $\forall \alpha\in(c,\,b]\quad f\,\mathcal{R}\,[\alpha,\,b]$. Tada ako  konvergiraju $\begin{align}\int_{a}^{c} f(x) \, dx\end{align}$ i $\begin{align}\int_{c}^{b} f(x) \, dx\end{align}$ onda konvergira   $\begin{align}\int_{a}^{b} f(x) \, dx\end{align}$
   i važi $\boxed{\begin{align}\int_{a}^{b} f(x) \, dx=\int_{a}^{c} f(x) \, dx+\int_{c}^{b} f(x) \, dx\end{align}}$
$c$ je singularitet.
$\:$
- Nesvojstveni integral sa više singulariteta (na krajevima i/ili unutra intervala) treba pomoću zaokruženih formula razviti na <u>zbir više nesvojstvenih integrala sa po jednim singularitetom na jednom od krajeva intervala</u>. Tada ako svaki sabirak konvergira konvergira i polazni integral.

> Napomena: U drugom (a samim tim i trećem) delu definicije $f$ bi mogla da bude definisana u tački $c$, ali $c$ bi ostao singularitet ako je $c$ tačka [[Prekidi|prekida druge vrste]]. Isto važi i za polaznu definiciju nesvojstvenog integrala.

___

**Def**. Integral $\begin{align}\int_{a}^{b} f(x) \, dx\end{align}$ **konvergira apsolutno** ako $\begin{align}\int_{a}^{b} |f(x)| \, dx\end{align}$ konvergira.

**Stav**. Ako integral $\begin{align}\int_{a}^{b} f(x) \, dx\end{align}$ konvergira apsolutno tada on konvergira.
> Dokaz: tvrđenje sledi iz [[Kriterijumi konvergencije nesvojstvenih integrala#^a8ab77|stava]] uzimajući $g(x):=|f(x)|$
___

**Stav**.
1. $\begin{align}\int_{1}^{+\infty}  \frac{dx}{x^{\alpha}} \end{align}$ $\ \:$ konvergira za $\alpha>1$
$\:$
2. $\begin{align}\int_{0}^{1}  \frac{dx}{x^{\alpha}} \end{align}$ $\ \:$ konvergira za $\alpha<1$
$\:$
### [[Kriterijumi konvergencije nesvojstvenih integrala]]
### [[Gama funkcija i beta funkcija]]