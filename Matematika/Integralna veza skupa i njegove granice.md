#fax #math #a3 [deo poglavlja [[Krivolinijski integral|"krivolinijski integral"]] i [[Površinski integral|"površinski integral"]]]
$\:$

> Napomena: [[Konzervativno vektorsko polje]]

$\:$
### Grinova formula
 **Teorema** (Grinova formula). Neka je $D\subseteq\mathbb{R}^{2}$ [[Vrste tačaka u odnosu na neki skup. Ograničenost i kompaktnost#^3969f8|kompaktan]] i takav da mu je granica $\mathcal{C}=\partial D$ deo po deo glatka kriva. Neka je $\mathbf{f}=(P,\,Q):\ D\to\mathbb{R}^{2}$ vektorsko polje, takvo da su $P,\,Q,\,P'_{y},\,Q'_{x}$ neprekidni na $\mathcal{C}$. I neka je $\mathcal{C}$ orijentisana tako da $D$ ostaje sa leve strane. Tada
 $\begin{align}\oint_{\mathcal{C}} \mathbf{f} \cdot d\mathbf{r}=\iint_{D} (Q'_{x}-P'_{y}) \, dxdy\end{align}$
 > Dokaz: 
 > Dokazaćemo formulu u slučaju $\mathcal{C}=\mathcal{C}_{1}\cup\mathcal{C}_{2}=\mathcal{C}_{3}\cup\mathcal{C}_{4}$, gde je
 > $\mathcal{C}_{1}$ grafik fje $y=f(x),\ \ x\in[a,\,b]$
 > $\mathcal{C}_{2}$ grafik fje $y=g(x),\ \ x\in[a,\,b]$
 > $\mathcal{C}_{3}$ grafik fje $x=h(y),\ \ x\in[c,\,d]$
 > $\mathcal{C}_{4}$ grafik fje $x=k(y),\ \ x\in[c,\,d]$
 > ![[grinova formula slika1.png]]
 > 
 > Neka je $\mathcal{C}$ parametrizovana sa $\mathbf{r}=(x,\,y):\ [p,\,q]\to\mathbb{R}^{2}$
 > 
 > Iz [[Krivolinijski integral#^0ddf32|teoreme]]: $\begin{align}\oint_{\mathcal{C}} \mathbf{f}(x,\,y) \cdot d\mathbf{r} = \int_{p}^{q} P\Big(x(t),\,y(t)\Big)x'(t) \, dt+\int_{p}^{q} Q\Big(x(t),\,y(t)\Big)y'(t) \, dt\end{align}$
 > 
 > Treba pokazati:
 > - $\begin{align}\int_{p}^{q} P\Big(x(t),\,y(t)\Big)x'(t) \, dt = -\iint_{D} P'_{y}(x,\,y) \, dxdy \end{align}$
 > - $\begin{align}\int_{p}^{q} Q\Big(x(t),\,y(t)\Big)y'(t) \, dt = \iint_{D} Q'_{x}(x,\,y) \, dxdy \end{align}$
 >   
 > Dokažemo prvu jednačinu, druga se dokazuje analogno.
 > Neka je $\mathbf{r}(0)=\big(a,\,f(a)\big)$ i $\mathbf{r}(s)=\big(b,\,f(b)\big)$, tada $\mathcal{C}_{1}=\mathbf{r}\big[[p,\,s]\big]$ i $\mathcal{C}_{2}=\mathbf{r}\big[[s,\,q]\big]$
 > (smena $t=t+\mathrm{const}$ ne utiče ne levi deo jednačine)
 > $\begin{align}\int_{p}^{q} P\Big(x(t),\,y(t)\Big)x'(t) \, dt = \int_{p}^{s} P\Big(x(t),\,y(t)\Big)x'(t) \, dt + \int_{s}^{q} P\Big(x(t),\,y(t)\Big)x'(t) \, dt =\end{align}$
 > > u prvom integralu smena $x=x(t)$, tada $y(t)=f(x)$;
 > > u drugom integralu smena $x=x(t)$, tada $y(t)=g(x)$.
 > 
 > $\begin{align}= \int_{a}^{b} P\Big(x,\,f(x)\Big) \, dx + \int_{b}^{a} P\Big(x,\,g(x)\Big) \, dx =\int_{a}^{b} \bigg(P\Big(x,\,f(x)\Big)-P\Big(x,\,g(x)\Big)\bigg) \, dx=\end{align}$
 > 
 > > Njutn-Lajbnic: $\begin{align}\int_{g(x)}^{f(x)} P'_{y}(x,\,y)\,dy=P\Big(x,\,f(x)\Big)-P\Big(x,\,g(x)\Big)\end{align}$
 > > 
 >
 > $\begin{align}= \int_{a}^{b} \int_{g(x)}^{f(x)} P'_{y}(x,\,y)\,dydx=-\iint_{D} P'_{y}(x,\,y) \, dxdy\end{align}$
 >___ 
 > Komplikovanije figure delimo na više figura vertikalnim/horizontalnim linijama, tako da svaka seče granicu neparan broj puta
 > ![[grinova formula slika2.png]]
 > Treba pokazati (kao i odgovarajuću jednačinu sa $Q$ i horizontalnim linijama):
 > - $\begin{align}\int_{p}^{q} P\Big(x(t),\,y(t)\Big)x'(t) \, dt = -\iint_{D_{1}} P'_{y}(x,\,y) \, dxdy -\iint_{D_{2}} P'_{y}(x,\,y) \, dxdy-\dots-\iint_{D_{n}} P'_{y}(x,\,y) \, dxdy\end{align}$
 >
 > Levi deo jednačine se ne menja od dodavanja vertikalnih linija, a u desnom jer svaki deo linije se prolazi paran broj puta (u svaki prolaz u jednom smeru ima i prolaz u suprotnom), odgovarajući integrali će se skratiti i vertikalne linije neće uticati ni na desni deo jednačine.
 
 $\:$
### Stoksova formula
**Teorema** (Stoksova formula). Neka je $\mathcal{C}$ glatka deo po deo neprekidna zatvorena kriva, koja je granica površi $\mathcal{S}$, $\:$ $\mathcal{C}=\partial D$. $\mathcal{S}$ je zatvorena površ parametrizovana regularnom parametrizacijom. $\mathcal{C}$ i $\mathcal{S}$ su orijentisane tako da $\mathcal{S}$ ostaje sa leve strane od $\mathcal{C}$, gledajući sa strane $\mathcal{S}$ izabrane parametrizacijom $\mathbf{r}$. Neka je $\mathbf{f}=(P,\,Q,\,R)$ neprekidno (zajedno sa parcijalnim izvodima) vektorsko polje. Tada
$\begin{align}\oint_{\mathcal{C}} \mathbf{f} \cdot d\mathbf{r}=\iint_{\mathcal{S}} (\nabla\times \mathbf{f}) \cdot d\mathbf{S}\end{align}$
 > Dokaz: 
 > Prvo razmotrimo $\mathbf{f}=(P,\,0,\,0)$, analogno se dokazuje za $(0,\,Q,\,0)$ $\!$ i  $\!$ $(0,\,0,\,R)$.
 > Neka je $D\subseteq\mathbb{R}^{2}$, takav da $\mathbf{r}[D]=\mathcal{S}$, i neka je $L\subseteq D$, takav da $\mathbf{r}[L]=\mathcal{C}$.
 > Parametrizujemo $L$ sa $\big(u(t),\,v(t)\big)$, tad je $\mathcal{C}$ data sa 
 > $\mathbf{r}\big(u(t),\,v(t)\big)=\Big(x\big(u(t),\,v(t)\big),\ y\big(u(t),\,v(t)\big),\ z\big(u(t),\,v(t)\big)\Big)=\mathbf{w}(t),\quad t\in[a,\,b]$
 > 
 > $\begin{align}\oint_{\mathcal{C}} \mathbf{f} \cdot d\mathbf{r}=\int_{a}^{b} (\mathbf{f}\circ \mathbf{w})(t)\cdot \mathbf{w}'(t)\,dt=\end{align}$
 > > $\mathbf{w}'(t)=\left(\begin{array}{}x'_{u}&x'_{v}\\y'_{u}&y'_{v}\\z'_{u}&z'_{v}\end{array}\right)\left(\begin{array}{}u'\\v'\end{array}\right)=\left(\begin{array}{}x'_{u}u'+x'_{v}v'\\y'_{u}u'+y'_{v}v'\\z'_{u}u'+z'_{v}v'\end{array}\right)$
 > 
 > $\begin{align}=\int_{a}^{b} P\Big(x\big(u(t),\,v(t)\big),\,y\big(u(t),\,v(t)\big),\,z\big(u(t),\,v(t)\big)\Big)\, (x'_{u}u'+x'_{v}v')\,dt=\end{align}$
 >  $\begin{align}=\oint_{L} P\Big(x\big(u,\,v\big),\,y\big(u,\,v\big),\,z\big(u,\,v\big)\Big)\, x'_{u}\,du+P\Big(x\big(u,\,v\big),\,y\big(u,\,v\big),\,z\big(u,\,v\big)\Big)\,x'_{v}\,dv=\end{align}$
 >  > [[Integralna veza skupa i njegove granice#Grinova formula|Grinova formula]]
 > 
 > $\begin{align}=\iint_{D} \bigg(\Big(P\big(x(u,\,v),\,y(u,\,v),\,z(u,\,v)\big)\,x'_{v}\Big)'_{u}-\Big(P\big(x(u,\,v),\,y(u,\,v),\,z(u,\,v)\big)\, x'_{u}\Big)'_{v}\bigg)dudv=\end{align}$
 > $\begin{align}=\iint_{D} \Big(P'_{u}\,x'_{v}+P\,x''_{vu} -P'_{v}\,x'_{u}-P\,x''_{uv} \Big)dudv=\iint_{D}\Big( P'_{u}\,x'_{v} -P'_{v}\,x'_{u}\Big)dudv=\end{align}$
 > > $P'_{u}\big(x(u,\,v),\ y(u,\,v),\ z(u,\,v)\big)=\Big(P'_{x}\quad P'_{y}\quad P'_{z}\Big)\left(\begin{array}{}x'_{u}\\y'_{u}\\z'_{u}\end{array}\right)=P'_{x}\,x'_{u}+ P'_{y}\,y'_{u}+ P'_{z}z'_{u}$
 > 
 > $\begin{align}=\iint_{D} \Big(P'_{x}\,x'_{u}\,x'_{v}+ P'_{y}\,y'_{u}\,x'_{v}+ P'_{z}z'_{u}\,x'_{v}-P'_{x}\,x'_{v}\,x'_{u}- P'_{y}\,y'_{v}\,x'_{u}- P'_{z}z'_{v}\,x'_{u} \Big)dudv=\end{align}$
 > $\begin{align}=\iint_{D} \Big(P'_{y}\cdot\big(y'_{u}\,x'_{v}-y'_{v}\,x'_{u}\big)+P'_{z}\cdot\big(z'_{u}\,x'_{v}-z'_{v}\,x'_{u} \big)\Big)dudv=\end{align}$
 > $\begin{align}=\iint_{\mathcal{S}} P'_{y}\cdot dydx+P'_{z}\cdot dzdx=\iint_{\mathcal{S}} \Big(0,\ P'_{x},\ P'_{y}\Big)\cdot d\mathbf{S}=\iint_{\mathcal{S}} (\nabla\times \mathbf{f}) \cdot d\mathbf{S}\end{align}$
>
> Jer su oba (levi i desni deo jednačine) integrala linearni po $\mathbf{f}$, bilo koju $\mathbf{f}$ možemo predstaviti kao $\mathbf{f}=(P,\,Q,\,R)=(P,\,0,\,0)+(0,\,Q,\,0)+(0,\,0,\,R)$, i jer smo pokazali da jednačina važi za svaki od sabiraka, jednačina važi za bilo koje polje $\mathbf{f}$.

$\:$
### Gausova formula
**Teorema** (Gausova formula). Neka je regularna površ $\mathcal{S}=\partial T$ granica kompaktog skupa $T \subseteq \mathbb{R}^{3}$, $\mathcal{S}$ je parametrizovana po spoljnom delu $T$ i $\mathbf{f}$ neprekidno (zajedno sa parcijalnim izvodima) vektorsko polje na $T$. Tada
$\begin{align}\iint_{\mathcal{S}}  \mathbf{f} \cdot d\mathbf{S}=\iiint_{T} \nabla\cdot\mathbf{f} \, dxdydz \end{align}$
> Dokaz: 
> Dokazaćemo formulu u slučaju $\mathcal{S}=\mathcal{P}_{1}\cup\mathcal{Q}_{1}=\mathcal{P}_{2}\cup\mathcal{Q}_{2}=\mathcal{P}_{3}\cup\mathcal{Q}_{3}$, gde su
 > $\mathcal{P}_{1}=\Big\{(x,\,y,\,z)\ \Big|\ z=f_{1}(x,\,y)\Big\}\ \ \ \text{i} \ \ \ \mathcal{Q}_{1}=\Big\{(x,\,y,\,z)\ \Big|\ z=g_{1}(x,\,y)\Big\},\quad (x,\,y)\in D_{1}$
 > $\mathcal{P}_{2}=\Big\{(x,\,y,\,z)\ \Big|\ x=f_{2}(y,\,z)\Big\}\ \ \ \text{i} \ \ \ \mathcal{Q}_{2}=\Big\{(x,\,y,\,z)\ \Big|\ x=g_{2}(y,\,z)\Big\},\quad (y,\,z)\in D_{2}$
 > $\mathcal{P}_{3}=\Big\{(x,\,y,\,z)\ \Big|\ y=f_{3}(x,\,z)\Big\}\ \ \ \text{i} \ \ \ \mathcal{Q}_{3}=\Big\{(x,\,y,\,z)\ \Big|\ y=g_{3}(x,\,z)\Big\},\quad (x,\,z)\in D_{3}$
>
> Tada, $\begin{align}T&=\Big\{(x,\,y,\,z)\ \Big|\ (x,\,y)\in D_{1},\ \ f_{1}(x,\,y)\leqslant z\leqslant g_{1}(x,\,y)\Big\}=\\&=\Big\{(x,\,y,\,z)\ \Big|\ (y,\,z)\in D_{2},\ \ f_{2}(y,\,z)\leqslant x\leqslant g_{2}(y,\,z)\Big\}=\\&=\Big\{(x,\,y,\,z)\ \Big|\ (x,\,z)\in D_{3},\ \ f_{3}(x,\,z)\leqslant y\leqslant g_{3}(x,\,z)\Big\}\end{align}$ 
>
> Neka $\mathbf{f}=(P,\,Q,\,R)$
>
> $\begin{align}\iint_{\mathcal{S}} \mathbf{f} \cdot d\mathbf{S} =\iint_{\mathcal{S}} P\,dydz + Q\,dzdx + R\,dxdy \end{align}$
> $\begin{align}\iiint_{T} \nabla\cdot\mathbf{f}\, dxdydz =\iiint_{T} P'_{x}\, dxdydz+\iiint_{T}Q'_{y}\, dxdydz+\iiint_{T} R'_{z}\, dxdydz\end{align}$
> 
> Treba pokazati:
> - $\begin{align}\iint_{\mathcal{S}} P\,dydz=\iiint_{T} P'_{x}\, dxdydz\end{align}$
> - $\begin{align}\iint_{\mathcal{S}} Q\,dzdx=\iiint_{T} Q'_{y}\, dxdydz\end{align}$
> - $\begin{align}\iint_{\mathcal{S}} R\,dxdy=\iiint_{T} R'_{z}\, dxdydz\end{align}$
>
> Pokazaćemo poslednju jednačinu, ostale dve se dokazuju analogno.
> Neka je $\mathbf{r}(u,\,v)=\big(x(u,\,v),\,y(u,\,v),\,z(u,\,v)\big),\ \ (u,\,v)\in D$ parametrizacija oblasti $T$. Pri tome $\mathcal{S}=\mathbf{r}[\partial D]$
> 
> $\begin{align}\iint_{\mathcal{S}} R\, dxdy =\iint_{\mathcal{R}_{1}} R\, dxdy+\iint_{\mathcal{Q}_{1}} R\, dxdy=\end{align}$
> > $\mathcal{S}$ je spoljašnost od $T$, stoga u $\mathcal{R}_{1}$ ("donji" deo) vektor normale usmeren "dole", a u $\mathcal{Q}_{1}$ ("gornji" deo) vektor normale usmeren "gore".
> 
> $\begin{align}=-\iint_{D_{1}} R\big(x,\,y,\,f_{1}(x,\,y)\big) \, dxdy+\iint_{D_{1}} R\big(x,\,y,\,g_{1}(x,\,y)\big) \, dxdy=\end{align}$
> $\begin{align}=\iint_{D_{1}} \bigg( R\big(x,\,y,\,g_{1}(x,\,y)\big) -R\big(x,\,y,\,f_{1}(x,\,y)\big)\bigg) dxdy=\end{align}$
>  > Njutn-Lajbnic: $\begin{align}\int_{f_{1}(x,\,y)}^{g_{1}(x,\,y)} R'_{z}(x,\,y,\,z) \, dz=R\big(x,\,y,\,g_{1}(x,\,y)\big)-R\big(x,\,y,\,f_{1}(x,\,y)\big) \end{align}$
> 
> $\begin{align}=\iint_{D_{1}}\bigg(\int_{f_{1}(x,\,y)}^{g_{1}(x,\,y)} R'_{z}(x,\,y,\,z) \, dz\bigg) dxdy=\iiint_{T} R'_{z}(x,\,y,\,z) \, dxdydz\end{align}$