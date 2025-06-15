#fax #math #a3 [deo [[Analiza|analize]]]
$\:$

**Def**. **Diferencijalna jednačina** je jednačina u kojoj je nepoznata funkcija $f$, a u kojoj se pojavljuju izvodi funkcije $f$; 
- ako je $f$ funkcija jedne promenljive, tada se diferencijalna jednačina naziva **običnom**;
- ako je $f$ funkcija više promenljivih (pa se u jednačini pojavljuju parcijalni izvodi), tada se diferencijalna jednačina zove **parcijalnom**.

**Def**. **Red** diferencijalne jednačine je red najvećeg izvoda koji se u njoj pojavljuje.

> Obična diferencijalna jednačina reda $n$, u kojoj je nepoznata fja $y:\ \mathbb{R}\to\mathbb{R}$, ima oblik $F(x,\,y,\,y',\,\dots,\,y^{(n)})=0$.
> Ali češće ima oblik $y^{(n)}=\varphi(x,\,y,\,y',\,\dots,\,y^{(n-1)})$

Rešiti (naći opšte rešenje) diferencijalnu jednačinu znači odrediti sve funkcije $f$ koje je zadovoljavaju.

### DJ prvog reda — slučajevi koji se neposredno rešavaju
$F(x,\,y,\,y')=0$

#### Razdvajanje promenljivih
$y'=f(x)\,g(y)$

$\begin{align}\frac{d y}{dx}=f(x)\,g(y)\quad\Rightarrow\quad\frac{dy}{g(y)}=f(x)\,dx\quad\Rightarrow\quad\int\frac{dy}{g(y)}= \int f(x) \, dx\end{align}$
#### Linearna DJ prvog reda (LDJ1)
$y'+P(x)y=Q(x)$
- množimo jednačinu sa $u(x)$ takvim da levi deo jednačine bude oblika $y'u+yu'$,
  tj. $\begin{align}u'=u\,P\quad\Rightarrow\quad \frac{du}{u}=Pdx\quad\Rightarrow\quad \ln u=\int P \, dx\quad\Rightarrow\quad u=e^{\int P \, dx}\end{align}$
  (biramo bilo koju primitivnu od $P$)
- Sad imamo 
   $\begin{align}(yu)'=u\,Q\quad\Rightarrow\quad yu=\int u\,Q \, dx \quad\Rightarrow\quad y=\frac{\begin{align}\int u\,Q \, dx\end{align}}{u}\end{align}$ 
   (tu je bitna konstanta pri rešavanju integrala)

#### Bernulijeva DJ
$y'+P(x)y=Q(x)y^{\alpha}$ (ima smisla razlikovati za $\alpha\ne0,\,1$)

Množimo sa $y^{-\alpha}$: $\quad$ $y'y^{-\alpha}+P(x)y^{1-\alpha}=Q(x)$
Smena $z=y^{1-\alpha}$, tada $z'=(1-\alpha)y^{-\alpha}y'$
jednačina postaje  $\begin{align}\frac{1}{1-\alpha}z'+P(x)z=Q(x)\end{align}$
odakle dobijamo LDJ1 po $z$: $\quad$ $z'+(1-\alpha)P(x)z=(1-\alpha)Q(x)$ 

#### Totalni diferencijal 
$M(x,\,y)+N(x,\,y)y'=0$

Ako postoji $f(x,\,y)$ takva da $M=f'_{x}$ $\:$ i $\:$ $N=f'_{y}$
onda $\begin{align}\bigg(f\big(x,\,y(x)\big)\bigg)'_{x}=\Big(f'_{x}\quad f'_{y}\Big)\left(\begin{array}{}1\\y'\end{array}\right)=f'_{x}+f'_{y}\,y'=M+Ny'=0\end{align}$
tj. tada je implicitno rešenje date jednačine $f\big(x,\,y(x)\big)=c$
> Napomena:
> Pomnožimo polaznu jednačinu sa $dx$
> Imamo, $M(x,\,y)dx+N(x,\,y)dy=0$
> Izraz sa leve strane jednačine zove se **totalnim diferencijalom**.
> > $df=f'_{x}dx+f'_{y}dy$
> 
>  Ako postoji $f$, koje zadovoljava $M=f'_{x}$ $\:$ i $\:$ $N=f'_{y}$ i koje je dva puta neprekidno diferencijabilna, treba da važi $f''_{xy}=f'_{yx}$, a samim tim i $M'_{y}=N'_{x}$ (nužni uslov postojanja rešenja).

$\:$
#### Smena $\begin{align}z=\frac{y}{x}\end{align}$
$\begin{align}y'=f\left( \frac{y}{x} \right)\end{align}$

Smena $\begin{align}z=\frac{y}{x}\end{align}$, tada $y'=z'x+z$
jednačina postaje $z'x+z=f(z)$
dobijamo jednačinu $\begin{align}z'=\frac{f(z)-z}{x}\end{align}$, koju rešavamo razdvajanjem promenljivih

#### Smena $\begin{align}z=ax+by+c\end{align}$
$y'=f(ax+by+c)$

Smena $z=ax+by+c$, tada $\begin{align}y'=\frac{z'-a}{b}\end{align}$
jednačina postaje $\begin{align}\frac{z'-a}{b}=f(z)\end{align}$
dobijamo jednačinu $z'=b\,f(z)+a$, koju rešavamo razdvajanjem promenljivih

### Linearna DJ reda $n$ (LDJ$n$)