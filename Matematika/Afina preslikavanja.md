#fax #math #geom  [deo [[Geometrija|geometrije]]]
$\:$

**Def**. Neka je $\overline{f}: \mathbb{V}\to\mathbb{V}$ [[Linearni operator|linearni operator]] u prostoru $\mathbb{V}$ kojem je pridružen prostor tačaka $\mathbb{E}$. **Afino preslikavanje** indukovano preslikavanjem $\overline{f}$ je preslikavanje $f:\mathbb{E\to \mathbb{E}}$, takvo da važi:
$\mathrm{M}'=f(\mathrm{M}),\,\mathrm{N}'=f(N)\quad \Rightarrow\quad \overline{f}(\overrightarrow{\rm MN})=\overrightarrow{\rm M'N'}$

**Lema**. Svako afino preslikavanje u fiksiranom [[Reper. Koordinate vektora i tačke|reperu]] $\mathrm{O}e$ ima oblik:
$\big[f(\mathrm{M})\big]_{\mathrm{O}e}=A\cdot\big[\mathrm{M}\big]_{\mathrm{O}e}+b$, $\quad\quad\quad\quad\quad\quad(1)$ 
- gde je $A$  matrica preslikavanja $\overline{f}$ u bazi $e$,
  tj. kolone $A$ su redom slike vektora baze $e$,
- $b=\big[f(\mathrm{O})\big]_{\mathrm{O}e}$ — koordinate slike koordinatnog početka

> Dokaz:
> $\begin{align}\big[f(\mathrm{M})\big]_{\mathrm{O}e}-\big[f(\mathrm{O})\big]_{\mathrm{O}e}&=\big[\overrightarrow{f(\mathrm{O})f(\mathrm{M})}\big]_{e} = \big[\overline{f}(\overrightarrow{\rm OM})\big]_{e}=\big[\overline{f}\big]_{e}\big[\overrightarrow{\rm OM}\big]_{e}=\\&=A\cdot\big[M\big]_{\mathrm{O}e}\end{align}$

Formula (1) može se posmatrati kao:
- koordinate iste tačke u različitim bazama \[[[Reper. Koordinate vektora i tačke#Transformacija koordinata tačaka|*]]];
- koordinate slike afinog preslikavanja u fiksiranoj bazi.

Skup afinih preslikavanja u $n$-dim prostoru čine <u>grupu</u> $A\!f\!f_{n}(\mathbb{R})$

### Afina preslikavanja u ravni
Afino preslikavanje $f$ u $\mathbb{E}^{2}$ sa reperom $\mathrm{O}e$ je dato formulom
$\begin{align}\binom{x'_{1}}{x'_{2}}=\left(\begin{array}{}\alpha_{11}&\alpha_{12}\\\alpha_{21}&\alpha_{22}\end{array}\right)\binom{x_{1}}{x_{2}}+\binom{b_{1}}{b_{2}}\end{align}\quad$ za $\det( a_{ij})\ne0$,  $\quad\quad$ (2)

gde su $\quad$  $\begin{align}\big[\mathrm{M}\big]_{\mathrm{O}e}=\binom{x_{1}}{x_{2}}\quad\big[f(\mathrm{M})\big]_{\mathrm{O}e}=\binom{x'_{1}}{x'_{2}}\end{align}$
$\begin{align}\big[\overline{f}(e_{1})\big]_{e}=\binom{\alpha_{11}}{\alpha_{21}}\quad\big[\overline{f}(e_{2})\big]_{e}=\binom{\alpha_{12}}{\alpha_{22}}\quad\big[f(\mathrm{O})\big]_{\mathrm{O}e}=\binom{b_{1}}{b_{2}}\end{align}$
$\:$

**Teorema**. Postoji jedinstveno afino preslikavanje koje preslikava tri nekolinearne tačke $P,\,Q,\, R$ u tri nekolinearne tačke $P',\,Q',\,R'$

**Teorema** (Osobine afinih preslikavanja ravni).
1. Preslikavaju prave u prave
2. Čuvaju paralelnost pravih
3. Čuvaju odnos dužina kolinearnih duži
4. Odnos površina slike i originala $\begin{align}\frac{P(\mathcal{F}')}{P(\mathcal{F})}=|\det(a_{ij})|\end{align}$
5. Čuvaju centar mase i baricentričke koordinate
6. $\det(a_{ij}) > 0 \quad\Leftrightarrow\quad$ čuva se orijentacija trouglova
   $\det(a_{ij}) < 0 \quad\Leftrightarrow\quad$ menja se orijentacija trouglova

#### Predstavljanje matricom

Afino preslikavanje u $\mathbb{E}^{2}$ dato formulom (2) možemo predstaviti matricom $A_{b}=\left(\begin{array}{}\alpha_{11}&\alpha_{12}&b_{1}\\\alpha_{21}&\alpha_{22}&b_{2}\\0&0&1\end{array}\right)$

(2) $\quad\Leftrightarrow\quad$ $\begin{align}\left(\begin{array}{}x'_{1}\\x'_{2}\\1\end{array}\right)=\left(\begin{array}{}\alpha_{11}&\alpha_{12}&b_{1}\\\alpha_{21}&\alpha_{22}&b_{2}\\0&0&1\end{array}\right)\left(\begin{array}{}x_{1}\\x_{2}\\1\end{array}\right)\end{align}$


**Teorema**. Proizvod matrica oblika $A_{b}$ odgovara kompoziciji afinih preslikavanja.

#### Translacija
Translacija $\mathcal{T}_{b}$ za vektor $b\,(b_{1},\,b_{2})$
$\begin{cases}x'_{1}=x_{1}+b_{1}\\x'_{2}=x_{2}+b_{2}\end{cases}$

$\mathcal{T}_{b}:\ \begin{align}\binom{x'_{1}}{x'_{2}}=\left(\begin{array}{}1&0\\0&1\end{array}\right)\binom{x_{1}}{x_{2}}+\binom{b_{1}}{b_{2}}\end{align}$

$\mathcal{T}_{b}=\left(\begin{array}{}1&0&b_{1}\\0&1&b_{2}\\0&0&1\end{array}\right)$

Translacija ne utiče na vektore.
Translacije komutiranju i kompozicija translacija je translacija:
$\mathcal{T}_{v}\circ\mathcal{T}_{u}=\mathcal{T}_{u}\circ \mathcal{T_{v}}=\mathcal{T}_{v\,+\,u}$

#### Rotacija
- rotacija oko koordinatnog početka za ugao $\varphi=[0,\,2\pi)$ :

$\mathcal{R}_{\varphi}:\ \begin{align}\binom{x'_{1}}{x'_{2}}=\left(\begin{array}{}\cos\varphi&-\sin\varphi\\\sin\varphi&\cos\varphi\end{array}\right)\binom{x_{1}}{x_{2}}\end{align}$

$\mathcal{R}_{\varphi}=\left(\begin{array}{}\cos\varphi&-\sin\varphi&0\\\sin\varphi&\cos\varphi&0\\0&0&1\end{array}\right)$

- rotacija oko tačke $Q(q_{1},\,q_{2})$  za ugao $\varphi=[0,\,2\pi)$ :

$\mathcal{R}_{Q,\,\varphi}=\mathcal{T_{\overrightarrow{\rm OQ}}}\circ\mathcal{R_{\varphi}}\circ\mathcal{T}_{\overrightarrow{\rm QO}}$

$\:$
Svojstva:
1. $\det \mathcal{R}_{\varphi}=1$
2. $\mathcal{R}_{\varphi}\circ \mathcal{R}_{\theta}=\mathcal{R}_{\theta}\circ \mathcal{R}_{\varphi}=\mathcal{R}_{\varphi+\theta}$
3. $\mathcal{R}_{-\varphi}=\mathcal{R}^{-1}=\mathcal{R}^{\mathrm{T}}$
4. $\mathcal{R}_{0}=E$

$\big\{ \mathcal{R}_{\varphi}\ \big|\ \varphi\in[0,\,2\pi)\big\}$ je grupa.
#### Refleksija
- refleksija u odnosu na pravu $p_{0}$ koja prolazi kroz koordinatni početak i gradi ugao $\begin{align}\frac{\varphi}{2}\end{align}$ sa $e_{1}$ (osom $\mathrm{O}x$):

$\mathcal{S}_{\varphi}:\ \begin{align}\binom{x'_{1}}{x'_{2}}=\left(\begin{array}{}\cos\varphi&\sin\varphi\\\sin\varphi&-\cos\varphi\end{array}\right)\binom{x_{1}}{x_{2}}\end{align}$

$\mathcal{S}_{\varphi}=\left(\begin{array}{}\cos\varphi&\sin\varphi&0\\\sin\varphi&-\cos\varphi&0\\0&0&1\end{array}\right)$

- refleksija u odnosu na pravu $p$ koja prolazi kroz $Q(q_{1},\,q_{2})$ i gradi ugao $\begin{align}\frac{\varphi}{2}\end{align}$ sa $e_{1}$ (osom $\mathrm{O}x$),   $\big($tj. $\ p\parallel p_{0}\big)$ :


$\mathcal{S}_{Q,\,\varphi}=\mathcal{T_{\overrightarrow{\rm OQ}}}\circ\mathcal{S}_{\varphi}\circ\mathcal{T}_{\overrightarrow{\rm QO}}$

$\:$
Svojstva:
1. $\det \mathcal{S}_{\varphi}=-1$
2. $\mathcal{S}_{\varphi}\circ \mathcal{S}_{\theta}=\mathcal{R}_{\varphi-\theta}$
3. $\mathcal{S}^{-1}=\mathcal{S}^{\mathrm{T}}$
4. $\mathcal{S}_{\varphi}^{2}=E$

Rotacije i refleksije čine ortogonalnu grupu.

Refleksija kao kompozicija rotacija i skaliranja:
$\mathcal{S}_{\varphi}=\mathcal{R}_{\varphi/2}\circ\mathcal{H}_{1,\,-1}\circ\mathcal{R}_{-\varphi/2}$
#### Skaliranje
- skaliranje u odnosu na koordinatni početak:

$\mathcal{H}_{\lambda_{1},\,\lambda_{2}}:\ \begin{align}\binom{x'_{1}}{x'_{2}}=\left(\begin{array}{}\lambda_{1}&0\\0&\lambda_{2}\end{array}\right)\binom{x_{1}}{x_{2}}\end{align}$

$\mathcal{H}_{\lambda_{1},\,\lambda_{2}}=\left(\begin{array}{}\lambda_{1}&0&0\\0&\lambda_{2}&0\\0&0&1\end{array}\right)$

- skaliranje u odnosu na tačku $Q(q_{1},\,q_{2})$ :

$\mathcal{H}_{Q,\,\lambda_{1},\,\lambda_{2}}=\mathcal{T_{\overrightarrow{\rm OQ}}}\circ\mathcal{H}_{\lambda_{1},\,\lambda_{2}}\circ\mathcal{T}_{\overrightarrow{\rm QO}}$
$\:$

Specijalni slučajevi:
- $\mathcal{H}_{1,\,1}=E$
- $\mathcal{H}_{1,\,-1}=\mathcal{S}_{0}$
- $\mathcal{H}_{-1,\,1}=\mathcal{S}_{\pi}$
- $\mathcal{H}_{-1,\,-1}=\mathcal{R}_{\pi}$

Ako $\lambda_{1}=\lambda_{2}=\lambda$, pišemo $\mathcal{H}_{\lambda} \ \ \Big(\mathcal{H}_{Q,\,\lambda}\Big)$ i kažemo da takvo preslikavanje **homotetija**.

#### Smicanje

- Smicanje sa koeficijentom $\lambda$ u odnosu na vektor $e_{1}$:

$\mathcal{S}_{e_{1}}(\lambda):\ \begin{align}\binom{x'_{1}}{x'_{2}}=\left(\begin{array}{}1&\lambda\\0&1\end{array}\right)\binom{x_{1}}{x_{2}}\end{align}$

![[afina preslikavanja 1 geo.png]]

- Smicanje sa koeficijentom $\lambda$ u odnosu na vektor $e_{2}$:

$\mathcal{S}_{e_{2}}(\lambda):\ \begin{align}\binom{x'_{1}}{x'_{2}}=\left(\begin{array}{}1&0\\\lambda&1\end{array}\right)\binom{x_{1}}{x_{2}}\end{align}$

___
Rotacija pomoću tri smicanja:

$\begin{align}\left(\begin{array}{} \cos\varphi&-\sin\varphi\\\sin\varphi&\cos\varphi\end{array}\right)= \left(\begin{array}{}1&\frac{\cos\varphi-1}{\sin\varphi}\\0&1\end{array}\right) \left(\begin{array}{}1&0\\\sin\varphi&1\end{array}\right)\end{align} \left(\begin{array}{}1&\frac{\cos\varphi-1}{\sin\varphi}\\0&1\end{array}\right)$