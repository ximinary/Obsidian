#fax #math #alg [deo [[Komutativan prsten sa jedinicom|poglavlja "prsten"]]]
$\:$ 

**Teorema**. Neka je $F$ [[Invertibilni elementi u prstenu. Polje i domen#^b98e89|polje]], a $G$ je <u>konačna</u> podgrupa grupe $(F\setminus\{0\},\,\cdot)$. Tada je $G$ ciklična.
> Dokaz:
> Preformulišemo  [[Konačno generisana Abelova grupa#^0889d3|stav]] za operaciju $\cdot$ :
> Ako u Abelovoj grupi $A$ reda $m$ za svako $d$, koje deli $m$, postoji najviše $d$ elemenata $a\in A$ takvih da  $a^{d}=1$, onda je $A$ ciklična. 
> 
> Neka je $G$ podgrupa grupe $(F\setminus\{0\},\,\cdot)$ reda $m\in\mathbb{N}$.
> Kako polinom $x^{d}-1$ ima najviše $d$ korena u $F$, ispunjen je uslov preformulisanog stava.
> 
> 

$\:$
Stoga je $(\mathbb{Z}_{p}\setminus\{0\},\,\cdot_{p})$ ciklična za prost broj $p$ ([[Invertibilni elementi u prstenu. Polje i domen#^9c82dc|*]]).

$\:$
**Def**. Svaki generator grupe $(\mathbb{Z}_{n}\setminus\{0\},\,\cdot_{p})$ zove se **primitivni koren po modulu** $p$.

**Stav**. Neka je $r$ primitivni koren po modulu $p$. Tada je sledeća funkcija izomorfizam:
$\mathrm{ind}_{r}:\ (\mathbb{Z}_{p}\setminus \{0\},\,\cdot_{p})\to (\mathbb{Z}_{p-1},\,+_{p-1})$ $\ \:$ def. sa $\ \:$ $\mathrm{ind}_{r}(a)=x\quad\Leftrightarrow\quad r^{x}=a$.
(stepen se odnosi na operaciju $\cdot_{p}$)
> Napomena 1: Funkcija $\mathrm{ind}_{r}(a)$ slična je funkciji $\log_{r}(a)$ u polju $\mathbb{R}$. 
> Napomena 2: Tražimo neki primitivni koren $r$ po modulu $p$ prebrojavanjem, treba da važi $\{\mathrm{ind}_{r}(1),\,\mathrm{ind}_{r}(p),\,\mathrm{ind}_{r}(p^{2}),\,\dots,\,\mathrm{ind}_{r}(p^{p-2})\}=\{0,\,1,\,2,\,\dots,\,p-2\}$

^fff6b3


> Dokaz:
> Kako $\mathbb{Z}_{p}\setminus\{0\}$ ima $p-1$ elemenata i kako $\mathbb{Z}_{p}\setminus\{0\}=⟨r⟩$
> $\forall a\in \mathbb{Z}_{p}\setminus\{0\} \quad\exists x\in \mathbb{Z}_{p-1}\quad a=r^{x}\quad\Rightarrow\quad$ $\mathrm{ind}_{r}$ jeste funkcija
> 
> homomorfizam: da li $\mathrm{ind}_{r}(a\cdot_{p}b)=\mathrm{ind}_{r}(a)+_{p-1}\mathrm{ind}_{r}(b)$?
> neka $x=\mathrm{ind}_{r}(a),\quad y=\mathrm{ind}_{r}(b)$. $\ \:$ Tada $\ \:$ $a=r^{x},\quad b=r^{y}$.
> Polaznu jednačinu možemo prepisati kao
> $\mathrm{ind}_{r}(r^{x}\cdot_{p} r^{y})=x+_{p-1}y\quad\Leftrightarrow\quad r^{x}\cdot_{p}r^{y}=r^{x\,+_{p-1}\,y}$
> što sledi iz [[Kongruentnost#^8d358b|male Fermaove teoreme]].
>
>"na": $\quad$ za $x\in \mathbb{Z}_{p-1}\quad\exists a\in \mathbb{Z}_{p}\setminus\{0\}\quad r^{x}=a$
>"1-1": $\quad$ $\mathrm{ind}_{r}(a)=x=\mathrm{ind}_{r}(b)\quad\Rightarrow\quad a=r^{x}=b$


$\:$
> Rešavanje [[Kongruentnost|kongruencija]] oblika: $x^{a}\equiv_{p} b,\quad a,\,b,\,p\in\mathbb{N},\quad p$ — prost.
> Nađemo primitivan koren $r$ po modulu $p$ ([[Primitivni koren#^fff6b3|napomena 2]]).
> Primenjujemo $\mathrm{ind}_{r}$ na kongruenciju i dobijamo
> $ay\equiv_{p-1}\mathrm{ind}_{r}(b)$, $\quad$ gde je $y=\mathrm{ind}_{r}(x)\quad\Leftrightarrow\quad r^{y}\equiv_{p} x$
> Nalazimo rešenje kongruencije $ay\equiv_{p-1}\mathrm{ind}_{r}(b)$ pa ubacujemo $y$ u $r^{y}\equiv_{p} x$ i tako nalazimo $x$