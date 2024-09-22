#fax #math #laag [deo poglavlja [[Linearni operator|"linearni operator"]]]
$\:$

**Def**. $A\in\mathrm{Hom}\,V$, $L\leqslant V$.
$L$ je invarijantan potprostor operatora $A$ ako $A[L]\subseteq L$.
$\big(\forall x\in L\quad A(x)\in L\big)$

Restrikcija $A$ na $L$: $\quad$ $A_{L}:\ L\to L$ $\ \:$ def. sa $\ \:$ $A_{L}(x)=A(x)$

Trivijalni invarijantni prostori: $L=V$ i $L=\{0\}$

Stav. $A\in \mathrm{Hom}\,V$. Tada: $\mathrm{Im}\,A$ i $\mathrm{Ker}\,A$ su invarijantni prostori od $A$.

___
**Def**. $A\in\mathrm{Hom}\,V$ je
- **reducibilan**, ako ima netrivijalan invarijantni potprostor;
- **ireducibilan**, ako ima samo trivijalne inv. potprostore;
- **dekompozabilan**, ako ima netrivijalne inv. potprostore $L$ i $M$, takve da $V=L\oplus M$ 
- **potpuno reducibilan**, ako za svaki netrivijalan inv. potprostor $L$ postoji netrivijalan inv. potprostor $M$.

**Def**. Ako je $A$ dekompozabilan, onda $A$ je u potpunosti određen 
restrikcijama $A_{L}$ i $A_{M}$: 
$\forall x\in V\quad\exists!(l,\, m)\in L\times M\ \ :\ \ x=l+m$
Dakle, $A(x)=A(l)+A(m)=A_{L}(l)+A_{M}(m)$
Tada $A$ je direktna suma operatora $A_{L}$ i $A_{M}$.
Oznaka: $A=A_{L}\oplus A_{M}$

Teorema. $A\in\mathrm{Hom}\,V$
- $A$ je reducibilan, $L$ je invarijantan potprostor $\\ \ \Leftrightarrow$
$\Leftrightarrow\ \ \,$ $\exists e$ — baza od $V$ takva da matrica operatora $A$ u bazi $e$ je oblika $\left(\begin{array}{}\mathcal{A}_{11}&\mathcal{A}_{12}\\\mathcal{O}&\mathcal{A}_{22}\end{array}\right)$, gde je $\mathcal{A}_{11}$ matrica operatora $A_{L}$.
$\:$
- $A$ je dekompozabilan, $A=A_{L}\oplus A_{M}$ $\ \ \Leftrightarrow$
  $\Leftrightarrow\ \ \,$ $\exists e$ — baza od $V$ takva da matrica operatora $A$ u bazi $e$ je oblika $\left(\begin{array}{}\mathcal{A}_{1}&\mathcal{O}\\\mathcal{O}&\mathcal{A}_{2}\end{array}\right)$, gde su $\mathcal{A}_{1}$ i $\mathcal{A_{2}}$ matrice operatora $A_{L}$ i $A_{M}$.
  $\:$
- $A$ je potpuno reducibilan, $L_{1},\,L_{2},\,\dots,\,L_{m}$ su invarijantni potprostori $\big(A=A_{L_{1}}\oplus A_{L_{2}}\oplus\dots\oplus A_{L_{m}}\big)$ $\\ \ \Leftrightarrow$
  $\Leftrightarrow\ \ \,$ $\exists e$ — baza od $V$ takva da matrica operatora $A$ u bazi $e$ je oblika $\left(\begin{array}{}\mathcal{A}_{1}&\mathcal{O}&\dots&\mathcal{O}\\\mathcal{O}&\mathcal{A}_{2}&\dots&\mathcal{O}\\\dots&\dots&\dots&\dots\\\mathcal{O}&\mathcal{O}&\dots&\mathcal{A}_{m}\end{array}\right)$, gde je $\mathcal{A}_{i}$ matrica operatora $A_{L_{i}}$.