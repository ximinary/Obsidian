#fax #math #alg  [deo [[Grupa|poglavlja "grupa"]]]
$\:$

[[Grupa#^9d2aa9|Abelova Grupa]] je [[Algebarska struktura|algebarska struktura]] $(G,\,+)$, gde je $G$ neprazan skup a za binarnu operaciju $+$ na $G$ važi:
- $\forall x,\,y,\,z\in G\quad(x+y)+z=x+(y+z)$
- $\forall 0\in G\quad \forall x\in G\quad 0+x=x+0=x$
- $\forall x\in G\quad\exists \overline{x}\in G\quad \overline{x}+x=x+\overline{x}=0$
- $\forall x,\,y\in G\quad x+y=y+x$

Konačno generisana grupa je grupa koja je generisana konačnim [[Grupa#^eb2fd0|skupom generatora]]. Generatori su obično dati pomoću <u>sistema jednačina</u>.

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
### Normalna forma
**Teorema**. Neka je $A$ konačno generisana Abelova grupa. Tada postoje pozitivni brojevi $d_{1},\,\dots,\,d_{k}\in \mathbb{Z}$ i $s\in \mathbb{N}_{0}$ takvi da 
$\forall i=\overline{1,k\!-\!1}\quad d_{i}\,\big|\,d_{i+1}$ $\ \:$ i $\ \:$ $\boxed{A\cong \mathbb{Z}_{d_{1}}\times\mathbb{Z}_{d_{2}}\times\dots\times\mathbb{Z}_{d_{k}}\times\mathbb{Z}^{s}}$.

Brojevi $d_{1},\,d_{2},\,\dots,\,d_{k}$ zovu se **invarijantni delitelji**, a prikaz u zaokruženom obliku **normalna forma** 
### Generatori zadati sistemom jednačina/matricom
Neka je Abelova grupa $A$ zadata generatorima $x_{1},\,x_{2},\,\dots,\,x_{n}$ za koje važe
$\begin{align}a_{11}x_{1}+a_{12}x_{2}+\dots+a_{1n}x_{n}&=0\\a_{21}x_{1}+a_{22}x_{2}+\dots+a_{2n}x_{n}&=0\\&\dots\\a_{m1}x_{1}+a_{m2}x_{2}+\dots+a_{mn}x_{n}&=0\end{align}$

$A=(a_{ij})\in \mathbb{M}_{mn}(\mathbb{Z}),\quad \mathbf{x}=\left(\begin{array}{}x_{1}\\x_{2}\\\dots\\x_{n}\end{array}\right)$
Tada kraće: $A\mathbf{x}=\mathbf{0}$

Elementarne transformacije:
- množenje vrste/kolone sa $-1$
- dodavanje neke vrste/kolone pomnožene skalarom drugoj vrsti/koloni.
- promena mesta vrsta/kolona

**Teorema**. $A\in \mathbb{M}_{mn}(\mathbb{Z})$. Tada postoje invertibilne matrice $P\in \mathbb{M}_{m}(\mathbb{Z})$ i $Q\in\mathbb{M}_{n}(\mathbb{Z})$ tako da $PAQ=A^{0}$, gde je
$A^{0}=\left(\begin{array}{c|c} \begin{array}{}d_{1}&0&\cdots&0\\0&d_{2}&\dots&0\\\dots&\dots&\dots&\dots\\0&0&\dots&d_{k}\\\end{array}&\mathbf{0}\\\hline \mathbf{0}&\mathbf{0}\end{array}\right)$ $\quad$ i $\ \:$ $\forall i=\overline{1,k\!-\!1}\quad d_{i}\,\big|\,d_{i+1}$

$\:$
> Množenje elementarnim matricama sleva odgovara transformacijama nad vrstama (koje ne menjaju generatore).
> Množenje elementarnim matricama zdesna odgovara transformacijama nad kolonama (koje menjaju generatore).

Neka je sistem predstavljen sa $A\mathbf{x}=\mathbf{0}$.
Tada ako $PAQ=A^{0}$, množimo gornju jednačinu sa $P$ sleva:
$PA\mathbf{x}=\mathbf{0}$
$PA(QQ^{-1})\mathbf{x}=\mathbf{0}$
$A^{0}(Q^{-1}\mathbf{x})=\mathbf{0}$
$\mathbf{y}:=Q^{-1}\mathbf{x}$ $\ \:$ — $\ \:$ novi generatori; novi sistem generatora: $A^{0}\mathbf{y}=\mathbf{0}$

Matrično:
$\left(\begin{array}{c|c}A&\mathbf{0}\\\hline I&\begin{array}{}x_{1}\\\dots\\x_{n}\end{array}\end{array}\right)\xrightarrow{\text{transformacije vrsta}}\left(\begin{array}{c|c}PA&\mathbf{0}\\\hline I&\begin{array}{}x_{1}\\\dots\\x_{n}\end{array}\end{array}\right)\xrightarrow{\text{transformacije kolona}} \left(\begin{array}{c|c}PAQ&\mathbf{0}\\\hline Q&\begin{array}{}x_{1}\\\dots\\x_{n}\end{array}\end{array}\right)\xrightarrow{\text{transformacije vrsta}}\left(\begin{array}{c|c}PAQ&\mathbf{0}\\\hline I&\begin{array}{}y_{1}\\\dots\\y_{n}\end{array}\end{array}\right)$


> U donjem desnom uglu dobijamo nove generatore.
> U gornjem levom uglu dobijamo $A^{0}=PAQ$ relacije među novim generatorima.

> Čitamo $A^{0}=\left(\begin{array}{c|c} \begin{array}{}d_{1}&0&\cdots&0\\0&d_{2}&\dots&0\\\dots&\dots&\dots&\dots\\0&0&\dots&d_{k}\\\end{array}&\mathbf{0}\\\hline \mathbf{0}&\mathbf{0}\end{array}\right)$:
> $A\cong \mathbb{Z}_{d_{1}}\times\mathbb{Z}_{d_{2}}\times\dots\times\mathbb{Z}_{d_{k}}\times\mathbb{Z}^{n-k}$
> 
> > Nekoliko prvih $d_{i}$ mogu biti jednake $1$, tada oni odgovaraju grupi $\{0\}$, koju ne pišemo u navedenom proizvodu.