#fax #math #alg  [deo [[Grupa|poglavlja "grupa"]]]
$\:$

**Def**. Neka su $(G_{1},\,*_{1}),\ (G_{2},\,*_{2}),\ \dots,\ (G_{n},\,*_{n})$ grupe. Direktan proizvod $(P,\,*)$ ovih grupa je:
- $P=G_{1}\times G_{2}\times \dots\times G_{n}$
- $(g_{1},\,g_{2},\,\dots,\,g_{n})*(g'_{1},\,g'_{2},\,\dots,\,g'_{n})=(g_{1}*_{1}g'_{1},\,g_{2}*_{2}g'_{2},\,\dots,\,g_{n}*_{n}g'_{n})$

$(P,\,*)$ jeste grupa:
- asocijativnost sledi direktno
- neutral $e=(e_{1},\,e_{2},\,\dots,\,e_{n})$
- inverz $(g_{1},\,g_{2},\,\dots,\,g_{n})^{-1}=(g_{1}^{-1},\,g_{2}^{-1},\,\dots,\,g_{n}^{-1})$

**Stav**. Grupa $\mathbb{Z}_{m}\times\mathbb{Z}_{n}$ je ciklična akko $\mathrm{NZD}(m,\,n)=1$.
> Dokaz: 
> $\boxed{\Rightarrow}$ Neka je $\mathrm{NZD}(m,\,n)=d>1$. Neka je $\begin{align}r=\frac{mn}{d}<mn\end{align}$.
> 
> Neka je $(s,\,t)\in\mathbb{Z}_{m}\times\mathbb{Z}_{n}$ proizvoljni.
> $\begin{align}\underbrace{s+_{m}s+_{m}\dots+_{m} s}_{r}=s\cdot_{m}r=(s\cdot_{m}m)\cdot_{m}\frac{n}{d}=0\end{align}$
> $\begin{align}\underbrace{t+_{n}t+_{n}\dots+_{n} t}_{r}=t\cdot_{m}r=(t\cdot_{n}n)\cdot_{n}\frac{m}{d}=0\end{align}$
> Odakle, $\underbrace{(s,\,t)+(s,\,t)+\dots+(s,\,t)}_{r}=(0,\,0)$
> Svaka grupa generisana sa $\Big\langle (s,\,t) \Big\rangle$ ima $\leqslant r$ elemenata, a $\mathbb{Z}_{m}\times\mathbb{Z}_{n}$ ima $mn>r$, stoga $\mathbb{Z}_{m}\times\mathbb{Z}_{n}$ nije ciklična.
> 
> $\boxed{\Leftarrow}$ Neka je $\mathrm{NZD}(m,\,n)=1$. Neka je $\omega\Big((1,\,1)\Big)=r$.
> Pokazati da $\mathbb{Z}_{m}\times\mathbb{Z}_{n}=\Big\langle (1,\,1) \Big\rangle$, tj da je $r=mn$
> $\underbrace{(1,\,1)+\dots+(1,\,1)}_{r}=(0,\,0)\quad\Rightarrow\quad\begin{align}&\underbrace{1+_{m}\dots+_{m}1}_{r}=0\quad\Rightarrow\quad m\,|\,r\\&\underbrace{1+_{n}\dots+_{n}1}_{r}=0\quad\Rightarrow\quad n\,|\,r\end{align}$
> Jer je $\mathrm{NZD}(m,\,n)=1$, dobijamo $mn\,|\,r$.
> Dakle, $mn=r$, jer $r\leqslant mn$ (red elementa grupe manje ili jednak redu grupe).

$\:$
> Napomena: $G\cong G'\ \ \land\ \ H\cong H'\quad\Rightarrow\quad G\times H\cong G'\times H'$

> Napomena: Ako su $m_{1},\,m_{2},\,\dots,\,m_{n}$ par po par uzajamno prosti. Tada  
> - $\mathbb{Z}_{m_{1}m_{2}\dots m_{n}}\cong \mathbb{Z}_{m_{1}}\times\mathbb{Z}_{m_{2}}\times\dots\mathbb{Z}_{m_{n}}$
> - $\mathbb{C}_{m_{1}m_{2}\dots m_{n}}\cong \mathbb{C}_{m_{1}}\times\mathbb{C}_{m_{2}}\times\dots\mathbb{C}_{m_{n}}$

$\:$
**Stav**. Neka je $G$ grupa. $H,\,K\leqslant G$ takvi da
$\ \:$ — $\ \:$ $G=H\cdot K$
$\ \:$ — $\ \:$ $\forall h\in H\quad\forall k\in K\quad h\cdot k=k\cdot h$
$\ \:$ — $\ \:$ $K\cap H=\{e\}$
Tada $G\cong H\times K$.

> Dokaz: $H\cdot K=\{h\cdot k \ \ |\ \ h\in H,\ k\in K\}$
> Definišemo $f:\ H\times K\to G$ sa $f(h,\,k)=h\cdot k$
> 
> $f$ je "na" jer $G= H\cdot K$
> 
> pp da $f(h,\,k)=f(h',\,k')$, $\ \:$ tj. $\ \:$ $h\cdot k=h'\cdot k'$, 
> dalje, $(h')^{-1}\cdot h = k'\cdot k^{-1}$, stoga jer je levi deo jednačine iz $H$, a desni iz $K$ na osnovu $K\cap H=\{e\}$ važi 
> $\begin{align}(h')^{-1}\cdot h=e\quad\Rightarrow\quad h =h'\\k'\cdot k^{-1}=e\quad\Rightarrow\quad k =k'\end{align}\quad\quad\Rightarrow\quad$ $f$ je "1-1".
> 
> $\begin{align}f\Big((h,\,k)*(h',\,k')\Big)&=f\Big((h\cdot h',\ k\cdot k')\Big)=h\cdot h'\cdot k\cdot k'\xlongequal{\text{drugi uslov}} h\cdot k\cdot h'\cdot k'=\\&=f(h,\,k)\cdot f(h',\,k')\end{align}$
>
> Konačno, $f$ je izomorfizam grupa $H\times K$ i $G$.


> Primer: $\mathbb{D}_{6}\cong\mathbb{D}_{3}\times\mathbb{Z}_{2}$