#fax #math #laag [deo poglavlja[[Linearni operator|"linearni operator"]]]
$\:$

Napomene: [[direktna i inverzna slika skupa]], [[Potprostor. Operacije nad potprostorima|potprostor]]

Stav. $A\in \mathrm{Hom}(U,\,V)$. Tada
- $U_{1}\leqslant U\quad\Rightarrow\quad A[U_{1}] \leqslant V$
- $V_{1}\leqslant V\quad\Rightarrow\quad A^{-1}[V_{1}] \leqslant U$
### Slika i jezgro
$\:$
**Def**. $A\in \mathrm{Hom}(U,\,V)$. Tada
- **slika** lin. operatora $A$ je $\ \mathrm{Im}\,A=\Big\{ A(u)\ \Big|\ u\in U \Big\}=A[U]\subseteq V$
- **jezgro** lin. operatora $A$ je $\ \mathrm{Ker}\,A=\Big\{ u\in U\ \Big| \ A(u) = \mathbf{0} \Big\}= A^{-1}[\mathbf{0}]\subseteq U$

Stav. $A\in \mathrm{Hom}(U,\,V)$. Tada
- $\mathrm{Im}\,A\leqslant V$
- $\mathrm{Ker}\,A\leqslant U$
- $\mathrm{Ker}\,A=\{ 0 \}\quad\Leftrightarrow\quad A$ je monomorfizam (1-1)
### Rang i defekt
**Def**. $A\in \mathrm{Hom}(U,\,V)\quad\dim U,\,V\in\mathbb{N}$. Tada
- **rang** $A$ je $\mathrm{rang}\,A=\mathrm{Rank}\,A=\dim(\mathrm{Im}\,A)$
- **defekt** $A$ je $\mathrm{defekt}\,A=\mathrm{Nullity}\,A=\dim(\mathrm{Ker}\,A)$

**Teorema** (o rangu i defektu). $A\in \mathrm{Hom}(U,\,V)\quad\dim U,\,V\in\mathbb{N}$. Tada $\boxed{\mathrm{rang}\,A\,+\,\mathrm{defekt}\,A\,=\,\dim U}$

Posledica 1. $L$ je pravi potprostor od konačnodimenzionog VP-a $U$. Tada $L$ i $U$ nisu izomorfni: 
- $A: \ L\to U$ ne može biti epimorfizam (na)
- $B: \ U\to L$ ne može biti monomorfizam (1-1)

Posledica 2. $V$ je konačnodimenzioni VP, $A\in \mathrm{Hom}\,V$. Tada su ekvivalentne:
- $A$ je epimorfizam (na)
- $A$ je monomorfizam (1-1)
- $A$ je izomorfizam (bijekcija)

Posledica 3. $V$ je konačnodimenzioni VP, $A,\, B\in \mathrm{Hom}\,V$, takve da $\left[
\begin{array}{}A\circ B=id_V \\ A\circ B=id_V\end{array}\right.$
Tada su $A$ i $B$ izomorfizmi i  $B=A^{-1}$

___
Stav (svojstva projektora). $V$ je konačnodimenzioni VP, $P\in \mathrm{Hom}\,V$ i važi $P\circ P=P$. Tada
- $x\in \mathrm{Im}\,P\quad\Leftrightarrow\quad P(x)=x$
- $P\ne \mathrm{id}_{V}\quad\Rightarrow\quad P$ nije izomorfizam
- $V = \mathrm{Im}\,P\oplus\mathrm{Ker}\,P$

___
Stav. $A,\,B\in \mathrm{Hom}(U,\,V)$
- $\mathrm{rang}\,A= \mathrm{rang}\,B\quad\Leftrightarrow$
  $\Leftrightarrow\quad\exists S\in \mathrm{Hom}\,V,\ T\in \mathrm{Hom}\,U\text{ — regularni}\ \ :\ \ A=S\circ B\circ T$
- $\mathrm{rang}\,A= \mathrm{rang}\,B$ je relacija ekvivalencije na $\mathrm{Hom}(U,\,V)$