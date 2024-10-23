#fax #math #laag [deo poglavlja [[Vektorski prostor|"vektorski prostor"]]]
$\:$

**Def**. $V$ je VP dimenzije $n$ nad poljem $\mathbb{F}$, $\:$ $e=\{ e_{1},\,e_{2},\,\dots,\,e_{n} \}$ je neka baza VP-a $V$. Tada za bazu $e$, **koordinatizacija** je preslikavanje $\kappa_{e}:\ V\to \mathbb{F}^{n}$, koje je definisano formulom $\kappa_{e}(x)=\kappa_{e}\left( \sum\limits_{i=1}^{n}x_{i}\,e_{i} \right)=(x_{1},\,x_{2},\,\dots,\,x_{n})=\left(\begin{array}{}x_{1}\\x_{2}\\\dots\\x_{n}\end{array}\right)=[x]_{e}$. ^0319ea

$\kappa_{e}$ je [[Linearni operator#^86cf6f|izomorfizam]] VP-a $V$ i $\mathbb{F}^{n}$ jer važe:
- $\forall x,\,y\in V\quad \kappa_{e}(x+y)=\kappa_{e}(x)+\kappa_{e}(y)$
- $\forall x\in V,\ \forall \lambda\in \mathbb{F}\quad \kappa_{e}(\lambda\,x)=\lambda\,\kappa_{e}(x)$
- $\kappa_{e}$ je bijekcija

### Prelazak sa jedne baze na drugu
Neka su $e= \{e_{1},\,e_{2},\,\dots,\,e_{n}\}$ i $e'= \{e'_{1},\,e'_{2},\,\dots,\,e'_{n}\}$ baze VP-a $V$.

$e'_{k}=\sum\limits_{i=1}^{n}\alpha_{ik}\,e_{i}\quad\forall k=\overline{1,n}$
Matrično:
$\left(\begin{array}{c}e'_{1}&e'_{2}&\dots&e'_{n}  \end{array}\right)=\left(\begin{array}{c}e_{1}&e_{2}&\dots&e_{n}  \end{array}\right)\left(\begin{array}{c}\alpha_{11}&\alpha_{12}&\dots&\alpha_{1n}\\ \alpha_{21}&\alpha_{22}&\dots&\alpha_{2n}\\ \dots&\dots&\dots&\dots\\\alpha_{n1}&\alpha_{n2}&\dots&\alpha_{nn}\end{array}\right)$

$T_{ee'}:=(\alpha_{ij})$ — matrica prelaska sa $e$ u $e'$

tj. $T_{ee'}=[\underbrace{\kappa_{e}(e'_{1}),\ \kappa_{e}(e'_{2}),\ \dots,\ \kappa_{e}(e'_{n})}_{\text{kolone}}]$
$\:$
___
$\begin{align}x=\sum\limits_{i=1}^{n}\boxed{x_{i}}\,e_{i}&=\sum\limits_{j=1}^{n}x'_{j}\,e'_{j}=\sum\limits_{j=1}^{n}x'_{j}\bigg(\sum\limits_{i=1}^{n}\alpha_{ij}\,e_{i}\bigg)=\\&=\sum\limits_{i=1}^{n}\boxed{\bigg(\sum\limits_{j=1}^{n}\alpha_{ij}\,x'_{j}\bigg)}\,e_{i},\quad \forall x\in V\end{align}$

Odakle: $x_{k}=\sum\limits_{j=1}^{n}\alpha_{kj}\,x'_{j},\quad \forall k=\overline{1,n}$
Matrično:
$\left(\begin{array}{c}x_{1}\\x_{2}\\\dots\\x_{n}\end{array}\right)=\left(\begin{array}{c}\alpha_{11}&\alpha_{12}&\dots&\alpha_{1n}\\ \alpha_{21}&\alpha_{22}&\dots&\alpha_{2n}\\ \dots&\dots&\dots&\dots\\\alpha_{n1}&\alpha_{n2}&\dots&\alpha_{nn}\end{array}\right)\left(\begin{array}{c}x'_{1}\\x'_{2}\\\dots\\x'_{n}\end{array}\right)$
$\:$

**Teorema**. $e,\,e',\,e''$ su baze VP-a $V$. Tada:
1. $\kappa_{e}(x)=T_{ee'}\cdot\kappa_{e'}(x)\ \:$ — $\ \:$skraćeni matrični zapis ^da8114
2. $T_{ee} = E\ \:$ — $\ \:$jedinična matrica
3. $T_{ee''}=T_{ee'}\cdot T_{e'e''}$
4. $[T_{ee'}]^{-1}=T_{e'e}$

> Dokaz:
> 3\. $\begin{align}&\kappa_{e}(x)\overset{_{1)}}{=}T_{ee'}\cdot\kappa_{e'}(x)\overset{_{1)}}{=}T_{ee'}\,\big(T_{e'e''}\cdot\kappa_{e''}(x)\big)=(T_{ee'}\cdot T_{e'e''})\cdot\kappa_{e''}(x)\\&\kappa_{e}(x)\overset{_{1)}}{=}T_{ee''}\cdot\kappa_{e''}(x)\end{align}\Bigg|\ \ \Rightarrow$
>    
>    $\quad\Rightarrow\ \ T_{ee''}=T_{ee'}\cdot T_{e'e''}$
>    
>    4\. $\begin{align}&E\overset{_{2)}}{=}T_{ee}\overset{_{3)}}{=}T_{ee'}\cdot T_{e'e}\\&E\overset{_{2)}}{=}T_{e'e'}\overset{_{3)}}{=}T_{e'e}\cdot T_{ee'}\end{align}\Bigg|\ \ \Rightarrow\ \ [T_{ee'}]^{-1}=T_{e'e}$
