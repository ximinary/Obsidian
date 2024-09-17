#fax #math #laag [deo poglavlja [[Linearni operator|"linearni operator"]]]
$\:$

Napomena: [[Koordinatizacija. Zavisnost koordinata vektora o bazi#^0319ea|koordinatizacija]]
$\:$

Veza između $\mathrm{Hom}(U,\,V)$ $\ \ \Big(e = (e_{1},\,e_{2},\,\dots,\,e_{n})$  je baza $U$ i $f= (f_{1},\,f_{2},\,\dots,\,f_{m})$  je baza $V\ \Big)$ i $\mathbb{M}_{mn}(\mathbb{F})$.

$\varphi_{e,\,f}:\ \mathrm{Hom}(U,\,V)\to\mathbb{M}_{mn}(\mathbb{F})$, def. sa:
$\varphi_{e,\,f}(A)=\mathcal{A}$, tako da $\forall u\in U\quad \mathcal{A}\cdot\kappa_{e}(u)=\kappa_{f}\big(A(u)\big)$

$g_{k}:=A(e_{k}),\ \ \forall k =\overline{1,n}\ \ \:$ — slike baznih vektora,
tada $\ \mathcal{A}\cdot\kappa_{e}(e_{k})=\kappa_{f}(g_{k})$, tj. kolone matrice $\mathcal{A}$ su redom $\kappa_{f}(g_{k}),\ \ k=\overline{1,n}$
Dakle, ako $\mathcal{A}=(\alpha_{ij})$, onda $A(e_{k})=g_{k}=\sum\limits_{i=1}^{m}\alpha_{ik}\,f_{i},\ \  k=\overline{1,n}$

Teorema. $\varphi_{e,\,f}\in\mathrm{Hom}\Big(\mathrm{Hom}(U,\,V),\ \mathbb{M}_{mn}(\mathbb{F})\Big)$ i jeste izomorfizam.
___
Teorema. $\mathrm{Hom}\,V$ $(\dim V=n)$ i $\mathbb{M}_{n}(\mathbb{F})$ su izomorfni algebre sa jedinicom.
$\varphi_{e}$ slika regularni LO u invertibilne matrice.

### Kompozicija LO i množenje matrica:

$A=\mathrm{Hom}(V,\,W),\ \ B=\mathrm{Hom}(U,\,V)$,
$C=B\circ A$.

$e$ je baza $U$, $f$ je baza $V$, $g$ je baza $W$,
$\dim U=n$, $\dim V=m$, $\dim W=k$.

$\begin{array}{l l} \varphi_{f,\,g}(A)=\mathcal{A}=(\alpha_{ij})&\varphi_{e,\,f}(B)=\mathcal{B}=(\beta_{ij})\\A(e_{p})=\sum\limits_{i=1}^{m}\alpha_{ip}\,f_{i}&B(f_{q})=\sum\limits_{j=1}^{k}\beta_{jq}\,g_{j}\end{array}$

$C(e_{p})=B\big(A(e_{p})\big)=B\left( \sum\limits_{i=1}^{m}\alpha_{ip}\,f_{i} \right)=$
$=\sum\limits_{i=1}^{m}\alpha_{ip}\,B(f_{i})=\sum\limits_{i=1}^{m}\left(\alpha_{ip}\,\sum\limits_{j=1}^{k}\beta_{ji}\,g_{j}\right)=$
$=\sum\limits_{j=1}^{k}\underbrace{\left(\sum\limits_{i=1}^{m}\alpha_{ip}\,\beta_{ji}\right)}_{\gamma_{jp}}\,g_{j}=\sum\limits_{j=1}^{k}\gamma_{jp}\,g_{j}$

Odakle: $\varphi_{e,\,g}(C)=\mathcal{C}=(\gamma_{ip})$

$\gamma_{ip}=\sum\limits_{i=1}^{m}\beta_{ji}\,\alpha_{ip}=(\mathcal{B}\cdot\mathcal{A})_{ip}$

Konačno,  $\varphi_{e,\,g}(B\circ A)=\varphi_{e,\,f}(B)\cdot\varphi_{f,\,g}(A)$

### Zavisnost matrice LO o bazi
Napomena: [[Koordinatizacija. Zavisnost koordinata vektora o bazi#Prelazak sa jedne baze na drugu|Zavisnost koordinata vektora o bazi]]
$\:$

Teorema. Neka su
$e= \{e_{1},\,e_{2},\,\dots,\,e_{n}\}$ i $e'= \{e'_{1},\,e'_{2},\,\dots,\,e'_{n}\}$ baze VP-a $U$,
$f= \{f{1},\,f_{2},\,\dots,\,f_{n}\}$ i $f'= \{f'_{1},\,f'_{2},\,\dots,\,f'_{n}\}$ baze VP-a $V$,
$A\in \mathrm{Hom}(U,\,V)$

Tada: $\boxed{\varphi_{e',\,f'}(A)=[T_{ff'}]^{-1}\cdot\varphi_{e,\,f}(A)\cdot T_{ee'}}$

> Dokaz:
> $\forall x\in U\quad$ posmatrajmo $y=A(x)$
> u bazama $e$ i $f$: $\ \quad$ $\kappa_{f}(y)=\varphi_{e,\,f}(A)\cdot \kappa_{e}(x)$ $\ \quad$ (1)
> u bazama $e'$ i $f'$: $\ \,\:$ $\kappa_{f'}(y)=\varphi_{e',\,f'}(A)\cdot \kappa_{e'}(x)$ $\ \:$ (2)
> 
> Iz [[Koordinatizacija. Zavisnost koordinata vektora o bazi#^da8114|teoreme]]:
> $\kappa_{e}(x)=T_{ee'}\cdot\kappa_{e'}(x)$ $\ \ \quad$ (3)
> $\kappa_{f}(y)=T_{ff'}\cdot\kappa_{f'}(y)$ $\,\ \quad$ (4)
>
>$\boxed{\varphi_{e,\,f}(A)\cdot T_{ee'}}\cdot\kappa_{e'}(x)\overset{(3)}{=}\varphi_{e,\,f}(A)\cdot\kappa_{e}(x)\overset{(1)}{=}\kappa_{f}(y)\overset{(4)}{=}T_{ff'}\cdot\kappa_{f'}(y)\overset{(2)}{=}\boxed{T_{ff'}\cdot\varphi_{e',\,f'}(A)}\cdot\kappa_{e'}(x)$
>
>Odakle, jer je $T_{ff'}$ regularna, imamo:
>$\varphi_{e',\,f'}(A)=[T_{ff'}]^{-1}\cdot\varphi_{e,\,f}(A)\cdot T_{ee'}$

$\:$

Specijalno za $A\in\mathrm{Hom}\, V$ i
$e= \{e_{1},\,e_{2},\,\dots,\,e_{n}\}$, $e'= \{e'_{1},\,e'_{2},\,\dots,\,e'_{n}\}$ baze VP-a $V$:

$\varphi_{e',\,e'}(A)=[T_{ee'}]^{-1}\cdot\varphi_{e,\,e}(A)\cdot T_{ee'}$ ^4e5174
___
Operatori $id_{V}$ i $\mathbb{O}$ imaju istu matricu u svim bazama: $\mathbb{I}_{n}$ i $\mathcal{O}_{n\times n}$
___
[[Kvadratna matrica#Sličnost matrica|Sličnost matrica]]