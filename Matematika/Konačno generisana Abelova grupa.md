#fax #math #alg  [deo [[Grupa|poglavlja "grupa"]]]
$\:$

[[Grupa#^9d2aa9|Abelova Grupa]] je [[Algebarska struktura|algebarska struktura]] $(G,\,+)$, gde je $G$ neprazan skup a za binarnu operaciju $+$ na $G$ važi:
- $\forall x,\,y,\,z\in G\quad(x+y)+z=x+(y+z)$
- $\forall 0\in G\quad \forall x\in G\quad 0+x=x+0=x$
- $\forall x\in G\quad\exists \overline{x}\in G\quad \overline{x}+x=x+\overline{x}=0$
- $\forall x,\,y\in G\quad x+y=y+x$

Konačno generisana grupa je grupa koja je generisana konačnim [[Grupa#^eb2fd0|skupom generatora]]. Generatori su obično dati pomoću <u>skupa jednačina</u>.

### Suma i direktna suma
**Def**. Neka je $A$ Abelova grupa, $B,\,C\leqslant A$. Tada je **suma podgrupa** $B+C=\{b+c\ |\ b\in B,\ c\in C\}$ najmanja podgrupa od $A$ koja sadrži kao podgrupu i $B$ i $C$.
Suma je **direktna** ako $B\cap C=\{0\}$. Oznaka: $B\oplus C$.
> Napomena: Svaki element iz $B\oplus C$ moguće je na <u>jedinstven</u> način predstaviti kao zbir jednog elementa iz $B$ i jednog elementa iz $C$.

$\:$
Suma više podgrupa:
$B_{1},\,B_{2},\,\dots,\,B_{k}\leqslant A$. $\ \:$ $B_{1}+B_{2}+\dots+B_{k}=\{b_{1}+b_{2}+\dots+b_{k}\ |\ b_{1}\in B_{1},\ b_{2}\in B_{2},\ \dots,\ b_{k}\in B_{k}\}$
Ova suma je direktna ako je svaki njen element moguće predstaviti na <u>jedinstven</u> način kao zbir po jedan element iz svake od podgrupa $B_{1},\,B_{2},\,\dots,\,B_{k}.$

**Stav**. Neka je $A$ Abelova grupa. Suma podgrupa $B_{1},\,\dots,\,B_{k}$ grupe $A$ je direktna akko $\forall i=\overline{2,n}\quad (B_{1}+\dots+B_{i-1})\cap B_{i}=\{0\}$
> Dokaz: $\boxed\Rightarrow$ PPS: neka je $B_{1}+\dots+B_{k}$ direktna i neka $b\in(B_{1}+\dots+B_{i-1})\cap B_{i}$, $\ \:$ $b\ne 0,\ i=\overline{2,n}$.
> Tada $b=b_{1}+\dots+b_{i-1}=b_{i},\quad$ za $b_{j}\in B_{j}$.
> Što su dva različita prikaza $b$ u direktnoj sumi $B_{1}+\dots+B_{k}$. Kontradikcija.
> 
> $\boxed\Leftarrow$ PPS: neka $\forall i=\overline{2,n}\quad (B_{1}+\dots+B_{i-1})\cap B_{i}=\{0\}$
> i neka $b\in B_{1}+\dots+B_{k}$ ima bar dva prikaza: $b=b_{1}+\dots+b_{k}=b'_{1}+\dots+b'_{k}$ $\quad$ za $b_{j},\,b'_{j}\in B_{j}$ (nisu svi $b_{j}$ i $b'_{j}$ jednaki). Tada $0=b-b=(b_{1}-b'_{1})+\dots+(b_{k}-b'_{k})$
> Neka $j$ je takvo da je najveći broj za koji $b_{j}\ne b'_{j}$
> Odakle, $\underbrace{(b_{1}-b'_{1})+\dots+(b_{j-1}-b'_{j-1})}_{\in B_{1}+\dots+ B_{j-1}}=\underbrace{b'_{j}-b_{j}}_{\in B_{j}}$
> a jer $j=\overline{2,n}$ $\ \:$ važi $\ \:$ $(B_{1}+\dots+B_{j-1})\cap B_{j}=\{0\}$. Stoga $b'_{j}=b_{j}$. Kontradikcija.

$\:$
**Stav**. Neka je $A$ Abelova grupa, $B_{1},\,B_{k},\,\dots,\,B_{k}\leqslant A$. Tada
$B_{1}\oplus B_{2}\oplus\dots\oplus B_{k}\cong B_{1}\times B_{2}\times\dots\times B_{k}$.
> Dokaz: Izomorfizam $f:\ B_{1}\times B_{2}\times\dots\times B_{k}\to B_{1}\oplus B_{2}\oplus\dots\oplus B_{k}$ $\ \:$ definisan sa $\ \:$ $f(b_{1},\,b_{2},\,\dots,\,b_{k})=b_{1}+b_{2}+\dots+b_{k}$
> 
> homomorfizam: $\begin{align}f(b_{1}+b'_{1},\,b_{2}+b'_{2},\,\dots,\,b_{k}+b'_{k})&=(b_{1}+b'_{1})+(b_{2}+b'_{2})+\dots+(b_{k}+b'_{k})=\\&=(b_{1}+b_{2}+\dots+b_{k})+(b'_{1}+b'_{2}+\dots+b'_{k})=\\&=f(b_{1},\,b_{2},\,\dots,\,b_{k})+f(b'_{1},\,b'_{2},\,\dots,\,b'_{k})\end{align}$
> (jer u $A$ važi i asocijativnost i komutativnost)
> 
> "na": jasno je da ne postoji element koji ne možemo predstaviti odgovarajućem zbirom.
> "1-1": jasno je da je to predstavljanje jednoznačno iz definicije direktne sume. 

$\:$
**Teorema**. Neka je $A$ konačno generisana Abelova grupa. Tada postoje pozitivni brojevi $d_{1},\,\dots,\,d_{k}\in \mathbb{Z}$ i $s\in \mathbb{N}_{0}$ takvi da 
$\forall i=\overline{1,k\!-\!1}\quad d_{i}\,\big|\,d_{i+1}$ $\ \:$ i $\ \:$ $\boxed{A\cong \mathbb{Z}_{d_{1}}\times\mathbb{Z}_{d_{2}}\times\dots\times\mathbb{Z}_{d_{k}}\times\mathbb{Z}^{s}}$.

### Generatori i relacije
