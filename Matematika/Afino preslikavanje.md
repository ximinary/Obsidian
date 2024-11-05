#fax #math #geom  [deo [[Geometrija|geometrije]]]
$\:$

**Def**. Neka je $\overline{f}: \mathbb{V}\to\mathbb{V}$ [[Linearni operator|linearni operator]] u prostoru $\mathbb{V}$ kojem je pridružen prostor tačaka $\mathbb{E}$. **Afino preslikavanje** indukovano preslikavanjem $\overline{f}$ je preslikavanje $f:\mathbb{E\to \mathbb{E}}$, takvo da važi:
$\mathrm{M}'=f(\mathrm{M}),\,\mathrm{N}'=f(N)\quad \Rightarrow\quad \overline{f}(\overrightarrow{\rm MN})=\overrightarrow{\rm M'N'}$

**Lema**. Svako afino preslikavanje u fiksiranom [[Reper. Koordinate vektora i tačke|reperu]] $\mathrm{O}e$ ima oblik:
$\big[f(\mathrm{M})\big]_{\mathrm{O}e}=A\cdot\big[\mathrm{M}\big]_{\mathrm{O}e}+b$, $\quad\quad\quad\quad\quad\quad(1)$ 
- gde je $A$  matrica preslikavanja $\overline{f}$ u bazi $e$,
  tj. kolone $A$ su redom slike vektora baze $e$,
- $b=\big[f(\mathrm{O})\big]_{\mathrm{O}e}$ — koordinate slike koordinatnog početka

> Dokaz:
> $\begin{align}\big[f(\mathrm{M})\big]_{\mathrm{O}e}-\big[f(\mathrm{O})\big]_{\mathrm{O}e}&=\big[\overrightarrow{f(\mathrm{O})f(\mathrm{M})}\big]_{e} = \big[\overline{f}(\overrightarrow{\rm OM})\big]_{e}=\big[\overline{f}\big]_{e}\big[\overrightarrow{\rm OM}\big]_{e}=\\&=A\cdot\big[M\big]_{\mathrm{O}e}\end{align}$

Formula (1) može se posmatrati kao:
- koordinate iste tačke u različitim bazama \[[[Reper. Koordinate vektora i tačke#Transformacija koordinata tačaka|*]]];
- koordinate slike afinog preslikavanja u fiksiranoj bazi.

Skup afinih preslikavanja u $n$-dim prostoru čine <u>grupu</u> $A\!f\!f_{n}(\mathbb{R})$


### Izometrije

**Def**. **Izometrija** u euklidovskom prostoru $\mathbb{E}$ je preslikavanje koje čuva dužinu.
**Def**. **Kretanje** je izometrija koja čuva orijentaciju tj. $\det A=1$.

Translacija, rotacija i refleksija u izometrije.
Translacija i rotacija su kretanja.

**Teorema**. Svaka izometrija prostora $\mathbb{E}^{n}$ je afino preslikavanje.

**Teorema**. Afino preslikavanje je izometrija $\quad\Leftrightarrow\quad$ $A\,A^{\rm T}=A^{\rm T}A=E$, gde je $A$ matrica odgovarajućeg LO.

**Teorema**. Sledeća tvrđenja su ekvivalentna za $f: \mathbb{E}^{n}\to\mathbb{E}^{n}$
- $f$ je izometrija (čuva dužine)
- $f$ [[Unitarni prostor#Izomorfnost unitarnih prostora|čuva skalarni proizvod]]
- $f$ preslikava ortonormiranu bazu u ortonormiranu bazu.
- 
### [[Afino preslikavanje u ravni]]
### [[Afino preslikavanje u prostoru]]