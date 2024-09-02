#fax #math #ds2 [deo [[Kombinatorika|kombinatorike]]]
$\:$

**Def**. $n\in \mathbb{R},\ k\in \mathbb{N}$. Tada binomni koeficijent je:
$$
\binom{n}{k} = \frac{n\cdot(n-1)\dots(n-k+1)}{k!}
$$
Identiteti:
1. Uslov simetričnosti:
   $n,\,k\in\mathbb{N}_{0}\quad\begin{align}\binom{n}{k}=\binom{n}{n-k}\end{align}$
2. Negacija gornjeg indeksa:
   $n\in\mathbb{R},\,k\in\mathbb{N}_{0}\quad \begin{align}\binom{-n}{k}=(-1)^{k}\binom{n+k-1}{k}\end{align}$ ^37ae6b
3. Adiciona formula:
   $n\in\mathbb{R},\,k\in\mathbb{N}_{0}\quad \begin{align}\binom{n}{k-1}+\binom{n}{k}=\binom{n+1}{k}\end{align}$
4. Izvlačanje ispred zagrade:
   $n,\,k\in\mathbb{N}\quad\begin{align}\binom{n}{k}=\frac{n}{k}\binom{n-1}{k-1}=\frac{n}{n-k}\binom{n-1}{k}\end{align}$
5. Pojednostavljivanje proizvoda:
   $r,\,n,\,k\in\mathbb{N}_{0}\quad\begin{align}\binom{n}{r}\binom{r}{k}=\binom{n}{k}\binom{n-k}{r-k}\end{align}$
6. Sumacione formule:
   $r,\,n\in\mathbb{N}_{0}\quad\begin{align}\sum_{k=0}^{n}\binom{r+k}{k}=\binom{n+r+1}{n}\end{align}$
   $r,\,n\in\mathbb{N}_{0}\quad\begin{align}\sum_{k=0}^{n}\binom{k}{r}=\binom{n+1}{r+1}\end{align}$
7. Suma kvadrata:
   $n\in\mathbb{N}_{0}\quad\begin{align}\sum_{k=0}^{n}\binom{n}{k}^{2}=\binom{2n}{n}\end{align}$
8. Vandermodov identitet:
   $\begin{align}\sum_{k=0}^{r}\binom{r}{k}\binom{s}{n-k}=\binom{s+r}{n}\end{align}$
   $\begin{align}\sum_{k=0}^{r}\binom{r}{k}\binom{s}{n+k}=\binom{s+r}{n+r}\end{align}$