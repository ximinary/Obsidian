#fax #math #laag [deo [[Linearna algebra|linearne algebre]]]
$\:$

### Karakteristični polinom
**Def**. $\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})$ — proizvoljna [[Matrica|matrica]], tada matrica $\Big(\lambda\,\mathbb{I}_{n}-\mathcal{A}\Big)$ , gde je $\lambda\in\mathbb{F}$ promenljiva, zove se **karakteristična matrica** matrice $\mathcal{A}$.

$p_{\mathcal{A}}(\lambda)=\det\Big(\lambda\,\mathbb{I}_{n}-\mathcal{A}\Big)\in\mathbb{F}[\lambda]$ je **karakteristični polinom** matrice $A$. 
Oblika je $p_{\mathcal{A}}(\lambda)=\lambda^{n}+\mathrm{Tr}\,\mathcal{A}\cdot\lambda^{n-1}+\dots$

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

Stav. $\forall\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})\quad\exists q\in\mathbb{F}[\lambda]\ \ :\ \ q(\mathcal{A})=\mathcal{O}$

Lema (Bezuova). $q(\lambda)=\alpha_{n}\,\lambda^{n}+\alpha_{n-1}\,\lambda^{n-1}+\dots+\alpha_{2}\,\lambda^{2}+\alpha_{1}\,\lambda+\alpha_{0}\in\mathbb{F}[\lambda]$, za $\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})$ važi $q(\lambda)\,\mathbb{I}_{n}=\big(\lambda\,\mathbb{I}_{n}-\mathcal{A}\big)\,r(\lambda)$, $\ \:$  gde $r(\lambda)=\mathcal{C}_{n-1}\,\lambda^{n-1}+\mathcal{C}_{n-2}\,\lambda^{n-2}+\dots+\mathcal{C}_{1}\,\lambda+\mathcal{C}_{0}, \quad \mathcal{C}_{i}\in\mathbb{M}_{n}(\mathbb{F})$
Tada $q(\mathcal{A})=0$

Teorema (Hamilton-Kejlijeva). $\forall\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})\quad p_{\mathcal{A}}(\mathcal{A})=0$

### Minimalni polinom 

**Def**. **Minimalni polinom** [[Matrica|matrice]] $\mathcal{A}\in\mathbb{M}_{n}(\mathbb{F})$ je $\mu_{\mathcal{A}}(\lambda)\in\mathbb{F[\lambda]}$ — moničan (viši koef. je jednak $1$) polinom najmanjeg stepena za koji važi $\mu_{\mathcal{A}}(\mathcal{A})=0$.

Teorema. $\mathcal{A}\in \mathbb{M}_{n}(\mathbb{F})$.
- $q\in\mathbb{F}[\lambda]\ \ :\ \ q(\mathcal{A})\quad \Rightarrow\quad \mu_{\mathcal{A}}(\lambda)\ \Big|\ q(\lambda)$
- $\mu_{\mathcal{A}}$ je jedinstven 
- $\mu_{\mathcal{A}}$ je invarijanta sličnosti

Def. **Minimalni polinom [[Linearni operator|LO]]** $A\in\mathrm{Hom}\, V$ je $\mu_{A}(\lambda):=\mu_{\varphi_{e,\,e}(A)}(\lambda)$ za proizvoljnu bazu $e$ VP-a $V$.