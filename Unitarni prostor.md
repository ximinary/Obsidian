#fax #math #laag [deo [[Linearna algebra|linearne algebre]]]

**Def**. Vektorski prostor $V$ nad poljem $\mathbb{C}$ je **unitaran** ako je definisana funkcija $\langle \,\cdot\,,\,\cdot\,\rangle:\ V\times V\to\mathbb{C}$ za koju važi: $\forall u,\,v,\,w\in V,\ \ \forall\alpha\in\mathbb{C}$
- SP1) $\ \ \langle u+v,\ w\rangle=\langle u,\ w\rangle+\langle v,\ w\rangle$
- SP2) $\ \ \langle \alpha\,u,\ v\rangle=\alpha\,\langle u,\ v\rangle$
- SP3) $\ \ \langle u,\ v\rangle=\overline{\langle v,\ u\rangle}$
- SP4) $\ \ \langle u,\ u\rangle\geqslant0$
- SP5) $\ \ \langle u,\ u\rangle=0\quad\Leftrightarrow\quad u=\mathbf{0}$

$\langle\,\cdot\,,\,\cdot\,\rangle$ se zove **skalarni proizvod** na $V$.

Dodatna svojstva:
- SP1') $\ \ \langle u,\ v+w\rangle=\langle u,\ v\rangle+\langle u,\ w\rangle$ $\quad$ (iz SP1 i SP3)
- SP2') $\ \ \langle u,\ \alpha\,v\rangle=\overline\alpha\,\langle u,\ v\rangle$ $\ \ \!\quad\quad\quad\quad\quad$ (iz SP2 i SP3)

$\:$

**Def**. Unitarni prostor nad poljem $\mathbb{R}$ (SP3 bez konjugovanja) zove se **euklidski prostor**.

### Primeri unitarnih prostora
- $\mathbb{C}\,(\mathbb{R})$
  $u=(u_{1},\,u_{2},\,\dots,\,u_{n}),\ v=(v_{1},\,v_{2},\,\dots,\,v_{n})\in\mathbb{C}\,(\mathbb{R})$
  $\langle u,\ v\rangle:=\sum\limits_{i=1}^{n}v_{i}\,\overline{w_{i}}$ — standardni skalarni proizvod.
- $V=\mathbb{M}_{n}(\mathbb{C})$, $\quad$ $\mathcal{A},\,\mathcal{B}\in V$
  $\langle \mathcal{A},\ \mathcal{B}\rangle:= \mathrm{tr}\,(\mathcal{B}^{\bf *}\mathcal{A})$ — skalarni proizvod.
- $V=\mathbb{R}^{3}[x]$, $\quad$ $p,\,q\in V$
  $\langle p,\ q\rangle:=p(0)q(0) + p'(0)q'(0) + p(1)q(1) + p'(1)q'(1)$ — skalarni proizvod.
- $V=\Big\{ (\alpha_{1},\,\alpha_{2},\,\dots,\,\alpha_{n},\,\dots)\ \Big|\ \alpha_{i}\in\mathbb{R},\ \  \forall i \in \mathbb{N}; \ \ \sum\limits_{i=1}^{\infty}|\alpha_{i}|^{2} <\infty \Big\}\subseteq\mathbb{R}^{\mathbb{N}}$
  Za $\big(\alpha_{i}\big)_{i\in\mathbb{N}}\, ,\ \big(\beta_{i}\big)_{i\in\mathbb{N}} \in V\ \:$ važi $\ \:\sum\limits_{i=1}^{\infty}\alpha_{i}\,\beta_{i}<\infty$, tada
  $\Big\langle\big(\alpha_{i}\big)_{i\in\mathbb{N}}\, ,\ \big(\beta_{i}\big)_{i\in\mathbb{N}}\Big\rangle:=\sum\limits_{i=1}^{\infty}\alpha_{i}\,\beta_{i}$ — skalarni proizvod.
### Norma i ugao

**Def**. **Norma** je funkcija $||\ \ ||:\ V\to\mathbb{R}^{+}_{0}$ def. sa $||v||= \langle v,\ v\rangle$

**Teorema** (Koši-Švarcova nejednakost).
$v,\,w\in V$, $V$ je unitarni prostor. Tada
$\big|\langle u,\ w\rangle\big|\leqslant||v||\cdot||w||$

Odakle: $\begin{align}-1\leqslant\frac{\langle v,\ w\rangle}{||v||\cdot||w||}\leqslant1\end{align}$

**Def**. Kosinus **ugla** između $v,\,w\in V$: $\ \:$ $\begin{align}\cos\widehat{(v,\,w)}=\frac{\langle v,\ w\rangle}{||v||\cdot||w||}\end{align}$

### Ortogonalnost
**Def**. $V$ je unitaran prostor. $v,\,w\in V$ su **ortogonalni** (normalni) ako $\langle v,\ w\rangle=0$.
Oznaka: $v\perp w$

$\forall v\in V\quad v\perp \mathbf{0}$,
$\mathbf{0}$ je jedinstven element $V$ za koji to važi.

**Def**. $W_{1},\,W_{2}\subseteq V$, $V$ je unitarni prostor. Tada $W_{1}$ je ortogonalan (normalan) na $W_{2}$ ako $\forall v\in W_{1}\quad \forall w\in W_{2}\quad \langle v,\ w\rangle=0$
Oznaka: $W_{1}\perp W_{2}$

**Def**. Skup $W=\{ v_{1},\,v_{2},\,\dots,\,v_{k} \}\not\ni \mathbf{0}$ je ortogonalan ako $\langle v_{i},\ v_{j}\rangle=0,\ \ \forall i\ne j=\overline{1,k}$.

Stav. Ortogonalan skup je linearno nezavisan.

### Ortonormirana baza
**Def**. Baza $e=(e_{1},\,e_{2},\,\dots,\,e_{n})$ unitarnog prostora $V$ je ortonormirana ako $\langle e_{i},\ e_{j}\rangle=\delta_{ij},\quad \forall i,\,j=\overline{1,n}$
tj važe:
- $\{ e_{1},\,e_{2},\,\dots,\,e_{n} \}$ je ortogonalan skup.
- $||e_{i}||=1,\quad\forall i=\overline{1,n}$
$\:$

**Gram-Šmitov postupak ortogonalizacije**:

$V$ je unitaran prostor.

$\begin{align}&\text{proizvolna baza }V\\&f=(f_{1},\,f_{2},\,\dots,\,f_{n})\end{align}$$\quad\ \ \xrightarrow{\text{postupak}}\ \ \quad$$\begin{align}&\text{ortonormirana baza }V\\&e=(e_{1},\,e_{2},\,\dots,\,e_{n})\end{align}$

U $k$-tom ( $\forall k=\overline{1,n}$ ) koraku važi $\mathcal{L}(f_{1},\,\dots,\,f_{k})=\mathcal{L}(e_{1},\,\dots,\,e_{k})$

Koraci: ( $\varepsilon_{k}\in\{ -1,\,1 \},\quad\forall k=\overline{1,n}$ )

$\quad$ 1\.  $\ \:$ $\begin{align}e_{1}:=\varepsilon_{1}\frac{f_{1}}{||f_{1}||}\end{align}$

$\quad$ 2\.  $\ \:$ $v_{2}:=f_{2}- \langle f_{2},\ e_{1}\rangle\,e_{1}$

$\quad\quad\quad$ $\begin{align}e_{2}:=\varepsilon_{2}\frac{v_{2}}{||v_{2}||}\end{align}$

$\quad$ 3\.  $\ \:$ $v_{3}:=f_{3}- \langle f_{3},\ e_{1}\rangle\,e_{1}- \langle f_{3},\ e_{2}\rangle\,e_{2}$

$\quad\quad\quad$ $\begin{align}e_{3}:=\varepsilon_{2}\frac{v_{3}}{||v_{3}||}\end{align}$

$\quad\quad\quad$ $\dots$

$\quad$ k\.  $\ \:$ $v_{k}:=f_{k}- \sum\limits_{i=1}^{k-1}\langle f_{k},\ e_{i}\rangle\,e_{i}$

$\quad\quad\quad$ $\begin{align}e_{k}:=\varepsilon_{k}\frac{v_{k}}{||v_{k}||}\end{align}$

$\quad\quad\quad$ $\dots$
> Oduzimamo od narednog vektora sve njegove projekcije na vektore već ortonormiranog dela baze, pa normiramo.
> 
> Dokaz: ($e$ je ortonormirana)
> Očigledno, $||e_{i}||=1,\quad\forall i=\overline{1,n}$
> Pokazati da je $\{ e_{1},\,e_{2},\,\dots,\,e_{n} \}$ ortogonalan:
> 
> indukcija po broju vektora:
> baza: $\{e_{1}\}$ je ortogonalan
> korak:  ako je $\{ e_{1},\,e_{2},\,\dots,\,e_{k-1} \}$ ortogonalan, onda
> $\begin{align}\forall j=\overline{1,k\!-\!1}\quad &\langle e_{k},\ e_{j}\rangle= \bigg\langle \frac{v_{k}}{||v_{k}||},\ e_{j}\bigg\rangle=\frac{1}{||v_{k}||}\bigg\langle f_{k}- \sum\limits_{i=1}^{k-1}\langle f_{k},\ e_{i}\rangle\,e_{i}\,,\ e_{j}\bigg\rangle =\\\\&=\frac{1}{||v_{k}||}\bigg(\langle f_{k},\ e_{j}\rangle-\sum\limits_{i=1}^{k-1}\langle f_{k},\ e_{i}\rangle\,\delta_{ij}\bigg)=\\\\&=\frac{1}{||v_{k}||}\Big(\langle f_{k},\ e_{j}\rangle-\langle f_{k},\ e_{j}\rangle\Big)=0\end{align}$
> 
> $\Rightarrow\quad e_{k}\perp e_{j},\quad\forall j=\overline{1,k\!-\!1}\quad \Rightarrow\quad\{ e_{1},\,e_{2},\,\dots,\,e_{k} \}$ je ortogonalan.

$\:$
___
Neka je $e=(e_{1},\,e_{2},\,\dots,\,e_{n})$ ortonormirana baza unitarnog prostora $V$ $\:$i$\:$ $v=\sum\limits_{i=1}^{n}v_{i}\,e_{i}\in V$. Tada

$\forall j=\overline{1,n}\quad\langle v,\ e_{j}\rangle=\bigg\langle \sum\limits_{i=1}^{n}v_{i}\,e_{i}\,,\ e_{j}\bigg\rangle=\sum\limits_{i=1}^{n}v_{i}\,\delta_{ij}=v_{j}$

Odakle: $v=\sum\limits_{i=1}^{n}\langle v,\ e_{i}\rangle\,e_{i}$

**Def**. $\forall i = \overline{1,n}\quad v_{i}= \langle v,\ e_{i}\rangle$ zovu se **Furijeovi koeficijenti** vektora $v$ u bazi $e$.
___
Teorema. $\mathcal{E}_{k}=\{ e_{1},\,\dots,\, e_{k} \}$ je ortonormirani skup unitarnog prostora $V$. Tada
- Beselova nejednakost:
$\langle v,\ v\rangle\geqslant \Big|\langle v,\ e_{1}\rangle\Big|^{2}+ \Big|\langle v,\ e_{2}\rangle\Big|^{2} + \dots + \Big|\langle v,\ e_{n}\rangle\Big|^{2}$
$\:$
Specijalno, ako je $\mathcal{E}_{k}$ baza od $V$ važi jednakost.
$\:$

- Parservalova jednakost
 $\mathcal{E}_{k}$ je baza od $V$ $\quad\Leftrightarrow$
$\Leftrightarrow\quad\forall v,\,w\in V\quad\langle v,\ w\rangle=\sum\limits_{i=1}^{n}\langle v,\ e_{i}\rangle\langle e_{i},\ w\rangle$

### Ortogonalni komplement 