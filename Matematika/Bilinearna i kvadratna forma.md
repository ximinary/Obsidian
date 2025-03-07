#fax #math #laag [deo [[Linearna algebra|linearne algebre]]]

### Bilinearne forme
**Def**. Neka je $V$ [[Vektorski prostor|vektorski prostor]] nad poljem $\mathbb{F}$. Tada preslikavanje $\mathrm{A}:\ V\times V\to \mathbb{F}$ je:
- **bilinearna forma** na $\mathbb{F}=\mathbb{C}$ ako
  $\forall u,\,v,\,w\in V\quad \forall\alpha,\,\beta\in\mathbb{C}\ \ \:$ važe
	- (BF1) $\ \: \mathrm{A}(\alpha\,u+\beta\,v,\ w)=\alpha\,\mathrm{A}(u,\ w)+\beta\,\mathrm{A}(v,\ w)$
	- (BF2) $\ \: \mathrm{A}(u,\ \alpha\,v+\beta\,w)=\alpha\,\mathrm{A}(u,\ v)+\beta\,\mathrm{A}(u,\ w)$

$\:$
- **hermitska bilinearna forma** na $\mathbb{F}=\mathbb{C}$ ako
   $\forall u,\,v,\,w\in V\quad \forall\alpha,\,\beta\in\mathbb{C}\ \ \:$ važe
	- (BF1) $\ \: \mathrm{A}(\alpha\,u+\beta\,v,\ w)=\alpha\,\mathrm{A}(u,\ w)+\beta\,\mathrm{A}(v,\ w)$
	- (BF3') $\ \: \mathrm{A}(u,\ v)=\overline{\mathrm{A}(v,\ u)}$
	  $\:$
	- iz BF1 i BF3' sledi:
	  (BF2') $\ \: \mathrm{A}(u,\ \alpha\,v+\beta\,w)=\overline{\alpha}\,\mathrm{A}(u,\ v)+\overline{\beta}\,\mathrm{A}(u,\ w)$

$\:$
- **simetrična bilinearna forma** na $\mathbb{F}=\mathbb{R}$ ako
   $\forall u,\,v,\,w\in V\quad \forall\alpha,\,\beta\in\mathbb{C}\ \ \:$ važe
	- (BF1) $\ \: \mathrm{A}(\alpha\,u+\beta\,v,\ w)=\alpha\,\mathrm{A}(u,\ w)+\beta\,\mathrm{A}(v,\ w)$
	- (BF3) $\ \: \mathrm{A}(u,\ v)=\mathrm{A}(v,\ u)$
	  $\:$
	- iz BF1 i BF3 sledi BF2 (koje u $\mathbb{R}$ se podudara sa BF2')


### Primeri bilinearnih formi 
- [[Unitarni prostor. Euklidski prostor|Skalarni proizvod]] u VP nad poljem $\mathbb{C}$ je hermitska bilinearna forma.
[[Unitarni prostor. Euklidski prostor|Skalarni proizvod]] u VP nad poljem $\mathbb{R}$ je simetrična bilinearna forma.
- $V$ je VP nad $\mathbb{C}$
  - ako su $f$ i $g$ [[Linearni funkcional|linearni funkcionali]] tada je $\mathrm{A}(x,\ y):=f(x)\,g(y)$ bilinearna forma.
  - ako je $f$ [[Linearni funkcional|linearni funkcionali]], a $g$ je antilinearni funkcional $\big(\ \text{tj. } \ \ g(\lambda\,x)=\overline{\lambda}\,g(x)\quad\forall x\in V\quad\forall\lambda\in\mathbb{C} \ \big)$ tada je $\mathrm{A}(x,\ y):=f(x)\,g(y)$ hermitska bilinearna forma.

### Matrica bilinearne forme

Napomena: [[Koordinatizacija. Zavisnost koordinata vektora o bazi|koordinatizacija]], [[Matrica#Hermitsko konjugovanje|hermitsko konjugovanje]]

Teorema. Neka je $e$ baza VP-a $V.$
- $\mathcal{A}$ je matrica bilinearne forme $\mathrm{A}$ u bazi $e$ ako važi:
  $\boxed{\forall v,\ w\in V\quad \mathrm{A}(v,\ w)=\Big(\kappa_{e}(w)\Big)^{\mathrm{T}}\cdot\mathcal{A}\cdot\kappa_{e}(v)}$
  $\:$
- $\mathcal{A}$ je matrica hermitske bilinearne forme $\mathrm{A}$ u bazi $e$ ako važi:
  $\boxed{\forall v,\ w\in V\quad \mathrm{A}(v,\ w)=\Big(\kappa_{e}(w)\Big)^{*}\cdot\mathcal{A}\cdot\kappa_{e}(v)}$

Teorema. Neka je $\mathrm{A}$ hermitska bilinearna forma na [[Unitarni prostor. Euklidski prostor|unitarnom prostoru]] $V$. $\mathcal{A}$ je matrica $\mathrm{A}$ u bazi $e$, $\mathcal{B}$ je matrica $\mathrm{A}$ u bazi $f$. Tada važi 
$\boxed{\mathcal{B}=\big(T_{ef}\big)^{*}\cdot\mathcal{A}\cdot T_{ef}}$, gde je $T_{ef}$ matrica prelaska sa $e$ u $f$.

Tada su $\mathcal{A}$ i $\mathcal{B}$ [[Kvadratna matrica#Kongruentnost kompleksnih matrica|kongruentne]].

**Def**. **Rang** hermitske bilinearne forme je [[Rang matrice. Elementarne transformacije|rang]] njegove matrice u proizvoljnoj bazi.

### Kvadratne forme

**Def**. Neka je $V$ [[Vektorski prostor|vektorski prostor]] nad poljem $\mathbb{F}$. Tada preslikavanje $\mathbf{q}:\ V\to \mathbb{F}$ definisano sa $\forall v\in V\quad q(v)=\mathrm{A}(v,\ v)$ je:
- **kvadratna forma** na $\mathbb{F}=\mathbb{R}$ ako je $\mathrm{A}$ simetrična bilinearna forma.
- **hermitska kvadratna forma** na $\mathbb{F}=\mathbb{C}$ ako je $\mathrm{A}$ hermitska bilinearna forma.

Stav. $V$ je VP nad $\mathbb{R}$. Za kvadratnu formu $\mathbf{q}$ važi:
$\forall v,\,w\in V\quad \mathbf{q}(v+w)+\mathbf{q}(v-w)=2\,\mathbf{q}(w)+2\,\mathbf{q}(w)$

Stav. $V$ je VP nad $\mathbb{C}$. Za hermitsku kvadratnu formu $\mathbf{q}$ važi:
$\forall v\in V\quad \mathbf{q}(v)=\mathbf{q}(i\,v)\in\mathbb{R}$

Teorema. $V$ je VP nad poljem $\mathbb{F}.$
- $\mathbb{F}=\mathbb{R}$. Simetrična bilinearna forma $\mathrm{A}$ je određena odgovarajućem kvadratnom formom $\mathbf{q}$ $\Big(\mathbf{q}(v)=\mathrm{A}(v,\ v)\Big)$:
  $\:$
$\begin{align}\forall v,\, w\in V\quad\mathrm{A}(v,\ w)=\frac{\mathbf{q}(v+w)-\mathbf{q}(v-w)}{4}\end{align}$
$\:$
- $\mathbb{F}=\mathbb{C}$. Hermitska bilinearna forma $\mathrm{A}$ je određena odgovarajućem hermitskom kvadratnom formom $\mathbf{q}$ $\Big(\mathbf{q}(v)=\mathrm{A}(v,\ v)\Big)$:
$\:$
$\begin{align}\forall v,\, w\in V\quad\mathrm{A}(v,\ w)=\frac{\Big(\mathbf{q}(v+w)-\mathbf{q}(v-w)\Big)+i\,\Big(\mathbf{q}(v+i\,w)-\mathbf{q}(v-i\,w)\Big)}{4}\end{align}$

$\:$
**Def**. $V$ je VP nad $\mathbb{C}$. Hermitska kvadratna forma $\mathbf{q}$ je
- pozitivna ako važi $\forall v\in V\quad q(v)\geqslant0$
- strogo pozitivna ako važi $\forall v\ne\mathbf{0}\quad q(v)>0$, $\ \:$ $\mathbf{q}(\mathbf{0})=0$

Primedba: Skalarni proizvod je hermitska bilinearna forma, kojoj odgovara strogo pozitivna hermitska kvadratna forma. 
$\langle v,\ w\rangle_{\rm A}:=\mathrm{A}(v,\ w)=\Big(\kappa_{e}(w)\Big)^{*}\cdot\mathcal{A}\cdot\kappa_{e}(v)$

### Hermitska bilinearna forma u [[Unitarni prostor. Euklidski prostor|unitarnom prostoru]]

Teorema. $V$ je unitaran prostor. $\mathrm{A}$ je hermitska bilinearna forma $\ \:$ $\Leftrightarrow$ $\ \:$ $\exists!A: \ V\to V$ — [[Linearni operator u unitarnom prostoru#Klase operatora u unitarnom prostoru|hermitski operator]] takav da $\boxed{\mathrm{A}(v,\ w)= \langle A(v),\ w\rangle, \quad \forall v,\,w\in V}$