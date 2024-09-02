#fax #math #ds1 [deo poglavlja [[Celi brojevi|"celi brojevi"]]] 
$\:$

**Def**. Neka su $a,\,b\in \mathbb{Z}$ i $m> 1$ je prirodan broj. Tada $a$ je kongruentno sa $b$ po modulu $m$ ($a\equiv_{m} b$) ako $m\,|\,(a-b)$

($a$ i $b$ daju isti ostatak pri deljenju na $m$)

[[kongr stav 1.png|Stav]]. $\equiv_{m}$ je [[Relacija ekvivalencije|relacija ekvivalencije]] na $\mathbb{Z}$

[[kongr stav 2.png|Stav]]. Ako $a\equiv_{m}a_{1}$ i $b\equiv_{m}b_{1}$, onda važi
1) $a+b\equiv_{m}a_{1}+b_{1}$
2) $a\cdot b \equiv_{m} a_{1}\cdot b_{1}$
3) $a^{k} \equiv_{m} a_{1}^{k}$, $\:$ za svako $k\in \mathbb{Z}$

Stav. Broj je deljiv sa 3 akko zbir njegovih cifara je deljiv sa 3.
> $a = a_{k}\cdot10^{k} + a_{k-1}\cdot10^{k-1} +\dots+a_{1}\cdot10 +a_{0}$,
> $a_{k},\,a_{k-1},\,\dots,\,a_{1},\,a_{0}$ su cifre broja $a$
> 
> $10\equiv_{3}1$
> $10^{2}\equiv_{3}10\equiv_{3}1$
> $10^{3}\equiv_{3}10\equiv_{3}1$
> $\dots$
> $10^{k}\equiv_{3}10\equiv_{3}1$
> 
> Tada: $a\equiv_{3}a_{k}\cdot10^{k} + a_{k-1}\cdot10^{k-1} +\dots+a_{1}\cdot10 +a_{0}\equiv_{3}$
> $\equiv_{3}a_{k} + a_{k-1} +\dots+a_{1} +a_{0}$

Oznaka. $\mathbb{Z}_{n} = \{ 0,\,1,\,\dots,\,n \}$

> Primer. Odrediti ostatak pri deljenju $2^{30}$ sa $13$.
> Treba naći $x\in\mathbb{Z}_{13}$ tako da $2^{30}\equiv_{13}x$ *
> 
> $2^{30} = \big(2^{6}\big)^{5} = \big(2^{2}\cdot2^{4}\big)^{5}$
> 
> $2^4 = 16 \equiv_{13}3$
> $2^6 = 2^{2}\cdot2^{4} \equiv_{13}4\cdot3\equiv_{13}12\equiv_{13}-1$ **
> 
> $2^{30}= \big(2^{6}\big)^{5} \equiv_{13} (-1)^{5}\equiv_{13}-1\equiv_{13}12$ 
> 
> \* U zadacima nikada ne morate računati veće stepene. Uvek je moguće faktorisati i napraviti ugneždeni stepeni (na primer $12^{21} = 3^{21}\cdot\big(2^{2}\big)^{21}=\big(3^{7}\big)^{3} \cdot\bigg(\big(2^{7}\big)^{3}\bigg)^{2} =\dots$; $7^{26} = 7\cdot\big(7^{5}\big)^{5}=7\cdot\Big(7\cdot\big(7^{2}\big)^{2}\Big)^{5}=\dots$ )
> \** Obično je cilj imati najmanji broj po modulu (u ovom slučaju u intervalu $[-6,\, 6]$), onda je lakše množiti.

Stav. $a\cdot b\equiv_{m}a \cdot c\:$ i $\:\mathrm{NZD}(m,\,a)= 1$. $\:$ Tada $b\equiv_{m}c$
>Dokaz:
>$a\cdot b\equiv_{m}a \cdot c\ \ \Rightarrow\ \ m\,|\,(a\cdot b-a\cdot c)\ \ \Rightarrow$
>$\begin{align}\Rightarrow m\,|\,a\cdot(b-c) \\ \mathrm{NZD}(m,\,a) = 1\end{align}\ \ \Rightarrow\ \ m\,|\,(b-c) \ \ \Rightarrow \ \ b\equiv_{m}c$

$\:$
### Jednačina oblika $a\,x\equiv_{m}b$
$a\,x\equiv_{m}b\ \ \Leftrightarrow\ \ m\,|\,(a\,x-b) \ \ \Leftrightarrow\ \ \exists y\in \mathbb{Z}\ : \ a\,x-b=m\,(-y)$
$a\,x+m\,y=b\:$ — [[Diofantova jednačina]], koja ima rešenja ako $\mathrm{NZD}(a,\,m)\,|\,b$

$d:=\mathrm{NZD}(a,\, m);\ a'=\frac{a}{d};\ b'=\frac{b}{d};\ m'=\frac{m}{d}$
Možemo podeliti diofantovu jednačinu sa $d$:
$a'\,x+m'\,y=b'\ \ \Leftrightarrow\ \ a'\,x\equiv_{m'}b'\:$ (ima isti skup rešenja kao i polazna jednačina)
>I metoda:
>Rešavanjem diofantove jednačine $a'\,x+m'\,y=b'$ dobijamo rešenje u obliku $x = x_{0}+m'\,t,\quad \forall t\in \mathbb{Z}$
>
> II metoda:
> U $\mathbb{Z}_{m'}$ prebrojavanjem treba naći $x_0$ koji zadovoljava jednačinu $a'\,x_{0}\equiv_{m'}b'$
> Tada rešenje je $x = x_{0}+m'\,t,\quad\forall t\in \mathbb{Z}$

>Rešenja iz $\mathbb{Z}_{m}$: $\ \ d$ rešenja
>(Ako je $x_0$  rešenje iz $\mathbb{Z}_{m'}$ onda rešenja iz $\mathbb{Z}_{m}$ su
>$x_{0},\,x_{0}+m',\,x_{0}+2m',\,\dots,\,x_{0}+(d-1)m'$)

[[kongr primer 1.png|Primeri]]

### Kineska teorema o ostacima
[[kineska teorema.png|Teorema]]. Ako $\forall i\ne j\quad a_{i} \equiv_{\mathrm{NZD}(m_{i},\,m_{j})}a_{j}$ onda sistem jednačina 
$$
\begin{cases} x\equiv_{m_{1}}a_{1}\\
x\equiv_{m_{2}}a_{2} \\
\dots \\
x\equiv_{m_{k}}a_{k}\\ \end{cases}
$$ 
ima rešenja.
Ako je $\overline x$ je jedno rešenje sistema onda su sva rešenja oblika $x = \overline x+\mathrm{NZS}(m_{1},\,m_{2},\,\dots,\,m_{k})\,t,\quad t\in \mathbb{Z}$
>Rešavanje sistema:
>Rešavamo prvu jednačinu dobijamo $x = x_{0}+m_{1}\,t$
>Ubacujemo to u drugu jednačinu, rešavamo po $t$ dobijamo: $t = t_0+m_{2}'\,s$, gde je $m_2'=\frac{\mathrm{NZS}(m_{1},\, m_{2})}{m_{1}}$ \*
>Zatim vračamo: $x = x_{0}+m_{1}\,t = x_{0}+m_{1}\,(t_0+m_{2}'\,s)=\dots$
>Ubacujemo to u treću jednačinu, rešavamo po $s$ dobijamo: $s = s_0+m_{3}'\,u$, gde je $m_3'=\frac{\mathrm{NZS}(m_{1},\, m_{2},\,m_{3})}{\mathrm{NZS}(m_{1},\,m_{2})}$ \*
>Zatim vračamo: $x = x_{0}+m_{1}\,(t_0+m_{2}'\,(s_0+m_{3}'\,u))=\dots$
>i tako dalje, dok nećemo dobiti
>$x=\overline x+\mathrm{NZS}(m_{1},\,m_{2},\,\dots,\,m_{k})\,v$
>
>(\* ne morate da učite ove razlomke, te brojevi $m'_{k}$ se dobijaju sami, rešavanjem kongruencija)

[[kongr primer 2.png|Primer 1]]
[[kongr primer 3.png|Primer 2]] 

### Ojlerova teorema
**Def**. Neka je $n>1$ prirodan broj, tada skup $\Phi(n)=\{ k\in \mathbb{N}\ | \ 1\leqslant k< n \ \ \mathrm{i}\ \ \mathrm{NZD}(k,\,n)=1\}$ je **Ojlerov skup**.
$\varphi (n) = |\Phi(n)|$ je **Ojlerova funkcija**.
>Primer:
>$\Phi(3) = \{ 1,\,2 \}\quad\quad\quad\ \ \varphi(3)=2$
>$\Phi(4) = \{ 1,\,3 \}\quad\quad\quad\ \ \varphi(4)=2$
>$\Phi(5) = \{ 1,\,2\,3\,4 \}\quad\quad\,\varphi(5)=4$
>$\Phi(6) = \{ 1,\,5 \}\quad\quad\quad\ \ \varphi(6)=2$

Teorema. $m,\,n>1,\ \ \mathrm{NZD}(m,\,n)=1\ \ \Rightarrow\ \ \varphi(m\,n)=\varphi(m)\,\varphi(n)$


[[ojlerova fja prostog broja.png|Stav]]. $p$ je prost, tada $\varphi(p^{k})=p^{k}-p^{k-1}$

Iz [[Prost broj#Osnovna teorema aritmetike|osnovne teoreme aritmetike]]: $n = p_{1}^{\alpha_{1}}\,p_{2}^{\alpha_{2}}\,\dots\,p_{k}^{\alpha_{k}}$
Tada $\varphi(n)=\varphi(p_{1}^{\alpha_{1}})\,\varphi(p_{2}^{\alpha_{2}})\,\dots\,\varphi(p_{k}^{\alpha_{k}})=$
$= (p_{1}^{\alpha_{1}}-p_{1}^{\alpha_{1}-1})\,(p_{2}^{\alpha_{2}}-p_{2}^{\alpha_{2}-1})\,\dots\,(p_{k}^{\alpha_{k}}-p_{k}^{\alpha_{k}-1})=$
$\begin{align}=n\,\bigg(1-\frac{1}{p_{1}}\bigg)\,\bigg(1-\frac{1}{p_{2}}\bigg)\,\dots\,\bigg(1-\frac{1}{p_{k}}\bigg)\end{align}$

[[ojlevova teorema.png|Teorema]] (Ojlerova). $n > 1\:$ i $\:a$ su prirodni brojevi i $\mathrm{NZD}(a,\,n)=1$.
Tada $a^{\varphi(n)}\equiv_{n}1$

Posledica (mala Fermaova teorema). $a\in \mathbb{N}$,$\ p$ je prost, $p\nmid a$. 
Tada $a^{p-1}\equiv_{p}1$

[[kongr primer 4.png|Primer]]

### Vilsonova teorema
Teorema. $p$ je prost akko $(p-1)!\equiv_{p}-1$