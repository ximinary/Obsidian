#fax #math #laag [deo poglavlja [[Unitarni prostor|"unitarni prostor"]]]
$\:$

$V$ je unitarni prostor, $\{ v_{1},\,v_{2},\,\dots,\,v_{n} \}\subseteq V$

$\{ v_{1},\,v_{2},\,\dots,\,v_{n} \}$ je [[Linearna zavisnost i nezavisnost. Skup generatora, baza i dimenzija VP-a#Linearna zavisnost i nezavisnost|linearno nezavisan]] ako jednačina $\lambda_{1}\,v_{1}+\lambda_{2}\,v_{2}+\dots+\lambda_{n}\,v_{n}=0$ ima jedinstveno rešenje: $\lambda_{i}=0,\ \ \forall i=\overline{1,n}$

Skalarno množimo jednačinu redom sa $v_{1},\,v_{2},\,\dots,\,v_{n}$:

$\begin{align}\langle v_{1},\ v_{1}\rangle\,\lambda_{1}+\langle v_{2},\ v_{1}\rangle\,\lambda_{2}+\dots+\langle v_{n},\ v_{1}\rangle\,\lambda_{n}&=0\\\langle v_{1},\ v_{2}\rangle\,\lambda_{1}+\langle v_{2},\ v_{2}\rangle\,\lambda_{2}+\dots+\langle v_{n},\ v_{2}\rangle\,\lambda_{n}&=0\\\dots\\\langle v_{1},\ v_{n}\rangle\,\lambda_{1}+\langle v_{2},\ v_{n}\rangle\,\lambda_{2}+\dots+\langle v_{n},\ v_{n}\rangle\,\lambda_{n}&=0\end{align}$

Matrica ovog sistema se zove **Gramova matrica**:
$G=G(v_{1},\,v_{2},\,\dots,\,v_{n})=\left(\begin{array}{}\langle v_{1},\ v_{1}\rangle&\langle v_{2},\ v_{1}\rangle&\dots&\langle v_{n},\ v_{1}\rangle\\\langle v_{1},\ v_{2}\rangle&\langle v_{2},\ v_{2}\rangle&\dots&\langle v_{n},\ v_{2}\rangle\\\dots&\dots&\dots&\dots\\\langle v_{1},\ v_{n}\rangle&\langle v_{2},\ v_{n}\rangle&\dots&\langle v_{n},\ v_{n}\rangle\end{array}\right)$

**Gramova determinanta**: $\det G=\Gamma(v_{1},\,v_{2},\,\dots,v_{n})$
$\:$

- $\{ v_{1},\,v_{2},\,\dots,\,v_{n} \}$ je linearni nezavisan ako $\Gamma(v_{1},\,v_{2},\,\dots,\,v_{n})\ne0$

Teorema. $V$ je unitaran, $\{ v_{1},\,v_{2},\,\dots,\,v_{n} \}\subseteq V$. Tada:
- $\Gamma\left( v_{1},\,v_{2},\,\dots,v_{i}+\sum\limits_{j\ne i} \lambda_{j}\,v_{j},\dots,v_{n} \right)=\Gamma(v_{1},\,v_{2},\,\dots,\,v_{i},\,\dots,\,v_{n})$
  $\forall i=\overline{1,n},\quad \lambda\in\mathbb{C}$
  $\:$
- Ako $v_{n}\perp v_{1},\,v_{2},\,\dots,\,v_{k-1}$, onda
  $\Gamma(v_{1},\,v_{2},\,\dots,\,v_{n-1},\,v_{n})=||v_{n}||^{2}\cdot\Gamma(v_{1},\,v_{2},\,\dots,\,v_{n-1})$
  $\:$
- $\Gamma(v_{1},\,v_{2},\,\dots,\,v_{n})\geqslant0$
$\:$

Teorema.  $V$ je unitaran, $\{ v_{1},\,v_{2},\,\dots,\,v_{n} \}\subseteq V$. Tada 
$\Gamma(v_{1},\,v_{2},\,\dots,\,v_{n})=\Big(\mathrm{Vol}_{k}\,\mathcal{P}(v_{1},\,v_{2},\,\dots v_{n})\Big)^{2}$
— kvadrat $k$-zapremine $k$-paralelepipeda određenog vektorima $v_{1},\,v_{2},\,\dots,\,v_{n}$