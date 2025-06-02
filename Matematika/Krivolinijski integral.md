#fax #math #a3 [deo [[Analiza|analize]]]

### Podela [[Kriva i površ#Kriva u $ mathbb{R} {n}$|krive]]
Neka je $\mathcal{C}$ kriva parametrizovana sa $\mathbf{r}:\ [a,\,b]\to\mathbb{R}^{n}$ $\ \:$ i $\ \:$ neka je $(\mathcal{P},\,\xi)$ [[Određeni integral#Podela intervala|podela]] sa istaknutim tačkama intervala $[a,\,b]$, u kojoj su $t_{i},\ \ i=\overline{0,\,n}$ podeone tačke.


Tada je $\mathbf{P}=\Big\{\mathbf{r}\big[[t_{i-1},\,t_{i}]\big]\ \Big|\ i =\overline{1,\,n}\Big\}$ **podela krive** $\mathcal{C}$.

Pri tome tačke $\mathbf{x}_{i}:=\mathbf{r}(t_{i}),\ \ i=\overline{0,n}$ su podeone tačke te podele i $\lambda(\mathbf{P})=\lambda(\mathcal{P})$

$\boldsymbol{\xi}_{i}:=\mathbf{r}(\xi_{i}),\ \ \forall i=\overline{1,n}$, $\quad$ gde su $\xi_{i}$ istaknute tačke podele $\mathcal{P}$.

$(\mathbf{P},\,\boldsymbol{\xi})$ je **podela sa istaknutim tačkama krive** $\mathcal{C}$

Aproksimiramo dužinu dela krive $\mathbf{r}\big[[t_{i-1},\,t_{i}]\big]$ sa $||\mathbf{r}(t_{i})-\mathbf{r}(t_{i-1})||=||\mathbf{x}_{i}-\mathbf{x}_{i-1}||$

### Krivolinijski integral skalar-funkcije
**Def**. Neka je $f:\ \mathcal{C}\to\mathbb{R}\ \:$ i $\ \:(\mathbf{P},\,\boldsymbol{\xi})$ podela sa istaknutim tačkama krive $\mathcal{C}$. Zbir $\begin{align}\sigma(f,\,\mathbf{P},\,\boldsymbol{\xi})=\sum\limits_{i=1}^{n}||\mathbf{x}_{i}-\mathbf{x}_{i-1}||\,f(\boldsymbol{\xi}_{i})\end{align}$ je **integralna suma**.

$\:$
**Def**. Neka je $f:\ \mathcal{C}\to\mathbb{R}$. $\ \:$ $I\in\mathbb{R}$ je limes integralnih suma $\sigma(f,\,\mathbf{P},\,\boldsymbol{\xi})$ kad $\lambda(\mathbf{P})\to0$ ako
$\begin{align}\forall\varepsilon>0\quad\exists\delta>0\quad\forall\binom{(\mathbf{P},\,\boldsymbol{\xi} )\ \text{— podela sa istaknutim tačkama}}{\text{ krive }\mathcal{C}\text{ takva da } \lambda(\mathbf{P})<\delta}\quad \Big|I-\sigma(f,\,\mathbf{P},\,\boldsymbol{\xi})\Big|<\varepsilon\end{align}$
$\:$
Tada je $\begin{align}I=\int_{\mathcal{C}} f(\mathbf{x}) \, ||d\mathbf{r}|| \end{align}$ $\:$ **krivolinijski integral** (prve vrste) fje $f$ duž $\mathcal{C}$.
Ako je $\mathcal{C}$ [[Kriva i površ#^66ef03|zatvorena]] pišemo $\begin{align}I=\oint_{\mathcal{C}} f(\mathbf{x}) \, ||d\mathbf{r}|| \end{align}$.

$\:$
**Teorema**. Ako je $f$ deo po deo neprekidna i $\mathbf{r}$ je regularna parametrizacija krive $\mathcal{C}$, onda $\begin{align}\int_{\mathcal{C}} f(\mathbf{x}) \, ||d\mathbf{r}|| =\int_{a}^{b} (f\circ \mathbf{r})(t)\,||r'(t)||\, dt \end{align}$ 
> Dokaz:
> $\begin{align}\sigma(f,\,\mathbf{P},\,\boldsymbol{\xi})=\sum\limits_{i=1}^{n}||\mathbf{x}_{i}-\mathbf{x}_{i-1}||\,f(\boldsymbol{\xi}_{i})=\sum\limits_{i=1}^{n}||\mathbf{r}(t_{i})-\mathbf{r}(t_{i-1})||\,f(\mathbf{r}(\xi_{i}))=\end{align}$
> $\begin{align}=\sum\limits_{i=1}^{n}(t_{i}-t_{i-1})\Bigg|\Bigg|\frac{\mathbf{r}(t_{i})-\mathbf{r}(t_{i-1})}{t_{i}-t_{i-1}}\Bigg|\Bigg|\,(f\circ \mathbf{r})(\xi_{i})=\end{align}$ $\Big[\,$[[Teoreme o srednjoj vrednosti#^e52da5|Lagranž]], $\mu_{i}\in(t_{i-1},\,t_{i})\,\Big]=$
> $\begin{align}=\sum\limits_{i=1}^{n}(t_{i}-t_{i-1})||\mathbf{r}'(\mu_{i})||\,(f\circ \mathbf{r})(\xi_{i})\end{align}$
> 
> $\begin{align}\int_{\mathcal{C}} f(\mathbf{x}) \, ||d\mathbf{r}|| =\lim\limits_{ \lambda(\mathbf{P}) \to 0 }\sigma(f,\,\mathbf{P},\,\boldsymbol{\xi})=\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sum\limits_{i=1}^{n}(t_{i}-t_{i-1})||\mathbf{r}'(\mu_{i})||\,(f\circ \mathbf{r})(\xi_{i})=\end{align}$
> $\begin{align}=\int_{a}^{b} (f\circ \mathbf{r})(t)\,||r'(t)||\, dt \end{align}$ 

$\:$
**Def**. $||d\mathbf{r}||=||\mathbf{r}'(t)||\,dt$ je **element dužine**.

> Napomena:
> Ako razmatramo krivu $\mathcal{C}$ u $\mathbb{R}^{3}$ parametrizovanu sa $\mathbf{r}:\ [a,\,b]\to\mathbb{R}^{3}$ def. sa $\mathbf{r}(t)=\Big(x(t),\ y(t),\ z(t)\Big)$, imamo
> $\begin{align}\int_{\mathcal{C}} f(x,\,y,\,z) \, ||d\mathbf{r}||=\int_{a}^{b} f\Big(x(t),\ y(t),\ z(t)\Big) \sqrt[]{x'(t)^{2}+y'(t)^{2}+z'(t)^{2}} \, dt\end{align}$


___
Napomena: [[Riman-integrabilnost funkcija i svojstva određenog integrala#Svojstva određenog integrala|svojstva određenog integrala]]

**[[Riman-integrabilnost funkcija i svojstva određenog integrala#^cfc6a3|Stav]]**.  $f$ i $g$ su deo po deo neprekidni; $\ \ \alpha,\,\beta\in\mathbb{R}$. Tada važi
$\begin{align}\int_{\mathcal{C}}(\alpha\,f+\beta\,g)(\mathbf{x}) \, ||d\mathbf{r}|| = \alpha\int_{\mathcal{C}} f(\mathbf{x}) \, ||d\mathbf{r}||+\beta \int_{\mathcal{C}} g(\mathbf{x}) \, ||d\mathbf{r}|| \end{align}$

**Stav**.  $f$ i $g$ su deo po deo neprekidni; $\ \ \forall \mathbf{x}\in \mathcal{C}\quad f(\mathbf{x})\leqslant g(\mathbf{x})$. Tada $\begin{align}\int_{\mathcal{C}} f(\mathbf{x}) \, ||d\mathbf{r}||\leqslant \int_{\mathcal{C}} g(\mathbf{x}) \, ||d\mathbf{r}|| \end{align}$

**Stav**. $f$ je deo po deo neprekidna; krive $\mathcal{C}$ i $\mathcal{D}$ imaju samo jednu zajedničku tačku koja je kraj i jedne i druge krive. Tada
$\begin{align}\int_{\mathcal{C}\cup \mathcal{D}} f(\mathbf{x}) \, ||d\mathbf{r}|| = \int_{\mathcal{C}} f(\mathbf{x}) \, ||d\mathbf{r}|| + \int_{\mathcal{D}} f(\mathbf{x}) \, ||d\mathbf{r}||\end{align}$


**Stav**. $l(\mathcal{C})=\begin{align}\int_{\mathcal{C}} 1 \, ||d\mathbf{r}||\end{align}$ $\ \:$ je dužina krive $\mathcal{C}$

**[[Riman-integrabilnost funkcija i svojstva određenog integrala#Predstavljanje određenog integrala proizvodom|Stav]]**. 
- $f$ je deo po deo neprekidna, $\ \:$ $m=\min\limits_{\mathcal{C}} f$, $\ \:$ $M=\max\limits_{\mathcal{C}}f$. $\ \:$ Tada $\begin{align}\exists \mu\in[m,\,M]\quad \int_{\mathcal{C}} f(\mathbf{x}) \, ||d\mathbf{r}|| = \mu\cdot l(\mathcal{C}) \end{align}$
- $f$ je neprekidna. $\ \:$ Tada $\begin{align}\exists\mathbf{x}_{0}\in\mathcal{C}\quad \int_{\mathcal{C}} f(\mathbf{x}) \, ||d\mathbf{r}|| = f(\mathbf{x}_{0})\cdot l(\mathcal{C}) \end{align}$

### Krivolinijski integral vektorskog polja
**Def**. Neka je $\mathcal{C}$ kriva parametrizovana sa $\mathbf{r}:\ [a,\,b]\to\mathbb{R}^{n}$, $\ \:$ $(\mathbf{P},\,\boldsymbol{\xi})$ podela sa istaknutim tačkama te krive i $\ \:$ $\mathbf{f}:\ \mathcal{C}\to\mathbb{R}^{n}\ \:$ vektorsko polje. Zbir $\begin{align}\sigma(\mathbf{f},\,\mathbf{P},\,\boldsymbol{\xi})=\sum\limits_{i=1}^{n}(\mathbf{x}_{i}-\mathbf{x}_{i-1})\cdot\mathbf{f}(\boldsymbol{\xi}_{i})\end{align}$ je **integralna suma** ($\cdot$ je skalarni proizvod).

$\:$
**Def**. Neka je $\mathbf{f}:\ \mathcal{C}\to\mathbb{R}^{n}$. $\ \:$ $I\in\mathbb{R}$ je limes integralnih suma $\sigma(\mathbf{f},\,\mathbf{P},\,\boldsymbol{\xi})$ kad $\lambda(\mathbf{P})\to0$ ako
$\begin{align}\forall\varepsilon>0\quad\exists\delta>0\quad\forall\binom{(\mathbf{P},\,\boldsymbol{\xi} )\ \text{— podela sa istaknutim tačkama}}{\text{ krive }\mathcal{C}\text{ takva da } \lambda(\mathbf{P})<\delta}\quad \Big|I-\sigma(\mathbf{f},\,\mathbf{P},\,\boldsymbol{\xi})\Big|<\varepsilon\end{align}$
$\:$
Tada je $\begin{align}I=\int_{\mathcal{C}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{r} \end{align}$ $\:$ **krivolinijski integral** (druge vrste) fje $\mathbf{f}$ duž $\mathcal{C}$.
Ako je $\mathcal{C}$ [[Kriva i površ#^66ef03|zatvorena]] pišemo $\begin{align}I=\oint_{\mathcal{C}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{r} \end{align}$.

$\:$
**Teorema**. Neka je $\mathcal{C}$ kriva parametrizovana sa $\mathbf{r}:\ [a,\,b]\to\mathbb{R}^{n}$ $\ \:$ i $\ \:$ neka je $\mathbf{f}:\ \mathcal{C}\to \mathbb{R}^{n}$ vektorsko polje. Označimo sa $\begin{align}\mathbf{T}:=\frac{\mathbf{r}'}{||\mathbf{r}'||}\end{align}$ jedinični tangentni vektor na $\mathcal{C}$
Tada, $\begin{align}\int_{\mathcal{C}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{r} =\int_{a}^{b} (\mathbf{f}\circ\mathbf{r})(t) \cdot \mathbf{r'}(t) \, dt= \int_{\mathcal{C}} \mathbf{f}(\mathbf{x})\cdot \mathbf{T} \, ||d\mathbf{r}||\end{align}$ ^0ddf32
> Dokaz: 
> $\begin{align}\sigma(\mathbf{f},\,\mathbf{P},\,\boldsymbol{\xi})=\sum\limits_{i=1}^{n}(\mathbf{x}_{i}-\mathbf{x}_{i-1})\cdot\mathbf{f}(\boldsymbol{\xi}_{i})=\sum\limits_{i=1}^{n}(\mathbf{r}(t_{i})-\mathbf{r}(t_{i-1}))\cdot\mathbf{f}(\mathbf{r}(\xi_{i}))=\end{align}$ 
> $\begin{align}=\sum\limits_{i=1}^{n}(t_{i}-t_{i-1})\bigg(\frac{\mathbf{r}(t_{i})-\mathbf{r}(t_{i-1})}{t_{i}-t_{i-1}}\bigg)\cdot(\mathbf{f}\circ \mathbf{r})(\xi_{i})=\end{align}$ $\Big[\,$[[Teoreme o srednjoj vrednosti#^e52da5|Lagranž]], $\mu_{i}\in(t_{i-1},\,t_{i})\,\Big]=$
> $\begin{align}=\sum\limits_{i=1}^{n}(t_{i}-t_{i-1})\mathbf{r}'(\mu_{i})\cdot(\mathbf{f}\circ \mathbf{r})(\xi_{i})\end{align}$
> 
> $\begin{align}\int_{\mathcal{C}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{r} =\lim\limits_{ \lambda(\mathbf{P}) \to 0 }\sigma(\mathbf{f},\,\mathbf{P},\,\boldsymbol{\xi})=\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sum\limits_{i=1}^{n}(t_{i}-t_{i-1})\mathbf{r}'(\mu_{i})\cdot(\mathbf{f}\circ \mathbf{r})(\xi_{i})=\end{align}$
> $\begin{align}=\int_{a}^{b} (\mathbf{f}\circ \mathbf{r})(t)\cdot r'(t)\, dt =\int_{a}^{b} (\mathbf{f}\circ \mathbf{r})(t)\cdot \frac{r'(t)}{||\mathbf{r'(t)||}}||\mathbf{r}'(t)||\, dt=\int_{a}^{b} (\mathbf{f}\circ \mathbf{r})(t)\cdot \mathbf{T}(t)\, ||d\mathbf{r}||  \end{align}$ 

$\:$
> Napomena:
> Ako razmatramo krivu $\mathcal{C}$ u $\mathbb{R}^{3}$ parametrizovanu sa $\mathbf{r}:\ [a,\,b]\to\mathbb{R}^{3}$ def. sa $\mathbf{r}(t)=\Big(x(t),\ y(t),\ z(t)\Big)$ i vektorsko polje $\mathbf{f}=(P,\,Q,\,R)$, imamo
> $\begin{align}\int_{\mathcal{C}} \mathbf{f}(x,\,y,\,z) \cdot d\mathbf{r}=\int_{a}^{b} f\Big(x(t),\ y(t),\ z(t)\Big)\cdot \Big(x'(t),\ y'(t),\ z'(t)\Big) \, dt=\end{align}$
> $\begin{align}=\int_{a}^{b}\bigg( P\Big(x(t),\ y(t),\ z(t)\Big)x'(t)+Q\Big(x(t),\ y(t),\ z(t)\Big)y'(t)+R\Big(x(t),\ y(t),\ z(t)\Big)z'(t)\bigg) \, dt=\end{align}$
> $\begin{align}=\int_{\mathcal{C}}P(x,\, y,\, z)dx+Q(x,\, y,\, z)dy+R(x,\, y,\, z)dz\end{align}$

 ___
 
 **Stav**. $\alpha,\,\beta\in\mathbb{R}$. Tada važi
$\begin{align}\int_{\mathcal{C}}(\alpha\,\mathbf{f}+\beta\,\mathbf{g})(\mathbf{x}) \cdot d\mathbf{r} = \alpha\int_{\mathcal{C}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{r}+\beta \int_{\mathcal{C}} \mathbf{g}(\mathbf{x}) \cdot d\mathbf{r} \end{align}$

**Stav**. Krive $\mathcal{C}$ i $\mathcal{D}$ imaju samo jednu zajedničku tačku koja je kraj krive $\mathcal{C}$ i početak krive $\mathcal{D}$. Tada $\begin{align}\int_{\mathcal{C}\cup \mathcal{D}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{r} = \int_{\mathcal{C}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{r} + \int_{\mathcal{D}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{r}\end{align}$
___
Krivu $\mathcal{C}$ možemo orijentisati na dva načina: ako je $\mathbf{r}:\ [a,\,b]\to\mathbb{R}^{n}$ jedna parametrizacija krive $\mathcal{C}$, onda je parametrizacija $\mathbf{r}^{-}:\ [a,\,b]\to\mathbb{R}^{n}$ def. sa $\mathbf{r}^{-1}(t)=\mathbf{r}(a+b-t)$ suprotne orijentacije od $\mathbf{r}$.

**Stav**. $\begin{align}\int_{\mathcal{C}} \mathbf{f}(\mathbf{x})\cdot d\mathbf{r}^{-} =-\int_{\mathcal{C}} \mathbf{f}(\mathbf{x})\cdot d\mathbf{r}\end{align}$

Krivu orijentisanu suprotno od krive $\mathcal{C}$ označavamo sa $\mathcal{C}^{-}$, tj. $\begin{align}\int_{\mathcal{C}} \mathbf{f}(\mathbf{x})\cdot d\mathbf{r}^{-} =\int_{\mathcal{C}^{-}} \mathbf{f}(\mathbf{x})\cdot d\mathbf{r}\end{align}$

___
 **Teorema** (Grinova formula). Neka je $D\subseteq\mathbb{R}^{2}$ [[Vrste tačaka u odnosu na neki skup. Ograničenost i kompaktnost#^3969f8|kompaktan]] i takav da mu je granica $\mathcal{C}=\partial D$ deo po deo glatka kriva. Neka je $\mathbf{f}=(P,\,Q):\ D\to\mathbb{R}^{2}$ vektorsko polje, takvo da su $P,\,Q,\,P'_{y},\,Q'_{x}$ neprekidni na $\mathcal{C}$. I neka je $\mathcal{C}$ orijentisana tako da $D$ ostaje sa leve strane. Tada
 $\begin{align}\oint_{\mathcal{C}} \mathbf{f}(x,\,y) \cdot d\mathbf{r}=\iint_{D} (Q'_{x}-P'_{y}) \, dxdy\end{align}$
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
### Integriranje gradijenta
**Def**. Vektorsko polje $\mathbf{f}=\nabla f$ je **konzervativno** (gradijentno), a $f$ je **potencijal** tog polja.

**Teorema** (Uopštenje Njutn-Lajbnicove formule). Neka je $\mathbf{f}:\ D\to\mathbb{R}^{n}$ konzervativno neprekidno vektorsko polje ($\mathbf{f}=\nabla f$) i neka je $\mathcal{C}$ proizvoljna deo po deo glatka kriva koja spaja tačke $\mathbf{x},\,\mathbf{y}\in D$. Tada
$\begin{align}\int_{\mathcal{C}} \mathbf{f} \cdot d\mathbf{r} = f(\mathbf{y})-f(\mathbf{x})\end{align}$
> Dokaz: Neka je $\mathcal{C}$ parametrizovana sa $\mathbf{r}=(x_{1},\,x_{1},\,\dots,\,x_{n}):\ [a,\,b]\to\mathbb{R}^{n}$
> $\begin{align}\int_{\mathcal{C}} \mathbf{f} \cdot d\mathbf{r} = \int_{\mathcal{C}} \nabla f \cdot d\mathbf{r}= \int_{a}^{b} \sum\limits_{i=1}^{n} (f'_{x_{i}}\circ\mathbf{r})(t)\,x'_{i}(t)\,dt\end{align}$ $=$ \[[[Diferencijabilnost funkcije više promenljivih#^4816ca|*]]] $=$
> $\begin{align}=\int_{a}^{b} (f\circ\mathbf{r})'(t) \, dt=(f\circ\mathbf{r})(b)-(f\circ \mathbf{r})(a)=f(\mathbf{y})-f(\mathbf{x})\end{align}$

$\:$
**Teorema**. Neka je $\mathbf{f}:\ D\to\mathbb{R}^{n}$ neprekidno vektorsko polje. Tada su tvrđenja ekvivalentna:
1. $\mathbf{f}$ je konzervativno.
2. $\forall \mathbf{x},\,\mathbf{y}\in D$ $\quad$ za svaku deo po deo neprekidnu krivu $\mathcal{C}\subset D$ koja spaja $\mathbf{x}$ i $\mathbf{y}$ ista je vrednost $\begin{align}\int_{\mathcal{C}} \mathbf{f} \cdot d\mathbf{r} \end{align}$.
3. Za svaku zatvorenu deo po deo neprekidnu krivu $\mathcal{C}\subset D$ važi $\begin{align}\oint_{\mathcal{C}} \mathbf{f} \cdot d\mathbf{r} =0\end{align}$.  

> Dokaz:
> $\boxed{1. \Rightarrow 2.}$ Prethodna teorema.
> 
> $\boxed{2. \Rightarrow 3.}$ Neka je $\mathcal{C}$ zatvorena deo po deo neprekidna kriva.
> Neka su $\mathcal{C}_{1}\subset\mathcal{C}$ i $\mathcal{C}_{2}\subset\mathcal{C}$ krive koje spajaju tačke $\mathbf{x},\,\mathbf{y}\in\mathcal{C}$  ($\mathcal{C}_{1}\ne\mathcal{C}_{2}$).
> Tada $\mathcal{C}=\mathcal{C}_{1}\cup \mathcal{C}_{2}^{-}$, stoga $\begin{align}\int_{\mathcal{C}} \mathbf{f} \cdot d\mathbf{r}=\int_{\mathcal{C}_{1}} \mathbf{f} \cdot d\mathbf{r}+\int_{\mathcal{C}_{2}^{-}} \mathbf{f} \cdot d\mathbf{r}=\int_{\mathcal{C}_{1}} \mathbf{f} \cdot d\mathbf{r}-\int_{\mathcal{C}_{2}} \mathbf{f} \cdot d\mathbf{r} \xlongequal{\text{pretpostavka}} 0\end{align}$.
> 
> $\boxed{3. \Rightarrow 1.}$ Neka za svaku svaku zatvorenu deo po deo neprekidnu krivu $\mathcal{C}$ važi $\begin{align}\oint_{\mathcal{C}} \mathbf{f} \cdot d\mathbf{r} =0\end{align}$.
> 
> Izaberemo fiksiranu tačku $\mathbf{x}$, a $\mathbf{y}$ je proizvoljno.
> 
> Neka su $\mathcal{C}_{1}$ i $\mathcal{C}_{2}$ dve proizvoljne deo po deo neprekidne krive koje spajaju $\mathbf{x}$ i $\mathbf{y}$, tad za krivu $\mathcal{C}_{1}\cup \mathcal{C}_{2}^{-}$ važi pretpostavka. Stoga, $\begin{align}\int_{\mathcal{C}_{1}} \mathbf{f} \cdot d\mathbf{r}-\int_{\mathcal{C}_{2}} \mathbf{f} \cdot d\mathbf{r}=\int_{\mathcal{C}_{1}\cup\mathcal{C}_{2}^{-}} \mathbf{f} \cdot d\mathbf{r}=0\end{align}$, tj. vrednost $\begin{align}\int_{\mathcal{C}} \mathbf{f}\cdot d\mathbf{r} \end{align}$ ne zavisi od izbora krive.
> 
> Označimo sa $\mathcal{C}(\mathbf{x},\,\mathbf{y})$ proizvoljnu krivu sa početkom u $\mathbf{x}$ i krajem u $\mathbf{y}$.
> Zbog zaključka u prethodnom pasusu dobro je definisana fja $f:\ D\to\mathbb{R}$ sa $\begin{align}f(\mathbf{y}):=\int_{\mathcal{C}(\mathbf{x},\,\mathbf{y})}  \mathbf{f}\cdot d\mathbf{r} \end{align}$.
> 
> $\begin{align}f'_{x_{i}}(\mathbf{y})=\lim\limits_{ h \to 0 }\frac{f(\mathbf{y}+h\,\mathbf{e}_{i})-f(\mathbf{y})}{h}=\lim\limits_{ h \to 0 }\frac{\begin{align}\int_{\mathcal{C}(\mathbf{y},\,\mathbf{y}+h\mathbf{e}_{i})}\mathbf{f} \cdot d\mathbf{r}\end{align}}{h}=\end{align}$
> > Neka je kriva $\mathcal{C}(\mathbf{y},\,\mathbf{y}+h\mathbf{e}_{i})$ prava, tad nju možemo parametrizovati fjom $\mathbf{r}:\ [0,\,h]\to\mathbb{R}^{n}$ def. sa $\mathbf{r}(t)=\mathbf{y}+t\,\mathbf{e}_{i}$
> 
> $\begin{align}=\lim\limits_{ h \to 0 }\frac{\begin{align}\int_{0}^{h} (\mathbf{f}\circ \mathbf{r})(t) \cdot\mathbf{r}'(t)\, dt\end{align}}{h}=\lim\limits_{ h \to 0 }\frac{\begin{align}\int_{0}^{h} \mathbf{f}(\mathbf{y}+t\,\mathbf{e}_{i}) \cdot\mathbf{e}_{i}\, dt\end{align}}{h}=\end{align}$
> $=\Big[$ Iz [[Riman-integrabilnost funkcija i svojstva određenog integrala#^88105f|teoreme]] $\exists \xi$ između $0$ i $h$ $\Big]=$
>  $\begin{align}=\lim\limits_{ h \to 0 }\frac{h\,\mathbf{f}(\mathbf{y}+\xi\,\mathbf{e}_{i})\cdot\mathbf{e}_{i}}{h}=\lim\limits_{ h \to 0 }\Big(\,\mathbf{f}(\mathbf{y}+\xi\,\mathbf{e}_{i})\cdot\mathbf{e}_{i}\Big)=\mathbf{f}(\mathbf{y})\cdot\mathbf{e}_{i}\end{align}$ 
> 
> Stoga, $\mathbf{f}=\nabla f$

$\:$
> Napomena: Ako važi jedan od uslova $2.$ i $3.$ u prethodnoj teoreme, za dati gradijent možemo naći polaznu funkciju do na koeficijent.

$\:$
**Posledica** (prethodne teoreme i Grinove formule). Neka je $\mathbf{f}=(P,\,Q):\ D\to\mathbb{R}^{2}$ neprekidno vektorsko polje, takvo da su $P'_{y}$ i $Q'_{x}$ neprekidni.
Tada $\mathbf{f}$ je konzervativno akko $P'_{y}=Q'_{x}$