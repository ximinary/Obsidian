#fax #math #geom  [deo poglavlja [[Afino preslikavanje|"afino preslikavanje"]]]
$\:$

Afino preslikavanje $f$ u $\mathbb{E}^{3}$ sa reperom $\mathrm{O}e$ je dato formulom
$\begin{align}\left(\begin{array}{}x'_{1}\\x'_{2}\\x'_{3}\end{array}\right)=\left(\begin{array}{}\alpha_{11}&\alpha_{12}&\alpha_{13}\\\alpha_{21}&\alpha_{22}&\alpha_{23}\\\alpha_{31}&\alpha_{32}&\alpha_{33}\end{array}\right)\left(\begin{array}{}x_{1}\\x_{2}\\x_{3}\end{array}\right)+\left(\begin{array}{}b_{1}\\b_{2}\\b_{3}\end{array}\right)\end{align}\quad$ za $\det( a_{ij})\ne0$,  $\quad\quad$ (2)

gde su $\quad$  $\begin{align}\big[\mathrm{M}\big]_{\mathrm{O}e}=\left(\begin{array}{}x_{1}\\x_{2}\\x_{3}\end{array}\right)\quad\big[f(\mathrm{M})\big]_{\mathrm{O}e}=\left(\begin{array}{}x'_{1}\\x'_{2}\\x'_{3}\end{array}\right)\end{align}$
$\begin{align}\big[\overline{f}(e_{1})\big]_{e}=\left(\begin{array}{}\alpha_{11}\\\alpha_{21}\\\alpha_{31}\end{array}\right)\quad\big[\overline{f}(e_{2})\big]_{e}=\left(\begin{array}{}\alpha_{12}\\\alpha_{22}\\\alpha_{32}\end{array}\right)\quad\quad\big[\overline{f}(e_{3})\big]_{e}=\left(\begin{array}{}\alpha_{13}\\\alpha_{23}\\\alpha_{33}\end{array}\right)\end{align}$
$\begin{align}\big[f(\mathrm{O})\big]_{\mathrm{O}e}=\left(\begin{array}{}b_{1}\\b_{2}\\b_{3}\end{array}\right)\end{align}$
$\:$

___
Predstavljanje jednom matricom $A_{b}=\left(\begin{array}{}\alpha_{11}&\alpha_{12}&\alpha_{13}&b_{1}\\\alpha_{21}&\alpha_{22}&\alpha_{23}&b_{2}\\\alpha_{31}&\alpha_{32}&\alpha_{33}&b_{3}\\0&0&0&1\end{array}\right)$
### Translacija u $\mathbb{E}^{3}$
Translacija $\mathcal{T}_{b}$ za vektor $b\,(b_{1},\,b_{2},\,b_{3})$

$\begin{align}\mathcal{T}_{b}:\ \left(\begin{array}{}x'_{1}\\x'_{2}\\x'_{3}\end{array}\right)=\left(\begin{array}{}1&0&0\\0&1&0\\0&0&1\end{array}\right)\left(\begin{array}{}x_{1}\\x_{2}\\x_{3}\end{array}\right)+\left(\begin{array}{}b_{1}\\b_{2}\\b_{3}\end{array}\right)\end{align}$

analogno sa translacijom u $\mathbb{E}^{2}$
### Rotacija u $\mathbb{E}^{3}$
![[afina preslikavanja 2 geo.png]]
Rotacija oko usmerene prave $p$ za ugao $\varphi$.
Ako je $\varphi$ pozitivan rotiramo pomoću pravila desne ruke (palac u smeru usmerene prave, tada prsti u pesnici pokazuju smer rotacije).

Rotacija tačke $M$ oko prave $p$ u prostoru se svodi na rotaciju $M$ u $\big[$ ravni $\alpha$ koja je normalna na $p$ i koja sadrži $A$ $\big]$ oko tačke u preseku $p$ i $\alpha$.

##### Rotacija oko ose $\mathrm{O}x_{1}$ za ugao $\varphi$
$[\mathcal{R}_{\mathrm{O}x_{1}}(\varphi)]_{e}=R_{\mathrm{O}x_{1}}(\varphi)=\left(\begin{array}{}1&0&0\\0&\cos\varphi&-\sin\varphi\\0&\sin\varphi&\cos\varphi\end{array}\right)$
![[afina preslikavanja 3.1 geo.png]]
##### Rotacija oko ose $\mathrm{O}x_{2}$ za ugao $\theta$
$[\mathcal{R}_{\mathrm{O}x_{2}}(\theta)]_{e}=R_{\mathrm{O}x_{2}}(\theta)=\left(\begin{array}{}\cos \theta&0&\sin \theta\\0&1&0\\-\sin\theta&0&\cos\theta\end{array}\right)$
![[afina preslikavanja 3.2 geo.png]]
> Objašnjenje:
> pri rotacije oko $\mathrm{O}x_{2}$ druga koordinata se ne menja tj. $x_{2}=x'_{2}$, ostale koordinate se dobijaju rotiranjem u ravni $\mathrm{O}x_{3}x_{1}$ ili njoj paralelnoj za ugao $\theta$ oko koordinatnog početka:
> $(x_{3},\, x_{1})$ je pozitivna baza gledajući sa $x_{2}$ i jer rotiramo od $x_{3}$ ka $x_{1}$ imamo
> 
> $\begin{align}\binom{x'_{3}}{x'_{1}}=\left(\begin{array}{}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{array}\right)\binom{x_{3}}{x_{1}}\end{align}$
> 
> $\Rightarrow\quad\begin{cases}x'_{1}=x_{3}\sin \theta+x_{1}\cos \theta\\x'_{2}=x_{2}\\x'_{3}=x_{3}\cos \theta-x_{1}\sin \theta\end{cases}$
> 
> $\Rightarrow\quad\left(\begin{array}{}x'_{1}\\x'_{2}\\x'_{3}\end{array}\right)=\left(\begin{array}{}\cos \theta&0&\sin \theta\\0&1&0\\-\sin\theta&0&\cos\theta\end{array}\right)\left(\begin{array}{}x_{1}\\x_{2}\\x_{3}\end{array}\right)$

$\:$
##### Rotacija oko ose $\mathrm{O}x_{3}$ za ugao $\psi$
$[\mathcal{R}_{\mathrm{O}x_{3}}(\psi)]_{e}=R_{\mathrm{O}x_{3}}(\psi)=\left(\begin{array}{}\cos\psi&-\sin\psi&0\\\sin\psi&\cos\psi&0\\0&0&1\end{array}\right)$
![[afina preslikavanja 3.3 geo.png]]

##### Formula Rodrigeza
**Teorema**. Matrica $\big[$ rotacije za ugao $\varphi$ oko prave $p_{0}$ koja sadrži koordinatni početak $\big]$ u pozitivnoj bazi $e$ je
$\boxed{[\mathcal{R}_{p_{0}}(\varphi)]_{e}=R_{p_{0}}(\varphi)=pp^{\rm T}+\cos\varphi\big(E-pp^{\rm T}\big)+\sin\varphi\cdot p_{\times}}$,
gde je $p$ <u>jedinični</u> vektor pravca prave $p_{0}$,
$p_{\times}$ je matrica vektorskog množenja $p$ sa nekim vektorom
> $p_{\times}(x):=p\times x$
> Formiramo matricu $p_{\times}$
> $p_{\times}(e_{1})=p\times e_{1}=(p_{1}\,e_{1}+p_{2}\,e_{2}+p_{3}\,e_{3})\times e_{1}=-p_{2}\,e_{3}+p_{3}\,e_{2}$
> $p_{\times}(e_{2})=p\times e_{2}=(p_{1}\,e_{1}+p_{2}\,e_{2}+p_{3}\,e_{3})\times e_{2}=p_{1}\,e_{3}-p_{3}\,e_{1}$
> $p_{\times}(e_{3})=p\times e_{3}=(p_{1}\,e_{1}+p_{2}\,e_{2}+p_{3}\,e_{3})\times e_{3}=-p_{1}\,e_{2}+p_{2}\,e_{1}$
> $p_{\times}=\left(\begin{array}{}0&-p_{3}&p_{2}\\p_{3}&0&-p_{1}\\-p_{2}&p_{1}&0\end{array}\right)$

$\:$
Rotacija oko prave $p$ koja sadrži tačku $P$ i paralelna je pravoj $p_{0}$:
$\mathcal{R}_{p}(\varphi)=\mathcal{T}_{\overrightarrow{\rm OP}}\circ\mathcal{R}_{p_{0}}(\varphi)\circ\mathcal{T}_{\overrightarrow{\rm PO}}$


### Refleksija u $\mathbb{E}^{3}$
**Teorema**. Matrica $\big[$ refleksije u odnosu na ravan $\alpha$ koja sadrži koordinatni početak $\big]$ u pozitivnoj bazi $e$ je
$\boxed{[\mathcal{S}_{\alpha}]_{e}=S_{\alpha}=E - 2nn^{\rm T}}$,
gde je $n$ <u>jedinični</u> vektor normale na ravan $\alpha$

Rotacija u odnosu na ravan $\beta$ koja sadrži tačku $B$ i paralelna je ravni $\alpha$:
$\mathcal{S}_{\beta}=\mathcal{T}_{\overrightarrow{\rm OB}}\circ\mathcal{S}_{\alpha}\circ\mathcal{T}_{\overrightarrow{\rm BO}}$


### Prva Ojlerova teorema
**Teorema**. Svako kretanje u $\mathbb{E}^{3}$ sa fiksnom tačkom $O'$ je rotacija za ugao $\varphi$ oko neke prave $p$ koja sadrži $O'$.
> Objašnjenje:
> kretanje: $A\,A^{\rm T}=A^{\rm T}A=E\quad$ i $\quad \det A=1$
> 
> $\lambda_{1},\,\lambda_{2},\,\lambda_{3}\in\mathbb{C}$ su sopstvene vrednosti od $A$.
> $1=\det A = \lambda_{1}\,\lambda_{2}\,\lambda_{3}$
> ...
> Bar jedna sopstvena vrednost je jednaka $1$.
> Odakle, iz jednakosti $A\,v=\lambda\,v$  imamo $A\,v=v$,
> tj. $v$ je vektor koji se ne menja pri rotaciji, što znači da je takvo kretanje rotacija oko prave koja sadrži $O'$ i čiji je vektor pravca $v$.
> ___
> Tražimo $v$ iz sistema zadatog $(A - E)v=\mathbf{0}$ $\quad$ $(\lambda=1)$
> 
> Tražimo $\varphi$:
> treba preslikati neki vektor $u$ koji je ortogonalan na $v$ (na primer jedna od vrsta od matrice $A-E$) u vektor $A\,u$. Koristeći skalarni proizvod dobijamo $\begin{align}|\varphi|=\arccos\frac{u\circ A\,u}{||u||\cdot||A\,u||}\end{align}$. Znak $\varphi$ određujemo tako što tražimo pozitivnost trojke $[v,\,u,\,Au]$: ako je pozitivna traženi ugao je $\varphi$, ako je negativna — $(2\pi-\varphi)$.

$\:$
### Druga Ojlerova teorema
**Teorema**. Svako kretanje $f$ u $\mathbb{E}^{3}$ koje čuva koordinatni početak moguće predstaviti kao tri sopstvene (u odnosu na sopstveni koordinatni sistem ali sa istim koordinatnim početkom) rotacije.

$f=\mathcal{R}_{\mathrm{O}x''_{1}}(\varphi)\circ\mathcal{R}_{\mathrm{O}x'_{2}}(\theta)\circ\mathcal{R}_{\mathrm{O}x_{3}}(\psi)$
gde je $\mathrm{O}x'_{2}$ os $\mathrm{O}x_{2}$ posle prve rotacije;  $\mathrm{O}x''_{3}$ je os $\mathrm{O}x_{3}$ posle dve rotacije.

Tejt-Brajanoni uglovi: $\psi,\,\varphi\in[0,\,2\pi),\ \theta\in\left[ -\frac{\pi}{2},\,\frac{\pi}{2} \right]$


![[afina preslikavanja 4 geo.gif]]

U svetskom sistemu:
$[f]_{e}=[\mathcal{R}_{\mathrm{O}x''_{1}}(\varphi)\circ\mathcal{R}_{\mathrm{O}x'_{2}}(\theta)\circ\mathcal{R}_{\mathrm{O}x_{3}}(\psi)]_{e}=R_{x_{3}}(\psi)\,R_{x_{2}}(\theta)\,R_{x_{1}}(\varphi)$



### [[Kvaternion]]


