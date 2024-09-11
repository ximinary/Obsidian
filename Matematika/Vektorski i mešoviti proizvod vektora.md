#fax #math #laag [deo poglavlja [[Vektor|"vektor"]]]
$\:$

> $(x,\,y,\,z)$ je **pozitivna** trojka vektora ako su predstavnici $\overrightarrow{\rm OA},\,\overrightarrow{\rm OB},\,\overrightarrow{\rm OC}$ vektora $x,\,y,\,z\:$ takve da gledajući sa $\mathrm{C}$ kraći put od $\mathrm{A}$ do $\mathrm{B}$ je u smeru suprotnom od smera satne kazaljke; u suprotnom je **negativna**.
> 
> Pozitivnost/negativnost trojke se menja ako:
> - Dva vektora se menjaju mestima.
> - Jedan vektor se množi sa negativnim brojem.
> 
>  Na primer ako je $(x,\,y,\,z)$ pozitivna onda
> $(y,\,x,\,z)$, $(z,\,y,\,x)$ i $(x,\,y,\,-z)$  su negativne;
> $(z,\,x,\,y)$, $(-z,\,y,\,x)$ i $(x,\,-z,\,y)$ su pozitivne.

$\:$
### Vektorski i mešoviti proizvod
**Def**. **Vektorski** (spoljašnji) **proizvod** je funkcija $\times:\ V\times V\to V$, takva da $\forall x,\,y\in V\quad\exists x\times y\ \ :$
1. $||x\times y||=||x||\,||y||\,\sin\widehat{(x,\,y)}$ $\ \,\quad\quad$ — dužina 
   (površina paralelograma određenog sa $x,\,y$)
   $\:$
2. $x\cdot(x\times y)=0,\quad y\cdot(x\times y)=0$ $\quad$ — pravac
   $\:$
3. $(x\times y,\,x,\,y)$ je pozitivna trojka $\ \ \!\quad$ — orijentacija

Oznake: $\ \ x\times y;\quad[x,\,y]$
$\:$

**Def**. Mešoviti proizvod je funkcija $[\cdot,\,\cdot,\,\cdot]\ :\ \ V\times V\times V \to \mathbb{R}$, takva da $\forall x,\,y,\,z\in V\quad[x,\,y,\,z]=(x\times y)\cdot z$

**Teorema**. $\Big|[x,\,y,\,z]\Big|$ je zapremina paralelepipeda određenog sa $z,\,y,\,z.$

**Teorema** (Svojstva). $\forall x,\,y,\,z,\,v\in V \:$ i $\ \forall\alpha\in\mathbb{R}$ važe:
- **v1**) $\ \ [x,\,y]=-[y,\,x]$
- **v2**) $\ \ [\alpha\,x,\,y]=\alpha[x,\,y]$
- **v3**) $\ \ [x+y,\,z]=[x,\,z]+[y,\,z]$
- **v4**) $\ \ [x,\,[y,\,z]]+[y,\,[z,\,x]]+[z,\,[x,\,y]]=0$

(**v2** i **v3** važe za drugo mesto koristeći **v1**)
$\:$
- **m1**) $\ \ [x,\,y,\,z]=-[y,\,x,\,z]$
- **m2**) $\ \ [x,\,y,\,z]=[y,\,z,\,x]$
- **m3**) $\ \ [\alpha\,x,\,y,\,z]=\alpha[x,\,y,\,z]$
- **m4**) $\ \ [x+y,\,z,\,v]=[x,\,z,\,v]+[y,\,z,\,v]$

(**m3** i **m4** važe za drugo i treće mesto koristeći **m2**)
(iz **m1** i **m2** sledi: promena mesta dva vektora menja znak)

> Dokazi: 
> **v1** i **v2** iz definicije vektorskog proizvoda.
> **m1** i **m3** iz  **v1** i **v2**.
> 
> **m2**) Iz prethodne teoreme $\Big|[x,\,y,\,z]\Big|=\Big|[y,\,z,\,x]\Big|$ je zapremina paralelepipeda određenog sa $z,\,y,\,z.$
> — Ako $[x,\,y,\,z]>0$ $\: \ \Rightarrow\ \:$ $x\times y$ i $z$ su sa jedne strane od ravne $xy$ $\: \ \Rightarrow\ \:$ $(x,\,y,\,z)$ je pozitivna trojka $\: \ \Rightarrow\ \:$ $y\times z$ i $x$ su sa jedne strane od ravne $yz$ $\: \ \Rightarrow\ \:$ $[y,\,z,\,x]>0$
> — Ako $[x,\,y,\,z]<0$ $\: \ \Rightarrow\ \:$ $x\times y$ i $z$ su sa različitih strana od ravne $xy$ $\: \ \Rightarrow\ \:$ $(x,\,y,\,z)$ je negativna trojka $\: \ \Rightarrow\ \:$ $y\times z$ i $x$ su sa različitih strana od ravne $yz$ $\: \ \Rightarrow\ \:$ $[y,\,z,\,x]<0$
> Dakle, $[x,\,y,\,z]=[y,\,z,\,x]$
>
> **m4**) $[x+y,\,z,\,v]\xlongequal{\text{m2}}[z,\,v,\,x+y]=[z,\,v]\cdot(x+y)\xlongequal{\text{svojstva skalarnog proizvoda}}$
> $=[z,\,v]\cdot x + [z,\,v]\cdot y=[z,\,v,\,x]+[z,\,v,\,y]\xlongequal{\text{m2}}[x,\,z,\,v]+[y,\,z,\,v]$
> 
> **v3**) $[x+y,\,z]\cdot v\xlongequal{\text{m4}}\Big([x,\,z]+[y,\,z]\Big)\cdot v\quad\Rightarrow$
> $\Rightarrow \quad [x+y,\,z]=[x,\,z]+[y,\,z]$
> 
> **v4** ćemo dokazati kasnije.

$\:$
### Vektorski i mešoviti proizvod u koordinatama
Neka je $(e_{1},\,e_{2},\,e_{3})$ ortonormirana baza vektorskog prostora $V$.
$\varepsilon=\begin{cases}1,\quad\ \ \ \text{ako je }(e_{1},\,e_{2},\,e_{3})\text{ pozitivna}\\-1,\quad\text{ako je }(e_{1},\,e_{2},\,e_{3})\text{ negativna}\end{cases}$

> Asimetričan Kronekerov simbol:
> $\begin{cases}\varepsilon_{123}=\varepsilon_{231}=\varepsilon_{312}=\varepsilon\\\varepsilon_{132}=\varepsilon_{213}=\varepsilon_{321}=-\varepsilon\\\varepsilon_{ijk}=0,\quad\text{ako }\ i=j\ \text{ ili }\ i=k\ \text{ ili }\ j=k\end{cases}$
> 
> $e_{i}\times e_{j}=\sum\limits_{k=1}^{3}\varepsilon_{ijk}\,e_{k}$
> $[e_{i},\,e_{j},\,e_{k}]=\varepsilon_{ijk}$

$x = x_{1}\,e_{1}+x_{2}\,e_{2}+x_{3}\,e_{3}$
$y = y_{1}\,e_{1}+y_{2}\,e_{2}+y_{3}\,e_{3}$
$z = z_{1}\,e_{1}+z_{2}\,e_{2}+z_{3}\,e_{3}$

$x\times y=\sum\limits_{i,\,j=1}^{3}x_{i}\,y_{j}\,(e_{i}\times e_{j})=\sum\limits_{i,\,j,\,k=1}^{3}\varepsilon_{ijk}\,x_{i\,}y_{j}\,e_{k}=\varepsilon\ \begin{array}{|c c c|}e_{1}&e_{2}&e_{3}\\ x_{1}&x_{2}&x_{3}\\ y_{1}&y_{2}&y_{3}\end{array}$

$[x,\,y,\,z]=\bigg(\sum\limits_{i,\,j,\,k=1}^{3}\varepsilon_{ijk}\,x_{i\,}y_{j}\,e_{k}\bigg)\cdot\bigg(\sum\limits_{k=1}^{3}z_{k}\,e_{k}\bigg)=$

$\quad\quad\quad\ \,=\sum\limits_{i,\,j,\,k=1}^{3}\varepsilon_{ijk}\,x_{i\,}y_{j}\,z_{k}=\varepsilon\ \begin{array}{|c c c|}x_{1}&x_{2}&x_{3}\\ y_{1}&y_{2}&y_{3}\\ z_{1}&z_{2}&z_{3}\end{array}$

### Neasocijativnost $\times$
[[neasocijativnostVektProizv.png|Teorema]]. $\forall x,\,y,\,z\in V\quad(x\times y)\times z= (x\cdot z)\,y-(y\cdot z)\,x$

Posledica. $\times$ je neasocijativna.
> Dokaz: 
> $x\times(y\times z)=-x\times(z\times y)=(z\times y)\times x\xlongequal{\text{Teorema}}(z\cdot x)\,y-(y\cdot x)\,z$
> $(x\times y)\times z\xlongequal{\text{Teorema}}(x\cdot z)\,y-(y\cdot z)\,x$
> 
> pps $\times$ je asocijativna, tada:
> $\begin{align}x\times(y\times z)&=(x\times y)\times z\\ (z\cdot x)\,y-(y\cdot x)\,z&=(x\cdot z)\,y-(y\cdot z)\,x\\(y\cdot x)\,z&=(y\cdot z)\,x \end{align}$
> Što ne važi za $\forall x,\,y,\,z$, na primer:
> $x= (1,\,0,\,0),\quad y=(1,\,1,\,1),\quad z=(0,\,1,\,0)$
> odakle $\ y\cdot z=1,\quad y\cdot z=1;\quad$Tada $x=z.$ Kontradikcija. 

>Dokaz **v4**:
> Iz teoreme
> $\begin{array}{c|}x\times(y\times z)=(z\cdot x)\,y-(y\cdot x)\,z\\ y\times(z\times x)=(x\cdot y)\,z-(z\cdot y)\,x\\ z\times(x\times y)=(y\cdot z)\,x-(x\cdot z)\,y\end{array}\quad\Rightarrow$
> 
> $\Rightarrow\quad x\times(y\times z)+y\times(z\times x)+z\times(x\times y)=0$