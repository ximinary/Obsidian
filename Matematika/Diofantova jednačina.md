#fax #math #ds1 [deo poglavlja [[Celi brojevi|"celi brojevi"]]]
$\:$

**Def**. **Diofantova** je jednačina sa celobrojnim koeficijentima, u kojoj treba naći sva rešenja u $\mathbb{Z}$

- $a\,x = b\quad a,\,b\in \mathbb{Z},\ a\ne 0$
Ima jedinstveno rešenje $x = \frac{b}{a}$, ako $a\,|\,b$ (inače nema rešenja)
- $a\,x+b\,y=c\quad  a,\,b,\,c\in \mathbb{Z},\ a\ne 0,\ b\ne 0$
Treba naći sve parove $(x,\,y)$ da bi važila jednačina:

>$d := \mathrm{NZD}(a,\,b)$ tada (iz [[Euklidov algoritam#^e5f1a9|posledice Euklidovog algoritma]])
$\exists u,\,v\in \mathbb{Z}\ \ :\ \ a\,u + b\,v = d$
>
>Stav. $a\,x+b\,y=c$ ima rešenja akko $\mathrm{NZD}(a,\,b)\,|\,c$
> > [$\Leftarrow$] 
> > Ako $d\,|\,c$, tada $c':= \frac{c}{d}$ 
> > Pomnožimo jednačinu $a\,u + b\,v = d$ sa $c'$:
> > $a\,u\,c' + b\,v\,c' = c$
> > Odakle imamo jedno rešenje: $(u\,c',\,v\,c')$
> > 
> > [$\Rightarrow$] 
> > Ako $\exists$ rešenje $a\,x+b\,y=c$
> > $\mathrm{NZD}(a,\,b) = d$, tada $d\,|\,a$ i $d\,|\,b$
> > $\Rightarrow \ \ d\,|\,(a\,x+b\,y)\ \ \Rightarrow \ \ d\,|\,c$
> > 
>
>Potražimo sva rešenja jednačine:
>imamo jedno rešenje $(x_{0},\,y_{0}):=(u\,c',\,v\,c')$ 
>važi $a\,x_{0}+b\,y_{0}=c$ 
>
>Tada je $a\,x+b\,y=c$ isto što i $a\,x+b\,y=a\,x_{0}+b\,y_{0}$
>$a\,(x-x_{0}) = -b\,(y-y_{0})$
>
>$\mathrm{NZD}(a,\,b)=d$
>$\begin{aligned} a = a'\,d \\ b = b'\,d\end{aligned} \ \ \Rightarrow\ \ \mathrm{NZD}(a',\,b') = 1$
>
>Vratimo to u jednačinu:
>$a'\,d\,(x-x_{0}) = -b'\,d\,(y-y_{0})$
>$a'\,(x-x_{0}) = -b'\,(y-y_{0})$
>
>$\begin{aligned} b'\,|\,a'\,(x-x_{0}) \\ \mathrm{NZD}(a',\,b') = 1\end{aligned} \ \ \Rightarrow\ \ b'\,|\,(x-x_{0})\ \ \Rightarrow\ \ \exists t\in \mathbb{Z}\ :\ x-x_{0}=b'\,t$
>
>$x = x_{0} + b'\,t$
>$a'\,b'\,t=-b'(y-y_{0})\ \ \Rightarrow\ \ y = y_{0}-a'\,t$
>
>Opšte rešenje jednačine:
>$\begin{aligned} x= u\,c' + b'\,t\quad\quad\quad x = \frac{c\,u+b\,t}{d}\\ y=v\,c' - a'\, t\quad\quad\quad y = \frac{c\,v-a\,t}{d}\end{aligned}\quad\quad\quad\forall t\in \mathbb{Z},$
>gde su $u$, $v$ brojevi iz [[Euklidov algoritam#^e5f1a9|posledice Euklidovog algoritma]] za $a$ i $b$ $\:$ (tj važi $a\,u+b\,v=d$)

[[diofantova jednačina primer.png|Primer]]