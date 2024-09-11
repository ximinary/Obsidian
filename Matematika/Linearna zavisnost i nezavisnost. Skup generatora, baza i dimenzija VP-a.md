#fax #math #laag [deo poglavlja [[Vektorski prostor|"vektorski prostor"]]]
$\:$

**Def**. $0\ne B\subseteq V$. $\ \:$ $x\in V$ je **linearna kombinacija** vektora $a_{1},\,a_{2},\,\dots,\,a_{n}\in B \ \:$ ako
$\exists\alpha_{1},\,\alpha_{2},\,\dots,\,\alpha_{n}\in\mathbb{F}\ \ : \ \ x=\alpha_{1}\,a_{1}+\alpha_{2}\,a_{2}+\dots+\alpha_{n}\,a_{n}$

### Skup generatora
**Def**. Ako $\forall x\in V\ \:$ $x$ je linearna kombinacija vektora $a_{1},\,a_{2},\,\dots,\,a_{n}\in B$.
Tada je $B$ **skup generatora** VP-a $V$.

Ako je $B$ skup generatora $V$, tada važi
1. $y\in V,\ \ y\ne0\quad\Rightarrow\quad B'=B\cup\{y\}$ je skup generatora $V$
2. $z\in V$ je linearna kombinacija vektora iz $B''=B\setminus\{z\}$
   $\Rightarrow\quad B''$ je skup generatora $V$
### Linearna zavisnost i nezavisnost
**Def**. Neka je $B=\{{a_{1},\,a_{2},\,\dots,\,a_{n}\}}\subseteq V$. $B$ je **linearno nezavisan** ako jednačina  $\alpha_{1}\,a_{1}+\alpha_{2}\,a_{2}+\dots+\alpha_{n}\,a_{n}= 0,\quad \alpha_{i}\in\mathbb{F}\ \ \forall i=\overline{1,n}$
ima jedinstveno rešenje $\alpha_{1}=\alpha_{2}=\dots=\alpha_{n}=0$

$B$ je **linearno zavisan** inače.

Svojstva:
1. $B\subseteq V$. $B\cup\{0\}$ je uvek linearno zavisan.
2. $B=\{a_{1}\},\quad a_{1}\ne0\quad\Rightarrow\quad B$ je linearno nezavisan.
3. $B=\{a_{1},\,a_{2}\}$ je linearno zavisan $\:\ \Leftrightarrow\ \ \exists\lambda\in\mathbb{F}\ \ :\ \ a_{1}=\lambda\,a_{2}$
4. Podskup linearno nezavisnog skupa je linearno nezavisan.
5. Nadskup linearno zavisnog slupa je linearno zavisan.

Stav. $B=\{ a_{1},\,a_{2},\,\dots,\,a_{n} \}\not\ni0$ je podskup $V$. Tada
$B$ je linearno zavisan $\,\ \Leftrightarrow\ \ \exists i>1\ \ :\ \ a_{i}$ je lin. kombinacija $a_{1},\,a_{2},\,\dots,\,a_{i-1}$

### Baza i dimenzija 
**Def**. **Baza** VP-a $V$ je $\ \ B\subseteq V\ \:$ linearno nezavisan skup generatora $V$.

**Teorema** (o bazi). $V$ je VP nad $\mathbb{F}$. Tada
1. $\exists B\subseteq V$ baza VP-a $V$.
2. Ako su $B_{1},\,B_{2}\subseteq V$ baze VP-a $V$, tada $\exists f:B_{1}\overset{\mathrm{bijekcija}}{\longrightarrow} B_{2}$

**Def**. **Dimenzija** VP-a $V$ je kardinalni broj neke baze VP-a $V$.
Oznaka: $\dim V$

VP $V$ je konačno dimenzioni ako je $\dim V\in\mathbb{N}_{0}$

**Lema**. Neka je $B=\{ a_{1},\,a_{2},\,\dots,\,a_{n} \}$ skup generatora $V$, $S=\{ b_{1},\,b_{2},\,\dots,\,b_{m} \}\subseteq V$ je linearno nezavisan skup. Tada
$m\leqslant n\ \:$ i $\:\ \exists i_{1},\,i_{2},\,\dots\,i_{n-m}=\overline{1,n} \ \ :$
$\{ b_{1},\,b_{2}\,\dots,\,b_{m},\,a_{i_{1}},\,a_{i_{2}},\,\dots,\,a_{i_{n-m}} \}$ je baza $V$

**Stav**. $V$ je VP. $\dim V=n$. Tada:
1. $B\subseteq V,\ \ |B|>n\quad\Rightarrow\quad B$ je linearno zavisan;
2. $A\subseteq V$ je linearno nezavisan$,\ \ |A|=n\quad\Rightarrow\quad A$ je baza $V$;
3. $S$ je skup generatora $V,\ \ |S|=n\quad\Rightarrow\quad S$ je baza $V$;

$\:$

**Stav**. $S$ je skup generatora konačno dim. VP-a $V$. Tada
maksimalan linearno nezavisan podskup $S$ je baza $V$

**Stav**. $A\subseteq V$ je linearno nezavisan, $V$ je konačno dim. VP. Tada
$A$ je podskup neke baze $V$, koji moguće dopuniti do baze.

