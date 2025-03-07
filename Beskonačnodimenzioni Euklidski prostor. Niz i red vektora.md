#fax #math #a2 [deo [[Analiza|analize]] i poglavlja [[Unitarni prostor. Euklidski prostor|"unitarni i Euklidski prostor"]]]

### Niz vektora Euklidskog prostora
**Def**. Neka je $(u_{n})$ niz vektora [[Unitarni prostor. Euklidski prostor|Euklidskog prostora]] $V$. Niz $(u_{n})$ konvergira ka vektoru $u\in V$  $\Big(\lim\limits_{ n \to \infty } u_{n}=u\Big)$ ako za [[Niz brojeva|niz realnih brojeva]] $||u_{n} −u||$ važi $\lim\limits_{ n \to \infty }||u_{n}-u||=0$ 
tj. $\forall\varepsilon>0 \quad\exists N\in\mathbb{N}\quad\forall n\geqslant N\quad||u_{n}-u||<\varepsilon$ ^890b7c

$\:$
**Def**. Niz vektora $(u_{n})$ u Euklidskom prostoru $V$ je [[Košijev niz]] ako 
$\forall\varepsilon>0 \quad\exists N\in\mathbb{N}\quad\forall m,\,n\geqslant N\quad||u_{m}-u_{n}||<\varepsilon$

$\:$
**Def**. Ako svaki Košijev niz u Euklidskom prostoru $V$ konvergira onda je $V$ **Hilbertov prostor**.

### Red vektora Euklidskog prostora
**Def**. Neka je $(u_{n})$ niz vektora [[Unitarni prostor. Euklidski prostor|Euklidskog prostora]] $V$. Tada se **red generisan nizom** $(u_{n})$ definiše kao zbir svih elemenata niza $(u_{n})$:
$\begin{align}\sum\limits_{n=1}^{\infty}u_{n}:=u_{1}+u_{2}+\cdots+u_{n}+\cdots\end{align}$ ^bf65f3
- $\begin{align}s_{n}=\sum\limits_{k=1}^{n}u_{k},\quad \forall i\in\mathbb{N}\end{align}$ $\quad$ je parcijalna suma reda (jeste vektor iz $V$).
- $\begin{align}(s_{n})=(s_{1},\,s_{2},\,\dots,\,s_{n},\,\dots)\end{align}$ $\quad$ je niz parcijalnih suma reda.

Ako $\exists\lim\limits_{ n \to \infty }s_{n}=s\in\mathbb{R}$, onda red $\begin{align}\sum\limits_{k=1}^{\infty}a_{k}\end{align}$ **konvergira** i jednak je $s$, inače **divergira**. 

### Ortonormirani niz vektora
**Def**. Neka je $V$ beskonačnodimenzioni Euklidski prostor (sa skalarnim proizvodom $\langle\, ,\,\rangle$) i neka je $(e_{n})$ niz vektora u $V$. Ako elementi skupa $\{e_{n}\}_{n\in\mathbb{N}}$ čine ortonormirani sistem vektora (tj. [[Unitarni prostor. Euklidski prostor#^03b838|ortogonalni skup]] jediničnih vektora) u $V$, onda je niz vektora $(e_{n})$ **ortonormirani niz vektora u prostoru** $V$ (baza od $V$). ^e6bffc

**Def**. $\forall n \in \mathbb{N}\quad v_{n}= \langle v,\ e_{n}\rangle$ zovu se **Furijeovi koeficijenti** vektora $v$ u u odnosu na ortonormirani niz $e_{n}$. 

**Def**. Red vektora $\begin{align}\sum\limits_{n=1}^{\infty} \langle v,\,e_{n}\rangle\,e_{n}\end{align}$ naziva se **Furijeov red** vektora $v$ u odnosu na ortonormirani niz vektora $e_{n}$. ^e69126

___
**Teorema** (Beselova nejednakost). $\forall v\in V$. $(e_{n})$ je ortonormirani niz vektora u prostoru $V$. Tada $\begin{align}\langle v,\ v\rangle\geqslant \sum\limits_{n=1}^{\infty} \Big|\langle v,\ e_{n}\rangle\Big|^{2}\end{align}$ $\quad$ (i red konvergira).

**Posledica**. Za $v\in V$ važi $\lim\limits_{ n \to \infty } \langle v,\,e_{n}\rangle=0$

**Lema**. $u_{n},\,v_{n}\in V$. Ako $\lim\limits_{ n \to \infty }u_{n}=u$ i $\lim\limits_{ n \to \infty }v_{n}=v$, onda $\lim\limits_{ n \to \infty }\langle u_{n},\,v_{n}\rangle=\langle u,\,v\rangle$

**Teorema**. Sledeći iskazi su ekvivalentni.
1. $\begin{align}\forall v\in V\quad\forall\varepsilon>0\quad\exists n\in\mathbb{N}\quad\exists \lambda_{1},\,\lambda_{2},\,\dots,\,\lambda_{n}\in\mathbb{R}\quad\bigg|\bigg|u-\sum\limits_{k=1}^{n}\lambda_{k}e_{k}\bigg|\bigg|<\varepsilon\end{align}$
2. $\begin{align}\forall v\in V\quad \sum\limits_{n=1}^{\infty}\langle v,\,e_{n}\rangle\,e_{n}=v\end{align}$ $\quad$ (Furijeov red konvergira)
3. $\begin{align}\forall v\in V\quad \sum\limits_{n=1}^{\infty}\langle v,\,e_{n}\rangle^{2}=||v||\end{align}$ $\quad$ (Parsevalova jednakost)

Ako je tačan jedan od iskaza (a samim tim i sve) niz $(e_{n})$ je **potpun ortonormiran niz**.
### [[Prostor C₀]]