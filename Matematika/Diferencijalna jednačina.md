#fax #math #a3 [deo [[Analiza|analize]]]
$\:$

**Def**. **Diferencijalna jednačina** je jednačina u kojoj je nepoznata funkcija $f$, a u kojoj se pojavljuju izvodi funkcije $f$; 
- ako je $f$ funkcija jedne promenljive, tada se diferencijalna jednačina naziva **običnom**;
- ako je $f$ funkcija više promenljivih (pa se u jednačini pojavljuju parcijalni izvodi), tada se diferencijalna jednačina zove **parcijalnom**.

**Def**. **Red** diferencijalne jednačine je red najvećeg izvoda koji se u njoj pojavljuje.

> Obična diferencijalna jednačina reda $n$, u kojoj je nepoznata fja $y:\ \mathbb{R}\to\mathbb{R}$, ima oblik $F(x,\,y,\,y',\,\dots,\,y^{(n)})=0$.
> Ali češće ima oblik $y^{(n)}=\varphi(x,\,y,\,y',\,\dots,\,y^{(n-1)})$

Rešiti (naći opšte rešenje) diferencijalnu jednačinu znači odrediti sve funkcije $f$ koje je zadovoljavaju.


### DJ prvog reda (neki slučajevi)
Naći sva rešenja jedačine $F(x,\,y,\,y')=0$

Ako za dati $x_{0},\,y_{0}\in\mathbb{R}$ tražimo neko rešenje $y$ koje zadovoljava i jednačinu $F(x,\,y,\,y')=0$ i uslov $y_{0}=y(x_{0})$, onda se takav problem zove **Košijev problem**.

#### Razdvajanje promenljivih
$y'=f(x)\,g(y)$

$\begin{align}\frac{d y}{dx}=f(x)\,g(y)\quad\Rightarrow\quad\frac{dy}{g(y)}=f(x)\,dx\quad\Rightarrow\quad\int\frac{dy}{g(y)}= \int f(x) \, dx\end{align}$

uz proveru da li jeste ili nije $g(y)=0$ rešenje 
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
($y\equiv0$ je uvek rešenje za $\alpha>0$)

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

### Linearna DJ višeg reda (LDJ)
**Def**. **Linearna DJ** je jednačina oblika $y^{(n)}+a_{n-1}(x)\,y^{(n-1)}+\dots+a_{1}(x)\,y+a_{0}(x)\,y=b(x)$
Ako je $b(x)\equiv0$, onda je LDJ **homogena**.

#### Homogena LDJ
**Teorema**. Skup rešenja homogene LDJ $y^{(n)}+a_{n-1}(x)\,y^{(n-1)}+\dots+a_{1}(x)\,y+a_{0}(x)\,y=0$ čine $n$-dimenzioni [[Vektorski prostor|vektorski prostor]]. $\big\{y_{1}(x),\ y_{2}(x),\ \dots,\ y_{n}(x)\big\}$ je baza tog prostora akko
— $y_{i}$ je rešenje jednačine $\forall i=\overline{1,n}$
— $W(y_{1},\,y_{2},\,\dots,\,y_{n})=\left|\begin{array}{}y_{1}&y_{2}&\dots&y_{n}\\y'_{1}&y'_{2}&\dots&y'_{n}\\\dots&\dots&\dots&\dots\\y^{(n-1)}_{1}&y^{(n-1)}_{2}&\dots&y^{(n-1)}_{n}\end{array}\right|\ne0$
(**determinanta Vronskog** nije jednaka $0$)

**Def**. Baza prostora rešenja homogene LDJ zove se fundamentalni sistem rešenja homogene LDJ.

Ako je $\big\{y_{1}(x),\ y_{2}(x),\ \dots,\ y_{n}(x)\big\}$ fundamentalni sistem rešenja, onda su sva rešenja homogene LDJ oblika 
$y(x)=c_{1}\,y_{1}(x)+c_{2}\,y_{2}(x)+\dots+c_{n}\,y_{n}(x),\quad c_{i}\in\mathbb{C}\ \ \forall i=\overline{1,n}$

#### Homogena LDJ sa konstantnim koeficijentima 
$y^{(n)}+a_{n-1}\,y^{(n-1)}+\dots+a_{1}\,y+a_{0}\,y=0,\quad a_{i}\in\mathbb{R}\ \ \forall i=\overline{0,n\!-\!1}$

Neka je $y(x)=e^{\lambda x}$ rešenje jednačine, tad $y^{(i)}(x)=\lambda^{i}e^{\lambda x},\ \ \forall i=\overline{1,n}$
ubacujemo u jednačinu $\lambda^{n}e^{\lambda x}+a_{n-1}\lambda^{n-1}e^{\lambda x}+\dots+a_{1}\lambda e^{\lambda x}+a_{0}e^{\lambda x}=0$
podelimo sa $e^{\lambda}\ne 0$, dobijamo karakterističnu jednačinu 
$\boxed{\lambda^{n}+a_{n-1}\lambda^{n-1}+\dots+a_{1}\lambda+a_{0}=0}$
Znamo da ova jednačina ima $n$ nula (uključujući kompleksne i ponavljajuće).
<!-- 1. Realna nula $\lambda\in \mathbb{R}$
   tad je odgovarajuće rešenje
   $y(x)=e^{\lambda x}$
   $\:$
\2. Par kompleksno-konjugovanih nula $\lambda_{1}=\alpha+i\beta$ $\:$ i $\:$ $\lambda_{2}=\alpha-i\beta$
   tad su odgovarajuća rešenja 
   $y(x)=e^{\lambda_{1} x}=e^{\alpha x}e^{i\beta x}=e^{\alpha x} \big(\!\cos(\beta x)+i\sin(\beta x)\big)$
   $y(x)=e^{\lambda_{2} x}=e^{\alpha x}e^{-i\beta x}=e^{\alpha x} \big(\!\cos(\beta x)-i\sin(\beta x)\big)$
   $\:$
   Ovim rešenjima su ekvivalentna rešenja (što jedan, što drugi par generiše isti VP):
   $y(x)=e^{\alpha x}\cos(\beta x)$
   $y(x)=e^{\alpha x} \sin(\beta x)$
   $\:$
. -->
1. Realna nula $\lambda\in \mathbb{R}$ pojavljuje $k$ puta, tad su odgovarajuća rešenja
   $\begin{array}{}y(x)=e^{\lambda x},& y(x)=xe^{\lambda x},& y(x)=x^{2}e^{\lambda x},&\dots,& y(x)=x^{k-1}e^{\lambda x}\end{array}$
   $\:$
2. Par kompleksno-konjugovanih nula $\lambda=\alpha\pm i\beta$ pojavljuje $k$ puta, tad su odgovarajuća rešenja
   $\begin{array}{}y(x)=e^{\alpha x}\cos(\beta x),& y(x)=xe^{\alpha x}\cos(\beta x),&\dots,& y(x)=x^{k-1}e^{\alpha x}\cos(\beta x)\\y(x)=e^{\alpha x}\sin(\beta x),& y(x)=xe^{\alpha x}\sin(\beta x),&\dots,& y(x)=x^{k-1}e^{\alpha x}\sin(\beta x)\end{array}$

$\:$
Ako su $y_{1}(x),\ y_{2}(x),\ \dots,\ y_{n}(x)$ tako dobijana rešenja, onda su sva rešenja oblika $y(x)=c_{1}\,y_{1}(x)+c_{2}\,y_{2}(x)+\dots+c_{n}\,y_{n}(x),\quad c_{i}\in\mathbb{C}\ \ \forall i=\overline{1,n}$

#### Nehomogena LDJ sa konstantnim koeficijentima
$y^{(n)}+a_{n-1}\,y^{(n-1)}+\dots+a_{1}\,y+a_{0}\,y=b(x),\quad a_{i}\in\mathbb{R}\ \ \forall i=\overline{0,n\!-\!1}$

**Stav**. Neka je $y_{0}$ neko (konkretno) proizvoljno rešenje ove jednačine.
$y$ je rešenje ove jednačine akko je $y-y_{0}$ rešenje odgovarajuće homogene LDJ
>  Dokaz: značimo levi deo jednačine sa $L(y)$, jasno je da je $L$ linearna po $y$.
>  $y$ je rešenje ove jednačine $\quad\Leftrightarrow\quad L(y)=b(x)$
>  $\xLeftrightarrow{y_{0} \text{ je isto rešenje, tj. }b(x)=L(y_{0})}\quad L(y)=L(y_{0})\quad\Leftrightarrow\quad L(y-y_{0})=0$
>  $\Leftrightarrow\quad$ $y-y_{0}$ je rešenje odgovarajuće homogene LDJ

$\:$
Stoga, rešenje nehomogene LDJ je oblika
$\boxed{y=y_{\text{hom.}}+y_{0}}$, gde je $y_{\text{hom.}}$ rešenje odgovarajuće homogene LDJ, a $y_{0}$ je bilo koje konkretno rešenje nehomogene LDJ.

Tražimo $y_{0}$:
 - Ako $b(x)=P_{m}(x)\, e^{\lambda x}$, gde je $P_{m}$ polinom stepena $m$ i $\lambda\in \mathbb{R}$ je $k$-struka nula ($k:=0$ ako nije nula) karakteristične jednačine odgovarajuće homogene LDJ.
Tada $y_{0}=R_{m}(x)\, x^{k}\, e^{\lambda x}$, polinom $R_{m}$ se dobija ubacivanjem $y_{0}$ u polaznu DJ.
$\:$
 - Ako $b(x)=\big(P_{m}(x)\cos (\beta x)+Q_{m}(x)\sin(\beta x)\big) \,e^{\alpha x}$, gde su $P_{m}$ i $Q_{m}$ polinomi stepena najviše $m$ i $\alpha+ i \beta$ je $k$-struka nula ($k:=0$ ako nije nula) karakteristične jednačine odgovarajuće homogene LDJ.
Tada $y_{0}=\big(R_{m}(x)\cos (\beta x)+S_{m}(x)\sin(\beta x)\big)\, x^{k}\, e^{\alpha x}$, polinomi $R_{m}$ i $S_{m}$ se dobijaju ubacivanjem $y_{0}$ polaznu DJ.