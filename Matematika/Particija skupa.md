#fax #math #ds2 [deo [[Kombinatorika|kombinatorike]]]
$\:$

Particija skupa $A$ ($|A|=n$) na $k$ podskupova je skup $\{ S_{1},\,S_{2},\,\dots,\,S_{k} \}$ pri čemu važe $S_{i}\subseteq A \quad\forall i=\overline{1,k}$ ; $\:$ $S_{i}\cap S_{j}=\varnothing\quad \forall i\ne j=\overline{1,k}$ $\:$ i $\:$ $A=S_{1}\cup S_{2} \cup\dots\cup S_{k}$

> Primer: $A=\mathbb{N}_{3}$
> $k=1\ \:$ — $\:\ \Big\{\{ 1,\,2,\,3 \}\Big\}$
> $k=2\ \:$ — $\:\ \Big\{\{ 1\},\,\{2,\,3 \}\Big\},\ \Big\{\{ 2\},\,\{1,\,3 \}\Big\},\ \Big\{\{ 3\},\,\{1,\,2 \}\Big\}$
> $k=3\ \:$ — $\:\ \Big\{\{1\},\,\{2\},\,\{3\}\Big\}$
> Ukupno: $\boxed{5}$

**Def**. **Stirlingov broj druge vrste** $S(n,\,k)$ je broj particija skupa od $n$ elemenata na $k$ podskupova.
**Def**. **Belov broj** $B(n)$ je broj particija skupa od $n$ elemenata. $\big(B(0):=1\big)$

Teorema.
$S(n+1,\,k)=S(n,\,k-1)+k\,S(n,\,k)$
>Dokaz:
> Particiju skupa $\mathbb{N}_{n+1}$ na $k$ podskupova možemo $\big[$ na jedinstven način dobiti od particije skupa $\mathbb{N}_{n}$ na $(k-1)$ podskupova dodavanjem skupa $\{ n+1 \}$ $\big]$ ili $\big[$ na $k$ načina od particije skupa $\mathbb{N}_{n}$ na $k$ podskupova dodavanjem elementa $(n+1)$ nekom od postojećih skupova $\big]$.


Teorema. Važi [[Rekurentna jednačina]]:
$\begin{cases}S(n+1,\,k)=S(n,\,k)+k\,S(n,\,k)\\S(n,\,1)=1,\quad S(n,\,n)=1\end{cases}$

Teorema. Važi [[Rekurentna jednačina]]:
$\begin{cases}\begin{align}B(n)=\sum\limits_{k=0}^{n-1}\binom{n}{k}B(k)\end{align}\\B(0)=1\end{cases}$