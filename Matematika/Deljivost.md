#fax #math #ds1 [deo poglavlja [[Prirodni brojevi|"prirodni brojevi"]] i [[Celi brojevi|"celi brojevi"]]]
$\:$

### Deljivost u $\mathbb{N}$
**Def**. $a,\, b\in \mathbb{N}$
$a\,|\,b\:$ ($a$ deli $b$) ako $\exists c \in \mathbb{N}\ \ : \ \ b = a\cdot c$

[[deljivost stav.png|Stav]]. U skupu $\mathbb{N}\setminus\{ 0 \}$ relacija deljivosti je [[Relacija poretka|relacija nestrogog parcijalnog poretka]].

[[deljivost osobine.png|Osobine]]: $\: \forall a,\,b,\,c \in \mathbb{N}$
1. $a\,|\,0\:$
2. $a\,|\,b\ \ \mathrm{i}\ \ a\,|\, c\ \ \ \Rightarrow \ \ \ a\,|\, (b+c)$
3. $a\,|\,b\ \ \mathrm{ili}\ \ a\,|\, c\ \ \ \Rightarrow \ \ \ a\,|\, (b\cdot c)$
4. $a\,|\,b\ \ \ \Rightarrow \ \ \ a\,|\, b^{n},\ \:$ za $\ \forall n\in \mathbb{N}\setminus\{ 0 \}$ 

### Deljivost u $\mathbb{Z}$
**Def**. $a,\, b\in \mathbb{Z}$
$a\,|\,b\:$ ($a$ deli $b$) ako $\exists c \in \mathbb{Z}\ \ : \ \ b = a\cdot c$

Deljivost nije [[Relacija poretka|relacija poretka]] u skupu $\mathbb{Z}\setminus\{ 0 \}$, jer ne važi (AS).

### Zajednički delilac i zajednički sadržalac
**Def**. Neka su $a,\,b \in \mathbb{N}\, (\mathbb{Z})$. $d\in \mathbb{N}$ je **zajednički delilac** $a$  i $b$ ako $d\,|\,a$ i $d\,|\,b$.
$d$ je najveći zajednički delilac (**NZD**) ako za svako $d'\in \mathbb{N}$ takvo da $d'\,|\,a$ i $d'\,|\,b$ važi $d'\,|\,d$.

**Def**. Neka su $a,\,b \in \mathbb{N}\, (\mathbb{Z})$. $s\in \mathbb{N}$ je **zajednički sadržalac** $a$  i $b$ ako $a\,|\,s$ i $b\,|\,s$.
$s$ je najmanji zajednički delilac (**NZS**) ako za svako $s'\in \mathbb{N}$ takvo da $a\,|\,s'$ i $b\,|\,s'$ važi $s\,|\,s'$.

### [[Euklidov algoritam]]
___
$\:$
Teorema. $a\,|\,b\, c\ \:$ i $\ \: \mathrm{NZD}(a,\, b)= 1$. $\:$ Tada $a\,|\,c$ ^015ce1
>Dokaz: Iz [[Euklidov algoritam#^e5f1a9|posledice Euklidovog algoritma]]:
>$\exists p,\,q\in \mathbb{Z}\ \ : \ \ a\,p + b\,q = 1$, pomnožimo jednačinu sa $c$: $\:$ $a\,c\,p + b\,c\,q = c$
>$\begin{aligned} a\,|\,a\,c\,p \\ a\,|\,b\,c \ \ \Rightarrow \ \ a\,|\, b\,c\,q\end{aligned} \ \ \Rightarrow \ \ a\,|\,(a\,c\,p + b\,c\,q) \ \ \Rightarrow \ \ a\,|\,c$

Posledica. $a\,|\,c\:$ i $\:b\,|\,c$; $\:\mathrm{NZD}(a,\,b) = 1$. $\:$ Tada $a\,b\,|\,c$  
> Dokaz: $c = b\,b_{1},\quad b_{1}\in \mathbb{Z}$
> $\begin{align}a\,|\,c\ \ \Rightarrow\ \ a\,|\,b\,b_{1}\\ \mathrm{NZD}(a,\,b) = 1\end{align}\ \  \stackrel{\mathrm{iz\ teoreme}}{\Longrightarrow} \ \ a\,|\,b_{1}\ \ \Rightarrow \ \ \exists t \in \mathbb{Z} \ :\ b_{1}=a\,t$
> $c = b\,b_{1}=a\,b\,t \ \ \Rightarrow\ \ a\,b\,|\,c$