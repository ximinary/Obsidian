#fax #math #laag [deo poglavlja [[Vektor|"vektor"]]]
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
- v1) $\ \ [x,\,y]=-[y,\,x]$
- v2) $\ \ [\alpha\,x,\,y]=\alpha[x,\,y]$
- v3) $\ \ [x+y,\,z]=[x,\,z]+[y,\,z]$

(v2 i v3 važe za drugo mesto koristeći v1)
$\:$
- m1) $\ \ [x,\,y,\,z]=-[y,\,x,\,z]$
- m2) $\ \ [x,\,y,\,z]=[y,\,z,\,x]$
- m3) $\ \ [\alpha\,x,\,y,\,z]=\alpha[x,\,y,\,z]$
- m4) $\ \ [x+y,\,z,\,v]=[x,\,z,\,v]+[y,\,z,\,v]$

(m3 i m4 važe za drugo i treće mesto koristeći m2)
(iz m1 i m2 sledi: promena mesta dva vektora menja znak)

> Dokazi:
> 1.