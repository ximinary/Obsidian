#fax #math #a3 [deo [[Analiza|analize]]]
$\:$

**Def**. Neka je $\mathbf{r}:I\to\mathbb{R}^{3}$ diferencijabilno preslikavanje, tada je skup $\mathbf{r}[I]$ ([[Direktna i inverzna slika skupa#^93355e|slika]] intervala $I$) **kriva** u $\mathbb{R}^{3}$.
$\mathbf{r}(t)=\big(x(t),\,y(t),\,z(t)\big)$.
Kriva je **regularna** ako  $\forall t\in I\quad\big(x'(t),\,y'(t),\,z'(t)\big)\ne \mathbf{0}$. ^f25bf0

**Def**. $\tau$ je **tangenta** na (regularnu) krivu parametrizovanu sa $\mathbf{r}$ u tački $\mathbf{a}=\mathbf{r}(t_{0})$, ako prolazi kroz $\mathbf{a}$ i vektor pravca joj  je $\mathbf{r}'(t_{0})=\big(x'(t),\,y'(t),\,z'(t)\big)$

Kriva parametrizovana sa $\mathbf{r}:\ [a,\,b]\to\mathbb{R}^{3}$ je **zatvorena** ako $\mathbf{r}(a)=\mathbf{r}(b)$. ^66ef03

Kriva parametrizovana sa $\mathbf{r}:\ [a,\,b]\to\mathbb{R}^{3}$ je **prosta** ako $\forall x,\,y\in(a,\,b)\quad\mathbf{r}(x)\ne\mathbf{r}(y)$. 
___

**Def**. **Regularna površ** u prostoru $\mathbb{R}^{3}$ je skup $\mathcal{P} = \big\{(x, y, z)\ \ |\ \ f (x, y, z) = 0\big\}=f^{-1}\big[\{0\}\big]$,
gde je $f:\ \mathbb{R}^{3}\to\mathbb{R}$ je funkcija za koju važi $\forall \mathbf{a}\in \mathcal{P}\quad\nabla\!f(\mathbf{a})\ne\mathbf{0}$. ^5afd44

**Stav**. #note/to_do

**Def**. Neka je $\mathcal{P}$ regularna površ. Unija svih tangenti na sve krive $\mathbf{r}$ koje prolaze kroz tačku $\mathbf{a}\in\mathcal{P}$ i koje pripadaju površi $\mathcal{P}$ naziva se **tangentna ravan** u tački $\mathbf{a}$ na površ $\mathcal{P}$. 

$\:$
**Stav**. Neka je $\mathcal{P} = \big\{(x, y, z)\ \ |\ \ f (x, y, z) = 0\big\}$ regularna površ, neka kriva $\mathbf{r}$ pripada površi $\mathcal{P}$  i $\mathbf{a}=\mathbf{r}(t_{0})$. Tada je $\nabla\!f(\mathbf{a})\perp \mathbf{r}'(t_{0})$ ^635980

> Dokaz: $\mathbf{r}$ pripada $\mathcal{P}$, to znači da $f\big(\mathbf{r}(t)\big)=0,\quad\forall t\in\mathbb{R}$
> odakle, $(f\circ \mathbf{r})'(t)=df(t)\,d\mathbf{r}(t)=\nabla\!f(\mathbf{a})\cdot \mathbf{r}'(t_{0})=0$

$\:$
**Stav**. Ako je površ $\mathcal{P} = \big\{(x, y, z)\ \ |\ \ f (x, y, z) = 0\big\}$ regularna u tački $\mathbf{a}$, onda je njena tangentna ravan u $\mathbf{a}$ zaista ravan, čiji je vektor normale $\nabla\!f(\mathbf{a})$