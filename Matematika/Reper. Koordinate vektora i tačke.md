#fax #math #geom  [deo [[Geometrija|geometrije]]]
$\:$

Napomena: [[Koordinatizacija. Zavisnost koordinata vektora o bazi|koordinate vektora u bazi]]

Koordinate vektora $v$  [[Vektorski prostor|vektorskog prostora]] $\mathbb{V}^{n}$ u bazi  $e=\{ e_{1},\,e_{2},\,\dots,\,e_{n} \}$ su: $[v]_{e}=\left(\begin{array}{}x_{1}\\x_{2}\\\dots\\x_{n}\end{array}\right)=(x_{1},\,x_{2},\,\dots,\,x_{n})$. 

**Def**. Neka je $\mathbb{E}$ prostor tačaka;  $e=(e_{1},\,e_{2},\,\dots,\,e_{n})$ baza odgovarajućeg njemu  VP-a $\mathbb{V}$; $\mathrm{O}\in\mathbb{E}$ je fiksirana tačka. Tada $\mathrm{O}e$ je **koordinatni sistem** (**reper**) prostora $\mathbb{E}$; i $\mathrm{O}$ se zove **koordinatni početak**.

**Def**. Koordinate tačke $\mathrm{X}\in\mathbb{E}$ u reperu $\mathrm{O}e$ su:
$[\mathrm{X}]_{\mathrm{O}e}:=[\overrightarrow{\rm OX}]_{e}$

Stav. $\mathrm{M},\,\mathrm{N}\in\mathbb{E}$, $\mathrm{O}e$ je reper. Tada $[\overrightarrow{\rm MN}]_{e}=[\mathrm{N}]_{\mathrm{O}e}-[\mathrm{M}]_{\mathrm{O}e}$

### Transformacija koordinata vektora
Napomena: [[Koordinatizacija. Zavisnost koordinata vektora o bazi#Prelazak sa jedne baze na drugu|prelazak sa jedne baze na drugu]]

Prostor $\mathbb{V}^{n}$:
$e = (e_{1},\,e_{2},\,\dots e_{n})$ — stara baza
$f = (f_{1},\,f_{2},\,\dots f_{n})$ — nova baza

Matrica prelaska $C=C_{e\to f}$ sa baza $e$ u bazu $f$ je matrica čije su kolone redom koordinate vektora $f_{i}$ u bazi $e$.

Tada $\forall v\in \mathbb{V}^{n}\quad [v]_{e}=C[v]_{f}$

**Stav**. $\det C> 0\quad \Leftrightarrow\quad$ baze $e$ i  $f$ su iste orijentacije;
$\det C< 0\quad \Leftrightarrow\quad$ baze $e$ i  $f$ su različitih orijentacija.

### Transformacija koordinata tačaka
Prostor $\mathbb{E}$:
$\mathrm{O}e$ — stari reper
$\mathrm{Q}f$ — novi reper

$\begin{align}\forall \mathrm{X}\in \mathbb{E}\quad [\mathrm{X}]_{\mathrm{O}e}&=[\overrightarrow{\rm OX}]_{e}=[\overrightarrow{\rm OQ}+\overrightarrow{\rm QX}]_{e}=[\overrightarrow{\rm OQ}]_{e}+[\overrightarrow{\rm QX}]_{e}=\\&=[{\rm Q}]_{\mathrm{O}e}+C[\overrightarrow{\rm QX}]_{f}=C[\mathrm{X}]_{\mathrm{Q}f}+[Q]_{\mathrm{O}e}\end{align}$

$\begin{align}&q= [\mathrm{Q}]_{\mathrm{O}e}\\&x=[\mathrm{X}]_{\mathrm{O}e}\\&x'=[\mathrm{X}]_{\mathrm{Q}f}\end{align}\quad\quad\quad\quad\Rightarrow\quad \boxed{ x = Cx' + q}$ $\quad\quad (1)$

$C$ — linearni deo transformacije
$q$ — translatorni deo transformacije

### Transformacija ortonormiranih repera
Razmatramo specijalne slučajeve formule (1) u $\mathbb{V}^{2}$ sa ortonormiranim bazama: $e = (e_{1},\,e_{2})$ — stara i $f=(f_{1},\,f_{2})$ — nova; odgovarajući reperi su $\mathrm{O}e$ i $\mathrm{Q}f$.

$\begin{align}[\mathrm{Q}]_{\mathrm{O}e}=\binom{q_{1}}{q_{2}}\end{align}$

- Baze $e$ i $f$ su iste orijentacije:

$f_{1}$ gradi sa $e_{1}$ neki ugao $\varphi\in[0,\,2\pi)$

![[transformacija baze 1 geo.png]]

Tada $\begin{align}f_{1}=e_{1}\cos\varphi+e_{2}\sin \varphi\quad \Rightarrow\quad [f_{1}]_{e}=\binom{\cos\varphi}{\sin\varphi}\end{align}$
$\begin{align}f_{2}=-e_{1}\sin\varphi+e_{2}\cos \varphi\quad \Rightarrow\quad [f_{1}]_{e}=\binom{-\sin\varphi}{\cos\varphi}\end{align}$

Konačno: $\begin{align}\binom{x_{1}}{x_{2}}=\left(\begin{array}{}\cos\varphi&-\sin\varphi\\\sin\varphi&\cos\varphi\end{array}\right)\binom{x'_{1}}{x'_{2}}+\binom{q_{1}}{q_{2}}\end{align}$


___
$R_{\varphi}=\left(\begin{array}{}\cos\varphi&-\sin\varphi\\\sin\varphi&\cos\varphi\end{array}\right)$

1. $\det R_{\varphi}=1$
2. $R_{\varphi}\cdot R_{\theta}=R_{\varphi+\theta}$
3. $R_{-\varphi}=R^{-1}=R^{\mathrm{T}}$
4. $R_{0}=E$

Grupa rotacija:
$SO = \big\{ R_{\varphi} \ \big|\ \varphi \in [0,\,2\pi) \big\}$

___



- Baze $e$ i $f$ su različitih orijentacija:

$f_{1}$ gradi sa $e_{1}$ neki ugao $\varphi\in[0,\,2\pi)$

![[transformacija baze 2 geo.png]]

Imamo: $\begin{align}\binom{x_{1}}{x_{2}}=\left(\begin{array}{}\cos\varphi&\sin\varphi\\\sin\varphi&-\cos\varphi\end{array}\right)\binom{x'_{1}}{x'_{2}}+\binom{q_{1}}{q_{2}}\end{align}$

$\det\left(\begin{array}{}\cos\varphi&\sin\varphi\\\sin\varphi&-\cos\varphi\end{array}\right) =-1$