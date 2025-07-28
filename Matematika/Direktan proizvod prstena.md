#fax #math #alg [deo [[Komutativan prsten sa jedinicom|poglavlja "prsten"]]]
$\:$ 

**Def**. Neka su $(A_{1},\,+^{1},\,\cdot^{1}),\,\dots,\,(A_{n},\,+^{n},\,\cdot^{n})$ komutativni prsteni sa jedinicom. Direktni proizvod ovih prstena je $(B,\,+,\,\cdot)$ je dat sa:
- $B=A_{1}\times\dots \times A_{n}$
- $(a_{1},\,\dots,\,a_{n})+(a'_{1},\,\dots,\,a'_{n})=(a_{1}+^{1}a'_{1},\,\dots,\,a_{n}+^{n}a'_{n})$
- $(a_{1},\,\dots,\,a_{n})\cdot(a'_{1},\,\dots,\,a'_{n})=(a_{1}\cdot^{1}a'_{1},\,\dots,\,a_{n}\cdot^{n}a'_{n})$

$(B,\,+,\,\cdot)$ jeste komutativan prsten sa jedinicom
- $1_{B}=(1_{A_{1}},\,\dots,\,1_{A_{n}})$
- $0_{B}=(0_{A_{1}},\,\dots,\,0_{A_{n}})$.

$\:$
>Napomena: [[Potprsten i ideal#Kongruencija po idealu|kongruencije]]

$\:$
**Stav**. Neka su $m_{1},\,\dots,\,m_{n}\in \mathbb{N}_{0}$ takvi da $\forall i\ne j\quad\mathrm{NZD}(m_{i},\,m_{j})=1$. Tada
$\mathbb{Z}/(m_{1}\cdots m_{n})\mathbb{Z}\cong (\mathbb{Z}/m_{1}\mathbb{Z})\times\dots\times(\mathbb{Z}/m_{n}\mathbb{Z})$ ^0f9bac
> Dokaz:
> Definišemo [[Homomorfizam komutativnih prstena sa jedinicom|homomorfizam]] $f:\ \mathbb{Z}\to (\mathbb{Z}/m_{1}\mathbb{Z})\times\dots\times(\mathbb{Z}/m_{n}\mathbb{Z})$ sa $f(x):=(x+m_{1}\mathbb{Z},\,\dots,\,x+m_{n}\mathbb{Z})$
> 
> Nađemo $\mathrm{Ker}\,f$, tj. sve $x\in \mathbb{Z}$ za koje važi $f(x)=(m_{1}\mathbb{Z},\,\dots,\,m_{n}\mathbb{Z})$
> Stoga, $\begin{array}{}x+m_{1}\mathbb{Z}=m_{1}\mathbb{Z}\\\dots\\x+m_{n}\mathbb{Z}=m_{n}\mathbb{Z}\end{array}\quad\Rightarrow\quad x=pm_{1}\cdots m_{n},\ \ p\in \mathbb{Z}$, jer su $m_{i}$ uzajamno prosti.
> 
> Dobili smo da $\mathrm{Ker}\, f=(m_{1}\cdots m_{n})\mathbb{Z}$
> Jasno je da je $f$ "na".
> 
> Koristeći [[Homomorfizam komutativnih prstena sa jedinicom#^023ba8|teoremu o izomorfizmu]] $f$ indukuje <u>izomorfizam</u> $\tilde{f}:\ \mathbb{Z}/\mathrm{Ker}\,f\to \mathrm{Im}\,f$ 
> detaljnije $\tilde{f}:\ \mathbb{Z}/(m_{1}\cdots m_{n})\mathbb{Z}\to (\mathbb{Z}/m_{1}\mathbb{Z})\times\dots\times(\mathbb{Z}/m_{n}\mathbb{Z})$

$\:$
**Posledica**. Neka su $m_{1},\,m_{2},\,\dots,\,m_{n}\in \mathbb{N}$ par po par uzajamno prosti brojevi i neka  $x_{1},\,x_{2},\,\dots,\,x_{n}\in \mathbb{Z}$. Tada $\exists x\in \mathbb{Z}$ takav da
$x\equiv_{m_{1}} x_{1},\quad x\equiv_{m_{2}}x_{2},\quad\dots,\quad x\equiv_{m_{n}}x_{n}$.
Ako je $x'$ neki drugi broj koji zadovoljava taj sistem, onda $x'\equiv_{m_{1}m_{2}\cdots m_{n}} x$

$\:$
**Stav**. Važi $U(A_{1}\times\dots\times A_{n})=U(A_{1})\times\dots\times U(A_{n})$. $\quad$ ([[Invertibilni elementi u prstenu. Polje i domen#^d07f3d|*]]) ^eaafd8
> Dokaz: Neka $A=A_{1}\times\dots\times A_{n},\quad a=(a_{1},\,\dots,\,a_{n})\in A$. Tada
> $\begin{align}a\in U(A)\quad&\Leftrightarrow\quad \exists b=(b_{1},\,\dots,\,b_{n})\in A\quad a\cdot b = 1_{A}\\&\Leftrightarrow\quad \forall i=\overline{1, n}\quad\exists b_{i}\in A_{i}\quad a_{i}\cdot b_{i}=1_{A_{i}}\\&\Leftrightarrow\quad \forall i=\overline{1,n}\quad a_{i}\in U(A_{i})\\&\Leftrightarrow\quad a\in U(A_{1})\times\dots\times U(A_{n})\end{align}$

$\:$
**Teorema**. Neka su $m_{1},\,m_{2},\,\dots,\,m_{n}\in \mathbb{N}$ par po par uzajamno prosti brojevi. Tada
- $\mathbb{Z}_{m_{1}\cdots m_{n}}\cong \mathbb{Z}_{m_{1}}\times\dots\times\mathbb{Z}_{m_{n}}$
- $\varphi(m_{1}\cdots m_{n})=\varphi(m_{1})\cdots\varphi(m_{n})$ $\quad$ ($\varphi$ je Ojlerova fja)
 
> Dokaz: prvo tvrđenje sledi iz [[Direktan proizvod prstena#^0f9bac|stava]] i [[Homomorfizam komutativnih prstena sa jedinicom#^f4e2f8|stava]];
> drugo iz [[Homomorfizam komutativnih prstena sa jedinicom#^8cba06|stava]], [[Direktan proizvod prstena#^eaafd8|stava]] i činjenice $\varphi(m)=\big|U(\mathbb{Z}_{m})\big|$.