#not_linked
$\:$

**Def**. **Grupa** je [[Algebarska struktura|algebarska struktura]] $(G,\,\cdot)$, gde je $G$ neprazan skup a za binarnu operaciju $\cdot$ na $G$ važi:
- $\forall x,\,y,\,z\in G\quad(x\cdot y)\cdot z=x\cdot(y\cdot z)$
- $\forall e\in G\quad \forall x\in G\quad e\cdot x=x\cdot e=x$
- $\forall x\in G\quad\exists \overline{x}\in G\quad \overline{x}\cdot x=x\cdot\overline{x}=e$

$e$ je **neutral** grupe
**Stav**. Postoji jedinstven neutral.
> Dokaz: pps $e$ i $f$ su neutrali tada 
> ako je $e$ neutral onda $e\cdot f=f$
> ako je $f$ neutral onda $e\cdot f=e$
> odakle $e=f$, kontradikcija

$\overline{x}$ je **inverz** za $x$. Inverz se često označava sa $x^{-1}.$
**Stav**. Za svaki element grupe postoji jedinstven inverz.

**Def**. **Abelova** (komutativna) **grupa** je grupa $(G,\,\cdot)$ za koju važi: 
- $\forall x,\,y\in G\quad x\cdot y=y\cdot x$

Proizvod $\prod\limits_{i=1}^{n}x_{i},\quad x_{i}\in G$ se definiše rekurentnom formulom:
$\begin{cases}\prod\limits_{i=1}^{n}x_{i}=e,&n=0\\\prod\limits_{i=1}^{n}x_{i}=\prod\limits_{i=1}^{n-1}x_{i}\cdot x_{n},&n>0\end{cases}$

oznake:
$\prod\limits_{i=1}^{n}x_{i}=(x_{1}\cdots x_{n})$
$\prod\limits_{i=1}^{n}x=x^{n}$

pri tome za $-n<0$ definišemo $x^{-n}=\big(x^{-1}\big)^{n}$,
i važi $x^{0}=e$

**Def**. Za konačnu grupu možemo formirati **Kejlijevu tablicu**: vrste i kolone označavamo sa elementima grupe, a u preseku vrste označene sa $a$ i kolone označene sa $b$ zapisujemo element $a\cdot b$.


### Svojstva grupe
**Stav**. Neka je $(G,\,\cdot)$ grupa, $\ \:$ $n\geqslant2,\quad1\leqslant r<n$. 
Tada $(x_{1}\cdots x_{r})\cdot(x_{r+1}\cdots x_{n})=(x_{1}\cdots x_{n})$

**Stav**. Neka je $(G,\,\cdot)$ Abelova grupa. Tada ako $\{1,\,2,\,\dots,\,n\}=\{i_{1},\,i_{2},\,\dots,\,i_{n}\}$ onda $(x_{i_{1}}\cdots x_{i_{n}})=(x_{1}\cdots x_{n})$

**Stav**. Neka je $(G,\,\cdot)$ grupa. Tada $\big(x^{-1}\big)^{-1}$

**Stav**. Neka je $(G,\,\cdot)$ grupa. Tada $(x_{1}\cdots x_{n})^{-1}=x_{n}^{-1}\cdots x_{1}^{-1}$

**Stav**. Neka je $(G,\,\cdot)$ grupa. Tada 
- jednačina $a\cdot x=b$ ima jedinstveno rešenje $x=a^{-1}\cdot b$
- jednačina $x\cdot a=b$ ima jedinstveno rešenje $x=b\cdot a^{-1}$

**Stav**. Neka je $(G,\,\cdot)$ grupa. Tada $(a\,x\,a^{-1})^{n}=a\,x^{n}\,a^{-1}$

$\:$
**Def**. $a\,x\,a^{-1}$ je **konjugovan** elementu $x$

$\:$
**Stav**. Neka je $(G,\,\cdot)$ grupa, $\:$ $x\in G$, $\:$ $n,\,m\in\mathbb{Z}$. $\:$ Tada
- $x^{n}\cdot x^{m}=x^{n+m}$
- $\big(x^{n}\big)^{m}=x^{nm}$