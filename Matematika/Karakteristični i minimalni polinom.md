#fax #math #laag [deo [[Linearna algebra|linearne algebre]]]

### Karakteristični polinom
**Def**. $\mathcal{A}\in\mathbb{M}_{m}(\mathbb{F})$ — proizvoljna [[Matrica|matrica]], tada matrica $\Big(\lambda\,\mathbb{I}_{m}-\mathcal{A}\Big)$ , gde je $\lambda\in\mathbb{F}$ promenljiva, zove se **karakteristična matrica** matrice $\mathcal{A}$.

$p_{\mathcal{A}}(\lambda)=\det\Big(\lambda\,\mathbb{I}_{m}-\mathcal{A}\Big)\in\mathbb{F}[\lambda]$ je **karakteristični polinom** matrice $A$. 
Oblika je $p_{\mathcal{A}}(\lambda)=\lambda^{m}-\mathrm{Tr}\,\mathcal{A}\cdot\lambda^{m-1}+\dots$

$p_{\mathcal{A}}(\lambda)=0$ — **karakteristična jednačina** matrice $A$.

**Teorema**. Karakteristični polinom je [[Kvadratna matrica#Sličnost matrica|invarijanta sličnosti]].
> Dokaz: $\mathcal{A}\sim\mathcal{B}$
> Tada $\exists\mathcal{T}\ \ :\ \ \mathcal{B}=\mathcal{T}^{-1}\mathcal{A}\,\mathcal{T}$
> $\begin{align}p_{\mathcal{B}}(\lambda)&=\det\Big(\lambda\,\mathbb{I}_{n}-\mathcal{B}\Big)=\det\Big(\mathcal{T}^{-1}\big(\lambda\,\mathbb{I}_{n}\big)\,\mathcal{T}-\mathcal{T}^{-1}\mathcal{A}\,\mathcal{T}\Big)=\\&=\det\Big(\mathcal{T}^{-1}\big(\lambda\,\mathbb{I}_{n}-\mathcal{A}\big)\,\mathcal{T}\Big)=\det\mathcal{T}^{-1}\det\Big(\lambda\,\mathbb{I}_{n}-\mathcal{A}\Big)\det\mathcal{T}=\\&=\det\Big(\lambda\,\mathbb{I}_{n}-\mathcal{A}\Big)=p_{\mathcal{A}}(\lambda)\end{align}$

Def. **Karakteristični polinom [[Linearni operator|LO]]** $A\in\mathrm{Hom}\, V$ je $p_{A}(\lambda):=p_{\varphi_{e,\,e}(A)}(\lambda)$ za proizvoljnu bazu $e$ VP-a $V$.
$\:$
___
> $q(\lambda)=\alpha_{n}\,\lambda^{n}+\alpha_{n-1}\,\lambda^{n-1}+\dots+\alpha_{2}\,\lambda^{2}+\alpha_{1}\,\lambda+\alpha_{0}$
> 
> $\mathcal{A}\in\mathbb{M}_{m}(\mathbb{F})$
> $q(\mathcal{A})=\alpha_{n}\,\mathcal{A}^{n}+\alpha_{n-1}\,\mathcal{A}^{n-1}+\dots+\alpha_{2}\,\mathcal{A}^{2}+\alpha_{1}\,\mathcal{A}+\alpha_{0}\,\mathbb{I}_{m}$

Stav. $\forall\mathcal{A}\in\mathbb{M}_{m}(\mathbb{F})\quad\exists q\in\mathbb{F}[\lambda]\ \ :\ \ q(\mathcal{A})=\mathcal{O}$

Lema (Bezuova). $q(\lambda)=\alpha_{n}\,\lambda^{n}+\alpha_{n-1}\,\lambda^{n-1}+\dots+\alpha_{2}\,\lambda^{2}+\alpha_{1}\,\lambda+\alpha_{0}\in\mathbb{F}[\lambda]$, za $\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})$ važi $q(\lambda)\,\mathbb{I}_{n}=\big(\lambda\,\mathbb{I}_{n}-\mathcal{A}\big)\,r(\lambda)$, $\ \:$  gde $r(\lambda)=\mathcal{C}_{n-1}\,\lambda^{n-1}+\mathcal{C}_{n-2}\,\lambda^{n-2}+\dots+\mathcal{C}_{1}\,\lambda+\mathcal{C}_{0}, \quad \mathcal{C}_{i}\in\mathbb{M}_{n}(\mathbb{F})$
Tada $q(\mathcal{A})=\mathcal{O}$

Teorema (Hamilton-Kejlijeva). $\forall\mathcal{A}\in\mathbb{M}_{m}(\mathbb{F})\quad p_{\mathcal{A}}(\mathcal{A})=\mathcal{O}$

### Minimalni polinom 

**Def**. **Minimalni polinom** [[Matrica|matrice]] $\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})$ je $\mu_{\mathcal{A}}(\lambda)\in\mathbb{F[\lambda]}$ — moničan (viši koef. je jednak $1$) polinom najmanjeg stepena za koji važi $\mu_{\mathcal{A}}(\mathcal{A})=0$.

Teorema. $\mathcal{A}\in \mathbb{M}_{m}(\mathbb{F})$.
1. $q\in\mathbb{F}[\lambda]\ \ :\ \ q(\mathcal{A})\quad \Rightarrow\quad \mu_{\mathcal{A}}(\lambda)\ \Big|\ q(\lambda)$
2. $\mu_{\mathcal{A}}$ je jedinstven 
3. $\mu_{\mathcal{A}}$ je invarijanta sličnosti
> Dokaz:
> 1. pps $\mu_{\mathcal{A}}(\lambda)\not\Big|\ \ q(\lambda)$
>    Tada $q(\lambda)=\mu_{\mathcal{A}}(\lambda)\,s(\lambda)+r(\lambda),\ \ r\not\equiv0$, stepen $r$ je manji od stepena $\mu_{\mathcal{A}}$
>    $\underbrace{q(\mathcal{A})}_{=\,\mathcal{O}}=\underbrace{\mu_{\mathcal{A}}(\mathcal{A})}_{=\,\mathcal{O}}\,s(\mathcal{A})+r(\mathcal{A})\quad\Rightarrow\quad r(\mathcal{A})=\mathcal{O}$
>    kontradikcija, jer stepen $r$ je manji od stepena minimalnog polinoma
>    $\:$
>   1. pps $\exists \mu_{\mathcal{A}}\not\equiv\mu'_{\mathcal{A}}$ dva minimalnih polinoma stepena $n$. Tada
>    $\mu_{\mathcal{A}}(\mathcal{A})=\mathcal{A}^{n}+\alpha_{n-1}\,\mathcal{A}^{n-1}+\dots+\alpha_{2}\,\mathcal{A}^{2}+\alpha_{1}\,\mathcal{A}+\alpha_{0}=\mathcal{O}$
>    $\mu'_{\mathcal{A}}(\mathcal{A})=\mathcal{A}^{n}+\alpha'_{n-1}\,\mathcal{A}^{n-1}+\dots+\alpha'_{2}\,\mathcal{A}^{2}+\alpha'_{1}\,\mathcal{A}+\alpha'_{0}=\mathcal{O}$
>    Oduzmemo jednu jednačinu od druge:
>    $(\alpha'_{n-1}-\alpha_{n-1})\,\mathcal{A}^{n-1}+\dots+(\alpha'_{2}-\alpha_{2})\,\mathcal{A}^{2}+(\alpha'_{1}-\alpha_{1})\,\mathcal{A}+(\alpha'_{0}-\alpha_{0})=\mathcal{O}$
>    dobili smo polinom $r$ stepena manjeg od minimalnog, za koji važi $r(\mathcal{A})=\mathcal{O}$. Kontradikcija.
>      $\:$
>   3. $\mathcal{A}\sim\mathcal{B}$
> Tada $\exists\mathcal{T}\ \ :\ \ \mathcal{B}=\mathcal{T}^{-1}\mathcal{A}\,\mathcal{T}$
> $\mathcal{B}^{k}=(\mathcal{T}^{-1}\mathcal{A}\,\mathcal{T})^{k}=\mathcal{T}^{-1}\mathcal{A}^{k}\,\mathcal{T}$
> Neka je $\mu_{\mathcal{A}}(\lambda)=\lambda^{n}+\alpha_{n-1}\,\lambda^{n-1}+\dots+\alpha_{1}\,\lambda+\alpha_{0}$
> $\:$
> $\begin{align}\mu_{\mathcal{A}}(\mathcal{B})&=\mathcal{B}^{n}+\alpha_{n-1}\,\mathcal{B}^{n-1}+\dots+\alpha_{1}\,\mathcal{B}+\alpha_{0}=\\&=\mathcal{T}^{-1}\mathcal{A}^{n}\,\mathcal{T}+\alpha_{n-1}\,\mathcal{T}^{-1}\mathcal{A}^{n-1}\,\mathcal{T}+\dots+\alpha_{1}\,\mathcal{T}^{-1}\mathcal{A}\,\mathcal{T}+\alpha_{0}\mathcal{T}^{-1}\mathbb{I}_{m}\,\mathcal{T}=\\&=\mathcal{T}^{-1}\Big(\mathcal{A}^{n}+\alpha_{n-1}\,\mathcal{A}^{n-1}+\dots+\alpha_{1}\,\mathcal{A}+\alpha_{0}\Big)\mathcal{T}\\&=\mathcal{T}^{-1}\mu_{\mathcal{A}}(\mathcal{A})\,\mathcal{T}=\mathcal{T}^{-1}\mathcal{O}\,\mathcal{T}=\mathcal{O}\end{align}$
> Slično: $\mu_{\mathcal{B}}(\mathcal{A})=0$
> $\:$
> Odakle:
> $\begin{align}\mu_{\mathcal{A}}(\mathcal{B})=\mathcal{O}\ \ \overset{1.}{\Rightarrow}\ \ \mu_{\mathcal{B}}\ \Big|\ \mu_{\mathcal{A}}\\\mu_{\mathcal{B}}(\mathcal{A})=\mathcal{O}\ \ \overset{1.}{\Rightarrow}\ \ \mu_{\mathcal{A}}\ \Big|\ \mu_{\mathcal{B}}\end{align}\quad\Rightarrow\quad\mu_{\mathcal{A}}=\mu_{\mathcal{B}}$ $\ \:$ (jer su monične)


Def. **Minimalni polinom [[Linearni operator|LO]]** $A\in\mathrm{Hom}\, V$ je $\mu_{A}(\lambda):=\mu_{\varphi_{e,\,e}(A)}(\lambda)$ za proizvoljnu bazu $e$ VP-a $V$.

Stav. Minimalni polinom matrice $\mathcal{A}=\left(\begin{array}{}0&0&\dots&0&-\alpha_{0}\\1&0&\dots&0&-\alpha_{1}\\0&1&\dots&0&-\alpha_{2}\\\dots&\dots&\dots&\dots&\dots\\0&0&\dots&1&-\alpha_{n-1}\end{array}\right)$ je $\mu_{\mathcal{A}}(\lambda)=\lambda^{n}+\alpha_{n-1}\,\lambda^{n-1}+\dots+\alpha_{2}\,\lambda^{2}+\alpha_{1}\,\lambda+\alpha_{0}$

Stav. $\mathcal{A}\in\mathbb{M}_{m}(\mathbb{F})$
1. $\exists q\in\mathbb{F}[\lambda]\ \ :\ \ q(\mathcal{A})=\mathcal{O}\ \ \mathrm{i}\ \ q(0)\ne0\quad\Rightarrow\quad\mathcal{A}$ je invertibilna
2. $\mu_{\mathcal{A}}(0)\ne0\quad\Leftrightarrow\quad\mathcal{A}$ je invertibilna

> Dokaz.
> 1. Neka $q(\lambda)=\alpha_{n}\,\lambda^{n}+\alpha_{n-1}\,\lambda^{n-1}+\dots+\alpha_{2}\,\lambda^{2}+\alpha_{1}\,\lambda+\alpha_{0}$
>    $\alpha_{0}=q(0)\ne0$
>    $\begin{align}\mathcal{O}=q(\mathcal{A})&=\alpha_{n}\,\mathcal{A}^{n}+\alpha_{n-1}\,\mathcal{A}^{n-1}+\dots+\alpha_{2}\,\mathcal{A}^{2}+\alpha_{1}\,\mathcal{A}+\alpha_{0}\,\mathbb{I}_{m}\\-\alpha_{0}\,\mathbb{I}_{m}&=\Big(\alpha_{n}\,\mathcal{A}^{n-1}+\alpha_{n-1}\,\mathcal{A}^{n-2}+\dots+\alpha_{2}\,\mathcal{A}+\alpha_{1}\Big)\,\mathcal{A}\\\mathbb{I}_{m}&=\underbrace{\bigg(-\frac{1}{\alpha_{0}}\Big(\alpha_{n}\,\mathcal{A}^{n-1}+\alpha_{n-1}\,\mathcal{A}^{n-2}+\dots+\alpha_{2}\,\mathcal{A}+\alpha_{1}\Big)\bigg)}_{\mathcal{A}^{-1}}\mathcal{A}\end{align}$
> $\:$
> 2. $\boxed{\Rightarrow}$ Dokazano u 1.
>    $\boxed{\Leftarrow}$ pps $\mu_{\mathcal{A}}=0$,
>    tada $\mu_{\mathcal{A}}(\mathcal{A})=\mathcal{A}^{n}+\alpha_{n-1}\,\mathcal{A}^{n-1}+\dots+\alpha_{2}\,\mathcal{A}^{2}+\alpha_{1}\,\mathcal{A}=\mathcal{O}$
>    pomnožimo sa $\mathcal{A}^{-1}$:
>    $\mathcal{A}^{n-1}+\alpha_{n-1}\,\mathcal{A}^{n-2}+\dots+\alpha_{2}\,\mathcal{A}+\alpha_{1}=\mathcal{O}$,
>    dobili smo polinom $r$ stepena manjeg od minimalnog, za koji važi $r(\mathcal{A})=\mathcal{O}$. Kontradikcija.
^251032

$\:$

### Sopstvene vrednosti
**Def**. $\lambda\in\mathbb{F}$ je **sopstvena vrednost** LO $A\in\mathrm{Hom}\,V$, ako $\exists \underset{\ne\,0}{x\in} V \ \ :\ \ A(x)=\lambda\,x$.
Tada $x$ se zove **sopstveni vektor**.

$\mathrm{Sp}\,A$ — **spektar** $A$ — skup svih sopstvenih vrednosti.

$V\big._{\lambda}^{A}=\{ x\in V \ \big|\ A(x)=\lambda\,x\}$ — **sopstveni potprostor** sopstvene vrednosti $\lambda$ operatora $A$ — skup sopstvenih vrednosti $A$, koji odgovaraju sopstvenoj vrednosti $\lambda$, i nula vektora.

Stav. $V\big._{\lambda}^{A}\leqslant V$

Teorema. $A\in \mathrm{Hom}\,V$
$\lambda_{0}\in\mathbb{F}$ je sopstvena vrednost $A$ $\quad\Leftrightarrow\quad$ $p_{A}(\lambda_{0})=0$

> Napomene:
> - Sopstvene vrednosti su [[Kvadratna matrica#Sličnost matrica|invarijante sličnosti]].
> - Definicija sopstvene vrednosti bitno zavisi o polju:
> $p_{A}(\lambda)=\lambda^{2}+1$
> ako $\mathbb{F}=\mathbb{R}$: $A$ nema sopstvenih vrednosti
> ako $\mathbb{F}=\mathbb{C}$: $A$ ima sopstvene vrednosti $\lambda_{1}=i,\ \lambda_{2}=-i$

$\:$
Teorema. $A\in\mathrm{Hom}_{\mathbb{C}}\,V$, $V$ je VP nad poljem $\mathbb{C}$, $\dim V=n.$
Tada $A$ ima tačno $n$ sopstvenih vrednosti (među kojima može biti istih). 
(Jer u $\mathbb{C}$ samo linearni (faktori) polinomi nisu reducibilni)

Posledica. $A\in\mathrm{Hom}\,V$, $\dim V=n.$ Tada $A$ ima najviše $n$ sopstvenih vrednosti.
___
**Teorema**. $\mathcal{A}\in\mathbb{M}_{m}(\mathbb{F})$
Ako $\boxed{p_{\mathcal{A}}(\lambda)=q_{1}(\lambda)^{r_{1}}\cdot q_{2}(\lambda)^{r_{2}}\cdot\!\cdot\!\cdot q_{k}(\lambda)^{r_{k}}}$, gde
$k\in\mathbb{N}, \quad \forall i =\overline{1,k}\quad r_{i}\in\mathbb{N}\ \ \mathrm{i}\ \ p_{i}(\lambda)$ je ireducibilan moničan polinom nad $\mathbb{F}$, tada je
$\boxed{\mu_{\mathcal{A}}(\lambda)=q_{1}(\lambda)^{s_{1}}\cdot q_{2}(\lambda)^{s_{2}}\cdot\!\cdot\!\cdot q_{k}(\lambda)^{s_{k}}}$, gde
$\forall i=\overline{1,k}\quad s_{i}\in\mathbb{N}, \ \ s_{i}\leqslant r_{i}$

> Minimalni polinom tražimo tako što smanjujemo stepen ireducibilnih faktora karakterističnog polinoma, dok polinom od polazne matrice jednak $\mathcal{O}$.
___

Def. $A\in\mathrm{Hom}\,V$.
**Algebarska višestrukost** $\lambda_{0}$ — višestrukost $\lambda_{0}$ kao nule $p_{A}(\lambda)$.
**Geometrijska višestrukost** $\lambda_{0}$ — dimenzija $V\big._{\lambda_{0}}^{A}$.

Stav. Algebarska višestrukost $\geqslant$ geometrijska višestrukost.

### Dijagonalizacija
Stav. $A\in\mathrm{Hom}\,V$. Tada je $\mathrm{Sp}\,A$ je linearno nezavisan.

**Def**. **Dijagonalizacija** je nalaženje baze $V$ u kojoj matrica operatora $A\in\mathrm{Hom}\,V$ je dijagonalna.
$A$ je **dijagonalizabilan** ako takva baza postoji.


Teorema (O dijagonalizabilnosti).
$A\in\mathrm{Hom}\,V$,$\:$ $\dim V=n.$ Tada su ekvivalentni:
- $A$ je dijagonalizabilan
- $\exists e$ — baza od $V$ koja sastoji od sopstvenih vektora $A$.
- $A$ ima $n$ sopstvenih vektora.
- $\mu_{\mathcal{A}}(\lambda)$ je proizvod <u>različitih</u> linearnih faktora.

Matrica $A$ u bazi $e=(e_{1},\,e_{2},\,\dots,\,e_{n})$:
$\varphi_{e,\,e}(A)=\left(\begin{array}{}\lambda_{1}&0&\dots&0\\0&\lambda_{2}&\dots&0\\\dots&\dots&\dots&\dots\\0&0&\dots&\lambda_{n}\end{array}\right)$,
gde je $\lambda_{i}$ odgovarajuća sopstvenom vektoru $e_{i}$ sopstvena vrednost.
___

$\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})$ je **dijagonalizabilna** ako $\exists \mathcal{D}=\mathrm{diag}[\lambda_{1},\,\lambda_{2},\,\dots,\,\lambda_{n}]$, takva da $\mathcal{A}\sim\mathcal{D}$, tj. $\exists\mathcal{P}\ \ : \ \ \mathcal{D}=\mathcal{P}^{-1}\mathcal{A}\,\mathcal{P}$

$\lambda_{1},\,\lambda_{2},\,\dots,\,\lambda_{n}$ su rešenja $p_{\mathcal{A}}(\lambda)=0$

$\mathcal{P}=\underbrace{\big[v_{1},\ v_{2},\ \dots,\ v_{n}\big]}_{\text{kolone}}$, gde je $v_{i}\ne \mathbf{0}$ sopstveni vektor, 

tj. $\Big(\lambda_{i}\,\mathbb{I}_{n}-\mathcal{A}\Big)v_{i}=\mathbf{0},\quad \forall i=\overline{1,n}$

**!** Sopstvenom vektoru $v_{i}$ odgovara sopstvena vrednost $\lambda_{i}$

>Korišćenje:
> nalaženje $\mathcal{A}^{k}$:
> $\mathcal{A} = \mathcal{P}\,\mathcal{D}\,\mathcal{P}^{-1}$
> 
> $\mathcal{A}^{k} = \mathcal{P}\,\mathcal{D}^{k}\,\mathcal{P}^{-1}=\mathcal{P}\cdot\mathrm{diag}[\lambda_{1}^{k},\,\lambda_{2}^{k},\,\dots,\,\lambda_{n}^{k}]\cdot\mathcal{P}^{-1}$
