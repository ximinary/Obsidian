#fax #math #geom  [deo poglavlja [[Afino preslikavanje|"afino preslikavanje"]]]
$\:$

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

### Predstavljanje matricom

Afino preslikavanje u $\mathbb{E}^{2}$ dato formulom (2) možemo predstaviti matricom $A_{b}=\left(\begin{array}{}\alpha_{11}&\alpha_{12}&b_{1}\\\alpha_{21}&\alpha_{22}&b_{2}\\0&0&1\end{array}\right)$

(2) $\quad\Leftrightarrow\quad$ $\begin{align}\left(\begin{array}{}x'_{1}\\x'_{2}\\1\end{array}\right)=\left(\begin{array}{}\alpha_{11}&\alpha_{12}&b_{1}\\\alpha_{21}&\alpha_{22}&b_{2}\\0&0&1\end{array}\right)\left(\begin{array}{}x_{1}\\x_{2}\\1\end{array}\right)\end{align}$


**Teorema**. Proizvod matrica oblika $A_{b}$ odgovara kompoziciji afinih preslikavanja.

### Translacija u $\mathbb{E}^{2}$
Translacija $\mathcal{T}_{b}$ za vektor $b\,(b_{1},\,b_{2})$
$\begin{cases}x'_{1}=x_{1}+b_{1}\\x'_{2}=x_{2}+b_{2}\end{cases}$

$\begin{align}\mathcal{T}_{b}:\ \binom{x'_{1}}{x'_{2}}=\left(\begin{array}{}1&0\\0&1\end{array}\right)\binom{x_{1}}{x_{2}}+\binom{b_{1}}{b_{2}}\end{align}$

$\mathcal{T}_{b}:\ \left(\begin{array}{}1&0&b_{1}\\0&1&b_{2}\\0&0&1\end{array}\right)$

Translacija ne utiče na vektore.
Translacije komutiranju i kompozicija translacija je translacija:
$\mathcal{T}_{v}\circ\mathcal{T}_{u}=\mathcal{T}_{u}\circ \mathcal{T_{v}}=\mathcal{T}_{v\,+\,u}$

### Rotacija u $\mathbb{E}^{2}$
- rotacija oko koordinatnog početka za ugao $\varphi=[0,\,2\pi)$ :

$\begin{align}\mathcal{R}_{\varphi}:\ \binom{x'_{1}}{x'_{2}}=\underbrace{\left(\begin{array}{}\cos\varphi&-\sin\varphi\\\sin\varphi&\cos\varphi\end{array}\right)}_{\text{matrica rotacije } R_{\varphi}}\binom{x_{1}}{x_{2}}\end{align}$

$\mathcal{R}_{\varphi}:\ \left(\begin{array}{}\cos\varphi&-\sin\varphi&0\\\sin\varphi&\cos\varphi&0\\0&0&1\end{array}\right)$

- rotacija oko tačke $Q(q_{1},\,q_{2})$  za ugao $\varphi=[0,\,2\pi)$ :

$\mathcal{R}_{Q,\,\varphi}=\mathcal{T_{\overrightarrow{\rm OQ}}}\circ\mathcal{R_{\varphi}}\circ\mathcal{T}_{\overrightarrow{\rm QO}}$

$\:$
Svojstva:
1. $\det R_{\varphi}=1$
2. $R_{\varphi}\cdot R_{\theta}=R_{\theta}\cdot R_{\varphi}=R_{\varphi+\theta}$
3. $R_{-\varphi}=R^{-1}=R^{\mathrm{T}}$
4. $R_{0}=E$

$SO(2)=\big\{ R_{\varphi}\ \big|\ \varphi\in[0,\,2\pi)\big\}$ je grupa (svih rotacija).
### Refleksija u $\mathbb{E}^{2}$
- refleksija u odnosu na pravu $p_{0}$ koja prolazi kroz koordinatni početak i gradi ugao $\begin{align}\frac{\varphi}{2}\end{align}$ sa $e_{1}$ (osom $\mathrm{O}x_{1}$):

$\begin{align}\mathcal{S}_{p_{0}}:\ \binom{x'_{1}}{x'_{2}}=\underbrace{\left(\begin{array}{}\cos\varphi&\sin\varphi\\\sin\varphi&-\cos\varphi\end{array}\right)}_{\text{matrica refleksije } S_{\varphi}}\binom{x_{1}}{x_{2}}\end{align}$

$\mathcal{S}_{p_{0}}:\ \left(\begin{array}{}\cos\varphi&\sin\varphi&0\\\sin\varphi&-\cos\varphi&0\\0&0&1\end{array}\right)$



- refleksija u odnosu na pravu $p$ koja prolazi kroz $Q(q_{1},\,q_{2})$ i gradi ugao $\begin{align}\frac{\varphi}{2}\end{align}$ sa $e_{1}$ (osom $\mathrm{O}x_{1}$),   $\big($tj. $\ p\parallel p_{0}\big)$ :


$\mathcal{S}_{p}=\mathcal{T_{\overrightarrow{\rm OQ}}}\circ\mathcal{S}_{p_{0}}\circ\mathcal{T}_{\overrightarrow{\rm QO}}$

$\:$
Svojstva:
1. $\det S_{\varphi}=-1$
2. $S_{\varphi}\circ S_{\theta}=R_{\varphi-\theta}$
3. $S^{-1}=S^{\mathrm{T}}$
4. $S_{\varphi}^{2}=E$

Rotacije i refleksije čine ortogonalnu grupu:
$O(2)=\big\{ R_{\varphi}\ \big|\ \varphi\in[0,\,2\pi)\big\}\cup \big\{ S_{\varphi}\ \big|\ \varphi\in[0,\,2\pi)\big\}$

Refleksija kao kompozicija rotacija i skaliranja:
$\mathcal{S}_{\varphi}=\mathcal{R}_{\varphi/2}\circ\mathcal{H}_{1,\,-1}\circ\mathcal{R}_{-\varphi/2}$


$\boxed{S_{\varphi}=E-2nn^{\rm T}}$, gde je $n$ <u>jedinični</u> vektor normale na $p_{0}$.
> Tj. ako $n=(a,\,b)$ nije jedinični tada je  $\begin{align}n_{1}=\frac{n}{||n||}=\left( \frac{a}{\sqrt[]{a^{2}+b^{2}}},\,\frac{b}{\sqrt[]{a^{2}+b^{2}}} \right)\end{align}$ jedinični.
> Odakle $\begin{align}S_{\varphi}=E-2n_{1}n_{1}^{\rm T}=E-2\left(\begin{array}{}\frac{a^{2}}{a^{2}+b^{2}}&\frac{ab}{a^{2}+b^{2}}\\ \frac{ab}{a^{2}+b^{2}}&\frac{b^{2}}{a^{2}+b^{2}}\end{array}\right)=\end{align}$
> $\begin{align}=\left(\begin{array}{}1- \frac{2a^{2}}{a^{2}+b^{2}}&-\frac{2ab}{a^{2}+b^{2}}\\-\frac{2ab}{a^{2}+b^{2}}&1-\frac{2b^{2}}{a^{2}+b^{2}}\end{array}\right)=\frac{1}{a^{2}+b^{2}}\left(\begin{array}{}b^{2}-a^{2}&-2ab\\-2ab&a^{2}-b^{2}\end{array}\right)\end{align}$

$\:$
### Skaliranje u $\mathbb{E}^{2}$
- skaliranje u odnosu na koordinatni početak:

$\begin{align}\mathcal{H}_{\lambda_{1},\,\lambda_{2}}:\ \binom{x'_{1}}{x'_{2}}=\left(\begin{array}{}\lambda_{1}&0\\0&\lambda_{2}\end{array}\right)\binom{x_{1}}{x_{2}}\end{align}$

$\mathcal{H}_{\lambda_{1},\,\lambda_{2}}:\ \left(\begin{array}{}\lambda_{1}&0&0\\0&\lambda_{2}&0\\0&0&1\end{array}\right)$

- skaliranje u odnosu na tačku $Q(q_{1},\,q_{2})$ :

$\mathcal{H}_{Q,\,\lambda_{1},\,\lambda_{2}}=\mathcal{T_{\overrightarrow{\rm OQ}}}\circ\mathcal{H}_{\lambda_{1},\,\lambda_{2}}\circ\mathcal{T}_{\overrightarrow{\rm QO}}$
$\:$

Specijalni slučajevi:
- $\mathcal{H}_{1,\,1}=E$
- $\mathcal{H}_{1,\,-1}=\mathcal{S}_{0}$
- $\mathcal{H}_{-1,\,1}=\mathcal{S}_{\pi}$
- $\mathcal{H}_{-1,\,-1}=\mathcal{R}_{\pi}$

Ako $\lambda_{1}=\lambda_{2}=\lambda$, pišemo $\mathcal{H}_{\lambda} \ \ \Big(\mathcal{H}_{Q,\,\lambda}\Big)$ i kažemo da takvo preslikavanje **homotetija**.

### Smicanje u $\mathbb{E}^{2}$

- Smicanje sa koeficijentom $\lambda$ u odnosu na vektor $e_{1}$:

$\begin{align}\mathcal{S}_{e_{1}}(\lambda):\ \binom{x'_{1}}{x'_{2}}=\left(\begin{array}{}1&\lambda\\0&1\end{array}\right)\binom{x_{1}}{x_{2}}\end{align}$

![[afina preslikavanja 1 geo.png]]

- Smicanje sa koeficijentom $\lambda$ u odnosu na vektor $e_{2}$:

$\begin{align}\mathcal{S}_{e_{2}}(\lambda):\ \binom{x'_{1}}{x'_{2}}=\left(\begin{array}{}1&0\\\lambda&1\end{array}\right)\binom{x_{1}}{x_{2}}\end{align}$

___
Rotacija pomoću tri smicanja:

$\begin{align}\left(\begin{array}{} \cos\varphi&-\sin\varphi\\\sin\varphi&\cos\varphi\end{array}\right)= \left(\begin{array}{}1&\frac{\cos\varphi-1}{\sin\varphi}\\0&1\end{array}\right) \left(\begin{array}{}1&0\\\sin\varphi&1\end{array}\right)\end{align} \left(\begin{array}{}1&\frac{\cos\varphi-1}{\sin\varphi}\\0&1\end{array}\right)$
