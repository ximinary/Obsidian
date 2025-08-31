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
**Teorema**. Ako je $f$ deo po deo neprekidna i $\mathbf{r}$ je regularna parametrizacija krive $\mathcal{C}$, onda $\begin{align}\int_{\mathcal{C}} f(\mathbf{x}) \, ||d\mathbf{r}|| =\int_{a}^{b} (f\circ \mathbf{r})(t)\,||\mathbf{r}'(t)||\, dt \end{align}$ 
> Dokaz:
> $\begin{align}\sigma(f,\,\mathbf{P},\,\boldsymbol{\xi})=\sum\limits_{i=1}^{n}||\mathbf{x}_{i}-\mathbf{x}_{i-1}||\,f(\boldsymbol{\xi}_{i})=\sum\limits_{i=1}^{n}||\mathbf{r}(t_{i})-\mathbf{r}(t_{i-1})||\,f(\mathbf{r}(\xi_{i}))=\end{align}$
> $\begin{align}=\sum\limits_{i=1}^{n}(t_{i}-t_{i-1})\Bigg|\Bigg|\frac{\mathbf{r}(t_{i})-\mathbf{r}(t_{i-1})}{t_{i}-t_{i-1}}\Bigg|\Bigg|\,(f\circ \mathbf{r})(\xi_{i})=\end{align}$ $\Big[\,$[[Teoreme o srednjoj vrednosti#^e52da5|Lagranž]], $\mu_{i}\in(t_{i-1},\,t_{i})\,\Big]=$
> $\begin{align}=\sum\limits_{i=1}^{n}(t_{i}-t_{i-1})||\mathbf{r}'(\mu_{i})||\,(f\circ \mathbf{r})(\xi_{i})\end{align}$
> 
> $\begin{align}\int_{\mathcal{C}} f(\mathbf{x}) \, ||d\mathbf{r}|| =\lim\limits_{ \lambda(\mathbf{P}) \to 0 }\sigma(f,\,\mathbf{P},\,\boldsymbol{\xi})=\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sum\limits_{i=1}^{n}(t_{i}-t_{i-1})||\mathbf{r}'(\mu_{i})||\,(f\circ \mathbf{r})(\xi_{i})=\end{align}$
> $\begin{align}=\int_{a}^{b} (f\circ \mathbf{r})(t)\,||\mathbf{r}'(t)||\, dt \end{align}$ 

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
### [[Integralna veza skupa i njegove granice#Grinova formula|Grinova formula]]. [[Integralna veza skupa i njegove granice#Stoksova formula|Stoksova formula]] 
### [[Konzervativno vektorsko polje]]
