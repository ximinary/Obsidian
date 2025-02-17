#fax #math #a2 [deo [[Analiza|analize]]]
$\:$

**Def**. Neka je $(a_{n})$ [[Niz brojeva|niz realnih brojeva]]. Tada se **red generisan nizom** $(a_{n})$ $\Big($ili **red sa opštim članom** $a_{n}$$\Big)$ definiše kao zbir svih elemenata niza $(a_{n})$:
$\begin{align}\sum\limits_{n=1}^{\infty}a_{n}:=a_{1}+a_{2}+\cdots+a_{n}+\cdots\end{align}$ ^bf65f3
- $\begin{align}s_{n}=\sum\limits_{k=1}^{n}a_{k},\quad \forall i\in\mathbb{N}\end{align}$ $\quad$ je parcijalna suma reda.
- $\begin{align}(s_{n})=(s_{1},\,s_{2},\,\dots,\,s_{n},\,\dots)\end{align}$ $\quad$ je niz parcijalnih suma reda.

Ako $\exists\lim\limits_{ n \to \infty }s_{n}=s\in\mathbb{R}$, onda red $\begin{align}\sum\limits_{k=1}^{\infty}a_{k}\end{align}$ **konvergira** i jednak je $s$, inače **divergira**. ^7a6e28


$\:$
**Stav**. Neka je $(a_{n})$ niz. Tada
$\begin{align}\sum\limits_{n=1}^{\infty}a_{n}\quad\text{konvergira}\quad\Leftrightarrow\quad\sum\limits_{n=k}^{\infty}a_{n}\quad\text{konvergira za }\ \forall k\in\mathbb{N}\end{align}$ ^6bf0d1

**Stav**. Neka je $(a_{n})$ niz. Tada
$\begin{align}\sum\limits_{n=1}^{\infty}a_{n}\quad\text{konvergira}\quad\Rightarrow\quad\sum\limits_{n=1}^{\infty}\alpha \,a_{n}=\alpha\sum\limits_{n=1}^{\infty}a_{n}\quad\text{konvergira za }\ \forall \alpha\in\mathbb{R}\end{align}$

**Stav**. Neka su $(a_{n})$ i $(b_{n})$ nizovi. Tada
- $\begin{align}\sum\limits_{n=1}^{\infty}a_{n}\ \ \text{i}\ \ \sum\limits_{n=1}^{\infty}b_{n}\quad\text{konvergiraju}\quad\Rightarrow\quad\sum\limits_{n=1}^{\infty}(a_{n}+b_{n})=\sum\limits_{n=1}^{\infty}a_{k}+\sum\limits_{n=1}^{\infty}b_{k}\quad\text{konvergira}\end{align}$
$\:$
- $\begin{align}\sum\limits_{n=1}^{\infty}a_{n}\ \ \text{konvergira}\ \ \text{i}\ \ \sum\limits_{n=1}^{\infty}b_{n}\quad\text{divergira}\quad\Rightarrow\quad\sum\limits_{n=1}^{\infty}(a_{n}+b_{n})\quad\text{divergira}\end{align}$
$\:$ 
- $\forall n\in \mathbb{N}\quad a_{n},\,b_{n}\geqslant0$
$\begin{align}\sum\limits_{n=1}^{\infty}a_{n}\ \ \text{i}\ \ \sum\limits_{n=1}^{\infty}b_{n}\quad\text{divergiraju}\quad\Rightarrow\quad\sum\limits_{n=1}^{\infty}(a_{n}+b_{n})\quad\text{divergira}\end{align}$
> Napomena: ako nizovi nisu nenegativni onda zbir može i da konvergira.

$\:$
**Teorema**. Neka je $(a_{n})$ niz. Tada
$\begin{align}\sum\limits_{n=1}^{\infty}a_{n}\quad\text{konvergira}\quad\Rightarrow\quad\lim\limits_{ n \to \infty }a_{n}=0\end{align}$ ^7e0ab5
> Dokaz:
> Neka je $\begin{align}\sum\limits_{n=1}^{\infty}a_{n}=s\end{align}$
> 
> Parcijalna suma: $s_{n}=a_{1}+a_{2}+\dots+a_{n}$
> Odakle, $a_{n}=s_{n}-s_{n-1}$
> $\lim\limits_{ n \to \infty }a_{n}= \lim\limits_{ n \to \infty }(s_{n}-s_{n-1})=\lim\limits_{ n \to \infty }s_{n}-\lim\limits_{ n \to \infty }s_{n-1}=s-s=0$

> Napomena: često se koristi kontrapozicija teoreme (za dokazivanje divergencije).

$\:$
### Apsolutna i uslovna konvergencija

**Def**. Red $\begin{align}\sum\limits_{n=1}^{\infty}a_{n}\end{align}$ **konvergira apsolutno** ako $\begin{align}\sum\limits_{n=1}^{\infty}|a_{n}|\end{align}$ konvergira.

**Stav**. Ako red $\begin{align}\sum\limits_{n=1}^{\infty}a_{n}\end{align}$ konvergira apsolutno tada on konvergira. ^3872fa
> Dokaz: tvrđenje sledi iz [[Kriterijumi konvergencije redova brojeva#^9d13dd|stava]] uzimajući $b_{n}:=|a_{n}|,\quad\forall n\in\mathbb{N}$

$\:$
**Def**. Red $\begin{align}\sum\limits_{n=1}^{\infty}a_{n}\end{align}$ **konvergira uslovno** ako on sam konvergira a red $\begin{align}\sum\limits_{n=1}^{\infty}|a_{n}|\end{align}$ divergira.

$\:$
**Teorema**. Neka  $\begin{align}\sum\limits_{n=1}^{\infty} a_{n}=S\end{align}$ konvergira apsolutno. Ako je $p\ : \mathbb{N} \to \mathbb{N}$ proizvoljna bijekcija (tj. permutacija $\mathbb{N}$) onda $\begin{align}\sum\limits_{n=1}^{\infty} a_{p(n)}=S\end{align}$ konvergira apsolutno.

$\:$
**Teorema** (Rimanova). Neka  $\begin{align}\sum\limits_{n=1}^{\infty} a_{n}\end{align}$ konvergira uslovno. Tada $\forall A\in\overline{\mathbb{R}} \quad\exists p\ : \mathbb{N} \to \mathbb{N}$  bijekcija $\begin{align}\ \ :\ \ \sum\limits_{n=1}^{\infty} a_{p(n)}=A\end{align}$ 

### [[Kriterijumi konvergencije redova brojeva|Kriterijumi konvergencije]]
### [[Konvergencija nekih redova]] 