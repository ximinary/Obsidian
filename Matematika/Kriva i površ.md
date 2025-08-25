#fax #math #a3 [deo [[Analiza|analize]]]


### Kriva u $\mathbb{R}^{n}$
**Def**. Neka je $\mathbf{r}:I\to\mathbb{R}^{n}$ diferencijabilno preslikavanje, tada je skup $\mathbf{r}[I]$ **kriva** u $\mathbb{R}^{n}$.
$\mathbf{r}(t)=\big(x_{1}(t),\,x_{2}(t),\,\dots,\,x_{n}(t)\big)$.
Kriva je **regularna** ako  $\forall t\in I\quad\mathbf{r}'(t)=\big(x_{1}'(t),\,x_{2}'(t),\,\dots,\,x_{n}'(t)\big)\ne \mathbf{0}$. ^f25bf0

**Def**. $\tau$ je **tangenta** na (regularnu) krivu parametrizovanu sa $\mathbf{r}$ u tački $\mathbf{a}=\mathbf{r}(t_{0})$, ako prolazi kroz $\mathbf{a}$ i vektor pravca joj  je $\mathbf{r}'(t_{0})=\big(x_{1}'(t_{0}),\,x_{2}'(t_{0}),\,\dots,\,x_{n}'(t_{0})\big)\ne \mathbf{0}$

Kriva parametrizovana sa $\mathbf{r}:\ [a,\,b]\to\mathbb{R}^{n}$ je **zatvorena** ako $\mathbf{r}(a)=\mathbf{r}(b)$. ^66ef03

Kriva parametrizovana sa $\mathbf{r}:\ [a,\,b]\to\mathbb{R}^{n}$ je **prosta** ako $\forall x,\,y\in(a,\,b)\quad\mathbf{r}(x)\ne\mathbf{r}(y)$. 

> Napomena: [[Krive drugog reda]]

$\:$
### Dvodimenziona površ u $\mathbb{R}^{n}$
**Def**. Neka je $D\in\mathbb{R}^{2}$ takav da je $\mathrm{int}\,D$ povezan i neka je $\mathbf{r}:D\to\mathbb{R}^{n}$ neprekidno (zajedno sa parcijalnim izvodima) preslikavanje, tada je skup $\mathbf{r}[D]$ **površ** u $\mathbb{R}^{n}$.
$\mathbf{r}(u,\,v)=\Big(x_{1}(u,\,v),\ x_{2}(u,\,v),\ \dots,\ x_{n}(u,\,v)\Big)$.
Površ je **regularna** ako  $\forall (u,\,v)\in D$ $\quad$ $\mathbf{r}'_{u}(u,\,v)$ $\:$ i $\:$ $\mathbf{r}'_{v}(u,\,v)$ su linearno nezavisni.  ^bc95d7

> Napomena: [[Površi drugog reda]]

$\:$
### $(n-1)$-dimenziona površ u $\mathbb{R}^{n}$

**Def**. **Regularna** $(n-1)$**-dimenziona površ** u $\mathbb{R}^{n}$ je skup $\mathcal{P} = \big\{\mathbf{x}\ \ |\ \ f (\mathbf{x}) = 0\big\}=f^{-1}\big[\{0\}\big]$,
gde je $f:\ \mathbb{R}^{n}\to\mathbb{R}$ je funkcija za koju važi $\forall \mathbf{a}\in \mathcal{P}\quad\nabla\!f(\mathbf{a})\ne\mathbf{0}$. ^5afd44

### Površ u $\mathbb{R}^{3}$
**Stav**. Definicije [[Kriva i površ#^bc95d7|1]] i [[Kriva i površ#^5afd44|2]] su lokalno ekvivalentne za $\mathbb{R}^{3}$.

$\:$
**Def**. Neka je $\mathcal{P}$ regularna površ. Unija svih tangenti na sve krive $\mathbf{r}$ koje prolaze kroz tačku $\mathbf{a}\in\mathcal{P}$ i koje pripadaju površi $\mathcal{P}$ naziva se **tangentna ravan** u tački $\mathbf{a}$ na površ $\mathcal{P}$. 

$\:$
**Stav**. Neka je $\mathcal{P} = \big\{(x, y, z)\ \ |\ \ f (x, y, z) = 0\big\}$ regularna površ, neka kriva $\mathbf{r}$ pripada površi $\mathcal{P}$  i $\mathbf{a}=\mathbf{r}(t_{0})$. Tada je $\nabla\!f(\mathbf{a})\perp \mathbf{r}'(t_{0})$ ^635980

> Dokaz: $\mathbf{r}$ pripada $\mathcal{P}$, to znači da $f\big(\mathbf{r}(t)\big)=0,\quad\forall t\in\mathbb{R}$
> odakle, $(f\circ \mathbf{r})'(t)=df(t)\,d\mathbf{r}(t)=\nabla\!f(\mathbf{a})\cdot \mathbf{r}'(t_{0})=0$

$\:$
**Stav**. Ako je površ $\mathcal{P} = \big\{(x, y, z)\ \ |\ \ f (x, y, z) = 0\big\}$ regularna u tački $\mathbf{a}$, onda je njena tangentna ravan u $\mathbf{a}$ zaista ravan, čiji je vektor normale $\nabla\!f(\mathbf{a})$