#fax #math #a3 [deo [[Analiza|analize]]]

### Podela [[Kriva i površ#Dvodimenziona površ u $ mathbb{R} {n}$|površi]] 
Neka je $\mathcal{S}$ površ regularno parametrizovana sa $\mathbf{r}:\ D\to\mathbb{R}^{n}$ $\ \:$ i $\ \:$ neka je $(\mathcal{P},\,\xi)$ [[Dvostruki integral#Podela pravougaonika|podela]] sa istaknutim tačkama pravougaonika $\Pi$ $\Big(D\subseteq\Pi\subseteq\mathbb{R}^{2}\Big)$, koja je zadata tačkama $(u_{i},\,v_{j}),\ \ i=\overline{0,n},\ j=\overline{1,m}$.
Neka je $\Pi_{ij}=[u_{i-1},\,u_{i}]\times[v_{j-1},\,v_{j}]$

*Proširimo* $\mathbf{r}$ na skup $\Pi$.
Sada je $\mathbf{P}=\Big\{\mathbf{r}[\Pi_{ij}]\ \Big|\ i =\overline{1,n},\ j=\overline{1,m}\Big\}$ **podela** *proširenja* **površi** $\mathcal{S}$, koja je zadata tačkama $\mathbf{x}_{ij}:=\mathbf{r}(u_{i},\,v_{j}),\ \ i=\overline{0,n}$ su podeone tačke te podele i $\lambda(\mathbf{P})=\lambda(\mathcal{P})$

$\boldsymbol{\xi}_{ij}:=\mathbf{r}(\xi_{ij}),\ \ \forall i=\overline{1,n},\ j=\overline{1,m}$, $\quad$ gde su $\xi_{i}$ istaknute tačke podele $\mathcal{P}$.

$(\mathbf{P},\,\boldsymbol{\xi})$ je **podela sa istaknutim tačkama** *proširenja* **površi** $\mathcal{S}$

Aproksimiramo površinu dela površi $\mathbf{r}[\Pi_{ij}]$ sa površinom koju određuju vektori $\overrightarrow{\mathbf{x}_{i-1j}\mathbf{x}_{ij}}$ i $\overrightarrow{\mathbf{x}_{ij-1}\mathbf{x}_{ij}}$ tj. sa $||(\mathbf{x}_{ij}-\mathbf{x}_{i-1j})\times(\mathbf{x}_{ij}-\mathbf{x}_{ij-1})||$

### Površinski integral skalar-funkcije
**Def**. Neka je $f:\ \mathcal{S}\to\mathbb{R}$,  a $\widetilde{f}:\ \Pi\to\mathbb{R}$ je *proširenje* fje $f$ na $\Pi\supseteq D$, pri tome $\widetilde{f}(u,\,v)=0$ za svako $(u,\,v)\in\Pi\setminus\mathcal{S}$. i $\ \:(\mathbf{P},\,\boldsymbol{\xi})$ podela sa istaknutim tačkama *proširenja* površi $\mathcal{S}$. Zbir $\begin{align}\sigma(\widetilde{f},\,\mathbf{P},\,\boldsymbol{\xi})=\sum\limits_{i,\,j}||(\mathbf{x}_{ij}-\mathbf{x}_{i-1j})\times(\mathbf{x}_{ij}-\mathbf{x}_{ij-1})||\,\widetilde{f}(\boldsymbol{\xi}_{ij})\end{align}$ je **integralna suma**. ($P$ je površina)

$\:$
**Def**. Neka je $f:\ \mathcal{S}\to\mathbb{R}$. $\ \:$ $I\in\mathbb{R}$ je limes integralnih suma $\sigma(\widetilde{f},\,\mathbf{P},\,\boldsymbol{\xi})$ kad $\lambda(\mathbf{P})\to0$ ako
$\begin{align}\forall\varepsilon>0\quad\exists\delta>0\quad\forall\binom{(\mathbf{P},\,\boldsymbol{\xi} )\ \text{— podela sa istaknutim tačkama}}{\text{ proširenja površi }\mathcal{S}\text{ takva da } \lambda(\mathbf{P})<\delta}\quad \Big|I-\sigma(\widetilde{f},\,\mathbf{P},\,\boldsymbol{\xi})\Big|<\varepsilon\end{align}$
$\:$
Tada je $\begin{align}I=\iint_{\mathcal{S}} f(\mathbf{x}) \, ||d\mathbf{S}|| \end{align}$ $\:$ **površinski integral** (prve vrste) fje $f$ po površi $\mathcal{S}$.

$\:$
**Teorema**. Ako je $\mathbf{r}:\ D\to\mathbb{R}$, onda $\begin{align}\iint_{\mathcal{S}} f(\mathbf{x}) \, ||d\mathbf{S}|| = \iint_{D} (f\circ\mathbf{r})(u,\,v) \, ||\mathbf{r}'_{u}(u,\,v)\times \mathbf{r}'_{v}(u,\,v)||\,du\,dv\end{align}$
> Dokaz:
> $\begin{align}\sigma(\widetilde{f},\,\mathbf{P},\,\boldsymbol{\xi})=\sum\limits_{i,\,j}||(\mathbf{x}_{ij}-\mathbf{x}_{i-1j})\times(\mathbf{x}_{ij}-\mathbf{x}_{ij-1})||\,\widetilde{f}(\boldsymbol{\xi}_{ij})=\end{align}$
> $\begin{align}=\sum\limits_{i,\,j}(u_{i}-u_{i-1})(v_{j}-v_{j-1})\Bigg|\Bigg|\frac{\mathbf{r}(u_{i},\,v_{j})-\mathbf{r}(u_{i-1},\,v_{j})}{u_{i}-u_{i-1}}\times\frac{\mathbf{r}(u_{i},\,v_{j})-\mathbf{r}(u_{i},\,v_{j-1})}{v_{j}-v_{j-1}}\Bigg|\Bigg|\,(\widetilde{f}\circ \mathbf{r})(\xi_{ij})=\end{align}$
> $=\Big[\,$[[Teoreme o srednjoj vrednosti#^e52da5|Lagranž]], $\overline{u}_{i}\in(u_{i-1},\,u_{i}),\ \overline{v}_{j}\in(v_{j-1},\,v_{j})\,\Big]=$
> $\begin{align}=\sum\limits_{i,\,j}(u_{i}-u_{i-1})(v_{j}-v_{j-1})||\mathbf{r}'_{u}(\overline{u}_{i},\,v_{j})\times\mathbf{r}'_{v}(u_{i},\,\overline{v}_{j})||\,(\widetilde{f}\circ \mathbf{r})(\xi_{ij})\end{align}$
> 
> $\begin{align}\int_{\mathcal{C}} f(\mathbf{x}) \, ||d\mathbf{S}|| =\lim\limits_{ \lambda(\mathbf{P}) \to 0 }\sigma(\widetilde{f},\,\mathbf{P},\,\boldsymbol{\xi})=\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sum\limits_{i,\,j}(u_{i}-u_{i-1})(v_{j}-v_{j-1})||\mathbf{r}'_{u}(\overline{u}_{i},\,v_{j})\times\mathbf{r}'_{v}(u_{i},\,\overline{v}_{j})||\,(\widetilde{f}\circ \mathbf{r})(\xi_{ij})=\end{align}$
> $\begin{align}=\iint_{D} (f\circ\mathbf{r})(u,\,v)) \, ||\mathbf{r}'_{u}(u,\,v)\times \mathbf{r}'_{v}(u,\,v)||\,du\,dv \end{align}$ 

$\:$
**Def**. $||d\mathbf{S}||=||\mathbf{r}'_{u}\times \mathbf{r}'_{v}||\,du\,dv$ je **element površine**.


___
Napomena: [[Dvostruki integral#Definicija i svojstva dvostrukog integrala na proizvoljnom merljivom skupu|svojstva dvostrukog integrala]]

**[[Riman-integrabilnost funkcija i svojstva određenog integrala#^cfc6a3|Stav]]**.  $f$ i $g$ su neprekidni; $\ \ \alpha,\,\beta\in\mathbb{R}$. Tada važi
$\begin{align}\iint_{\mathcal{S}}(\alpha\,f+\beta\,g)(\mathbf{x}) \, ||d\mathbf{S}|| = \alpha\iint_{\mathcal{S}} f(\mathbf{x}) \, ||d\mathbf{S}||+\beta \iint_{\mathcal{S}} g(\mathbf{x}) \, ||d\mathbf{S}|| \end{align}$

**Stav**.  $f$ i $g$ su neprekidni; $\ \ \forall \mathbf{x}\in \mathcal{S}\quad f(\mathbf{x})\leqslant g(\mathbf{x})$. Tada $\begin{align}\iint_{\mathcal{S}} f(\mathbf{x}) \, ||d\mathbf{S}||\leqslant \iint_{\mathcal{S}} g(\mathbf{x}) \, ||d\mathbf{S}|| \end{align}$

**Stav**. $f$ je neprekidna; presek površi $\mathcal{S}$ i $\mathcal{T}$ je regularna kriva. Tada
$\begin{align}\iint_{\mathcal{S}\cup \mathcal{T}} f(\mathbf{x}) \, ||d\mathbf{S}|| = \iint_{\mathcal{S}} f(\mathbf{x}) \, ||d\mathbf{S}|| + \iint_{\mathcal{T}} f(\mathbf{x}) \, ||d\mathbf{S}||\end{align}$


**Stav**. $\mathrm{P}(\mathcal{S})=\begin{align}\iint_{\mathcal{S}} 1 \, ||d\mathbf{S}||\end{align}$ $\ \:$ je površina površi $\mathcal{S}$

**[[Riman-integrabilnost funkcija i svojstva određenog integrala#Predstavljanje određenog integrala proizvodom|Stav]]**. $f$ je neprekidna. Tada
- Ako $m=\min\limits_{\mathcal{S}} f$, $\ \:$ $M=\max\limits_{\mathcal{S}}f$, $\ \:$ onda $\begin{align}\exists \mu\in[m,\,M]\quad \iint_{\mathcal{S}} f(\mathbf{x}) \, ||d\mathbf{S}|| = \mu\cdot \mathrm{P}(\mathcal{C}) \end{align}$
- $\begin{align}\exists\mathbf{x}_{0}\in\mathcal{S}\quad \iint_{\mathcal{S}} f(\mathbf{x}) \, ||d\mathbf{S}||= f(\mathbf{x}_{0})\cdot \mathrm{P}(\mathcal{S}) \end{align}$

### Površinski integral vektorskog polja
**Def**. Neka je $\mathcal{S}$ površ parametrizovana sa $\mathbf{r}:\ D\to\mathbb{R}^{3}$, $\ \:$ ($D\subseteq\mathbb{R}^{2}$) $\ \:$ i neka je $(\mathbf{P},\,\boldsymbol{\xi})$ podela sa istaknutim tačkama *proširenja* te površi. Neka je $\ \:$ $\mathbf{f}:\ \mathcal{S}\to\mathbb{R}^{3}\ \:$ vektorsko polje, a $\tilde{\mathbf{f}}:\ \Pi\to\mathbb{R}^{3}$ je proširenje $\mathbf{f}$ na $\Pi\supseteq D$, takvo da $\mathbf{f}(u,\,v)=\mathbf{0}$ za svako $(u,\,v)\in\Pi\setminus D$. 
Zbir $\begin{align}\sigma(\tilde{\mathbf{f}},\,\mathbf{P},\,\boldsymbol{\xi})=\sum\limits_{i,\,j}(\mathbf{x}_{ij}-\mathbf{x}_{i-1j})\times(\mathbf{x}_{ij}-\mathbf{x}_{ij-1})\cdot\mathbf{f}(\boldsymbol{\xi}_{i})\end{align}$ je **integralna suma** ($\cdot$ je skalarni proizvod).

$\:$
**Def**. Neka je $\mathbf{f}:\ \mathcal{S}\to\mathbb{R}^{3}$. $\ \:$ $I\in\mathbb{R}$ je limes integralnih suma $\sigma(\tilde{\mathbf{f}},\,\mathbf{P},\,\boldsymbol{\xi})$ kad $\lambda(\mathbf{P})\to0$ ako
$\begin{align}\forall\varepsilon>0\quad\exists\delta>0\quad\forall\binom{(\mathbf{P},\,\boldsymbol{\xi} )\ \text{— podela sa istaknutim tačkama}}{\text{ proširenja površi }\mathcal{S}\text{ takva da } \lambda(\mathbf{P})<\delta}\quad \Big|I-\sigma(\tilde{\mathbf{f}},\,\mathbf{P},\,\boldsymbol{\xi})\Big|<\varepsilon\end{align}$
$\:$
Tada je $\begin{align}I=\iint_{\mathcal{S}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{S} \end{align}$ $\:$ **površinski integral** (druge vrste) fje $\mathbf{f}$ po površi $\mathcal{S}$.

$\:$
**Teorema**. Neka je $\mathcal{S}$ površ parametrizovana sa $\mathbf{r}:\ D\to\mathbb{R}^{3}$ $\ \:$ i $\ \:$ neka je $\mathbf{f}:\ \mathcal{S}\to \mathbb{R}^{3}$ vektorsko polje. Označimo sa $\begin{align}\mathbf{n}:=\frac{\mathbf{r}'_{u}\times r'_{v}}{||\mathbf{r}'_{u}\times r'_{v}||}\end{align}$ jedinični vektor normale na $\mathcal{S}$
Tada, $\begin{align}\iint_{\mathcal{S}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{S} =\iint_{D} (\mathbf{f}\circ\mathbf{r})(u,\,v) \cdot \Big( \mathbf{r}'_{u}(u,\,v)\times r'_{u}(u,\,v)\Big) \, du\,dv= \iint_{\mathcal{S}} \mathbf{f}(\mathbf{x})\cdot \mathbf{n} \, ||d\mathbf{S}||\end{align}$

> Dokaz: 
> $\begin{align}\sigma(\tilde{\mathbf{f}},\,\mathbf{P},\,\boldsymbol{\xi})=\sum\limits_{i,\,j}(\mathbf{x}_{ij}-\mathbf{x}_{i-1j})\times(\mathbf{x}_{ij}-\mathbf{x}_{ij-1})\cdot\mathbf{f}(\boldsymbol{\xi}_{i})=\end{align}$
> $\begin{align}=\sum\limits_{i,\,j}(u_{i}-u_{i-1})(v_{j}-v_{j-1})\frac{\mathbf{r}(u_{i},\,v_{j})-\mathbf{r}(u_{i-1},\,v_{j})}{u_{i}-u_{i-1}}\times\frac{\mathbf{r}(u_{i},\,v_{j})-\mathbf{r}(u_{i},\,v_{j-1})}{v_{j}-v_{j-1}}\cdot(\tilde{\mathbf{f}}\circ \mathbf{r})(\xi_{ij})=\end{align}$
 > $=\Big[\,$[[Teoreme o srednjoj vrednosti#^e52da5|Lagranž]], $\overline{u}_{i}\in(u_{i-1},\,u_{i}),\ \overline{v}_{j}\in(v_{j-1},\,v_{j})\,\Big]=$
> $\begin{align}=\sum\limits_{i,\,j}(u_{i}-u_{i-1})(v_{j}-v_{j-1})\mathbf{r}'_{u}(\overline{u}_{i},\,v_{j})\times\mathbf{r}'_{v}(u_{i},\,\overline{v}_{j})\cdot\,(\tilde{\mathbf{f}}\circ \mathbf{r})(\xi_{ij})\end{align}$
> 
> $\begin{align}\iint_{\mathcal{S}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{S} =\lim\limits_{ \lambda(\mathbf{P}) \to 0 }\sigma(\tilde{\mathbf{f}},\,\mathbf{P},\,\boldsymbol{\xi})=\lim\limits_{ \lambda(\mathcal{P}) \to 0 }\sum\limits_{i,\,j}(u_{i}-u_{i-1})(v_{j}-v_{j-1})\mathbf{r}'_{u}(\overline{u}_{i},\,v_{j})\times\mathbf{r}'_{v}(u_{i},\,\overline{v}_{j})\cdot\,(\tilde{\mathbf{f}}\circ \mathbf{r})(\xi_{ij})=\end{align}$
> $\begin{align}=\iint_{D} (\mathbf{f}\circ\mathbf{r})(u,\,v) \cdot \Big( \mathbf{r}'_{u}(u,\,v)\times r'_{u}(u,\,v)\Big) \, du\,dv=\iint_{D} (\mathbf{f}\circ \mathbf{r})(u,\,v)\cdot \frac{\mathbf{r}'_{u}(u,\,v)\times r'_{u}(u,\,v)}{||\mathbf{r}'_{u}(u,\,v)\times r'_{u}(u,\,v)||}||\mathbf{r}'_{u}(u,\,v)\times r'_{u}(u,\,v)||\, du\,dv=\end{align}$ 
> $\begin{align}=\iint_{\mathcal{S}} (\mathbf{f}\circ \mathbf{r})(u,\,v)\cdot \mathbf{n}\,||d\mathbf{S}||\end{align}$

$\:$
> Napomena:
> Razmatramo površ $\mathcal{S}$ u $\mathbb{R}^{3}$ parametrizovanu sa $\mathbf{r}:\ D\to\mathbb{R}^{3}$ def. sa $\mathbf{r}(u,\,v)=\Big(x(u,\,v),\ y(u,\,v),\ z(u,\,v)\Big)$ i vektorsko polje $\mathbf{f}=(P,\,Q,\,R)$, imamo
> $\begin{align}\iint_{\mathcal{S}} \mathbf{f}(x,\,y,\,z) \cdot d\mathbf{S}=\iint_{D} \mathbf{f}\Big(x(u,\,v),\ y(u,\,v),\ z(u,\,v)\Big)\cdot \left|\begin{array}{c}\mathbf{i}&\mathbf{j}&\mathbf{k}\\x'_{u}(u,\,v)&y'_{u}(u,\,v)&z'_{u}(u,\,v)\\x'_{v}(u,\,v)&y'_{v}(u,\,v)&z'_{v}(u,\,v)\end{array}\right| \, du\,dv=\end{align}$
> $\begin{align}=\iint_{D} \left|\begin{array}{c}P\Big(x(u,\,v),\ y(u,\,v),\ z(u,\,v)\Big)&Q\Big(x(u,\,v),\ y(u,\,v),\ z(u,\,v)\Big)&R\Big(x(u,\,v),\ y(u,\,v),\ z(u,\,v)\Big)\\x'_{u}(u,\,v)&y'_{u}(u,\,v)&z'_{u}(u,\,v)\\x'_{v}(u,\,v)&y'_{v}(u,\,v)&z'_{v}(u,\,v)\end{array}\right| \, du\,dv=\end{align}$
> $\begin{align}=\iint_{\mathcal{S}}P(x,\, y,\, z)\,dy\,dz+Q(x,\, y,\, z)\,dz\,dx+R(x,\, y,\, z)\,dx\,dy\end{align}$

 ___
 
 **Stav**. $\alpha,\,\beta\in\mathbb{R}$. Tada važi
$\begin{align}\iint_{\mathcal{S}}(\alpha\,\mathbf{f}+\beta\,\mathbf{g})(\mathbf{x}) \cdot d\mathbf{S} = \alpha\iint_{\mathcal{S}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{S}+\beta \iint_{\mathcal{S}} \mathbf{g}(\mathbf{x}) \cdot d\mathbf{S} \end{align}$

**Stav**. Presek površi $\mathcal{S}$ i $\mathcal{T}$ je regularna kriva. Tada $\begin{align}\int_{\mathcal{S}\cup \mathcal{T}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{S} = \int_{\mathcal{S}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{S} + \int_{\mathcal{T}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{S}\end{align}$
___
Površ $\mathcal{S}$ možemo orijentisati na dva načina: ako je vektor normale $\mathbf{n}$ i ako je vektor normale $-\mathbf{n}$. Površ orijentisanu suprotno od površi $\mathcal{S}$ označavamo sa $\mathcal{S}^{-}$, tada $\begin{align}\iint_{\mathcal{S}^{-}} \mathbf{f}(\mathbf{x})\cdot d\mathbf{S} =-\iint_{\mathcal{S}} \mathbf{f}(\mathbf{x})\cdot d\mathbf{S}\end{align}$


> Napomena: Ako je površ data sa $\varphi(x,\,y,\,z)=0$, onda je $\begin{align}\mathbf{n}=\pm\frac{\nabla\varphi}{||\nabla\varphi||}\end{align}$. Tad $\begin{align}\iint_{\mathcal{S}} \mathbf{f}(\mathbf{x}) \cdot d\mathbf{S} = \pm\iint_{\mathcal{S}} \mathbf{f}(\mathbf{x})\cdot \frac{\nabla\varphi}{||\nabla\varphi||} \, ||d\mathbf{S}||\end{align}$