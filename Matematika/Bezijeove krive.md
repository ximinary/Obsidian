#fax #math #geom  [deo [[Geometrija|geometrije]]]
$\:$

**Def**. Neka su $\mathrm{P}_{0},\,\mathrm{P}_{1},\,\dots,\,\mathrm{P}_{n}$ tačke ravni $(\mathbb{R}^{2})$, $n\geqslant2$. Tada
$\begin{align}\alpha_{n}(t)=\sum\limits_{i=0}^{n}\underbrace{\binom{n}{i}x^{i}(1-x)^{n-i}}_{=B_{i}^{n}(t)}\,\mathrm{P}_{i},\quad t\in[0,\,1]\end{align}$
je **Bezijeova kriva** stepena $n$ sa kontrolnim tačkama $\mathrm{P}_{0},\,\mathrm{P}_{1},\,\dots,\,\mathrm{P}_{n}$.

$B_{i}^{n}(t)$ — Bernštajnov polinom.
$\mathrm{P}_{0}\mathrm{P}_{1}\dots\mathrm{P}_{n}$ — kontrolna poligonska linija.

### Osobine
- $\alpha_{n}(0)=\mathrm{P}_{0},\quad\alpha_{n}(1)=\mathrm{P}_{n}$
- $\mathrm{P}_{0}\mathrm{P}_{1}$ je tangenta krive u tački $\mathrm{P}_{0}$
  $\mathrm{P}_{n-1}\mathrm{P}_{n}$ je tangenta krive u tački $\mathrm{P}_{n}$
- Bezijeova kriva pripada konveksnom omotaču kontrolnih tačaka
- Svaka prava ima manje ili jednako tačaka preseka sa Bezijeovom krivom nego sa kontrolnom poligonskom linijom
- Afina invarijantnost — afino preslikavanje $f$ slika Bezijeovu krivu određenu tačkama $\mathrm{P}_{0},\,\mathrm{P}_{1},\,\dots,\,\mathrm{P}_{n}$ u Bizijeovu krivu određenu tačkama $f(\mathrm{P}_{0}),\,f(\mathrm{P}_{1}),\,\dots,\,f(\mathrm{P}_{n})$

**Teorema**. Bezijeova kriva stepena 2 je deo parabole

### Algoritam De-Kasteljau
Neka je $\alpha_{n}(t)$ Bezijeova kriva određena tačkama $\mathrm{P}_{0},\,\mathrm{P}_{1},\,\dots,\,\mathrm{P}_{n}$.

Za dato $t$ treba odrediti $\alpha_{n}(t)$:

- $0$-ti korak. $\ \:$ $\mathrm{P}^{0}_{0}=\mathrm{P}_{0},\ \ \mathrm{P}^{0}_{1}=\mathrm{P}_{1},\ \ \dots,\ \ \mathrm{P}^{0}_{n}=\mathrm{P}_{n}$ — imamo $n$ tačaka
- $i$-ti korak. $\ \:$ Za svako $\ \:$ $j=\overline{0,n\!-\!i}$ $\ \:$ nalazimo $\ \:$ $\mathrm{P}^{i+1}_{j}=(t-1)\mathrm{P}^{i}_{j}+t\mathrm{P}^{i}_{j+1}$
(tj. duž $\mathrm{P}^{i}_{j}\mathrm{P}^{i}_{j+1}$ delimo u odnosu $t:1\!-\!t$).
- na $n$-tom koraku imamo vrednost $\alpha_{n}(t)=\mathrm{P}^{n}_{0}$

Pri tome tačka $t$ je podelila Bezijeovu krivu $\alpha_{n}(t)$ stepena $n$ na dve Bezijeove krive stepena $n$:
- određenu tačkama $\mathrm{P}^{0}_{0},\ \mathrm{P}^{1}_{0},\ \dots,\ \mathrm{P}^{n}_{0}$ $\ \:$ i
- određenu tačkama $\mathrm{P}^{0}_{n},\ \mathrm{P}^{1}_{n-1},\ \dots,\ \mathrm{P}^{n}_{0}$


## Povećanje stepena
Povećanjem stepena (za jedan) Bezijeove krive $\alpha_{n}(t)$ određene tačkama $\mathrm{P}_{0},\,\mathrm{P}_{1},\,\dots,\,\mathrm{P}_{n}$ uz čuvanje oblika dobijamo krivu $\alpha_{n+1}(t)$ određenu tačkama $\mathrm{Q}_{0},\,\mathrm{Q}_{1},\,\dots,\,\mathrm{Q}_{n},\,\mathrm{Q}_{n+1}$, pri tome:
- $\mathrm{Q}_{0}=\mathrm{P}_{0},\quad \mathrm{Q}_{n+1}=\mathrm{P}_{n}$ $\ \:$ — prva i poslednja tačke ostaju iste
- $\begin{align}\forall i=\overline{1,n\!-\!1}\quad\mathrm{Q}_{i}=\frac{i}{n+1}\mathrm{P}_{i-1}+\left( 1 - \frac{i}{n+1} \right)\mathrm{P}_{i}\end{align}$