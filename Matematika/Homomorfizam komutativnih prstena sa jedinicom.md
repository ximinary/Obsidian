#fax #math #alg [deo [[Komutativan prsten sa jedinicom|poglavlja "prsten"]]]
$\:$ 

**Def**. Neka su $(A,\,+,\,\cdot)$ i $(B,\,+',\,\cdot')$ dva komutativnih prstena sa jedinicom. Funkcija $f:\ A\to B$ je homomorfizam komutativnih prstena sa jedinicom, ako 
- $\forall x,\,y\in A\quad f(x+y)=f(x)+f(y)$
- $\forall x,\,y\in A\quad f(x\cdot y)=f(x)\cdot f(y)$
- $f(1_{A})=1_{B}$

**Def**. Neka je $f:\ A\to B$ homomorfizam komutativnih prstena sa jedinicom. Tada je **jezgro homomorfizma** $\ \:$ $\mathrm{Ker}\,f=\{x\in A\ \big|\ f(x)=0_{B}\}$.

**Stav**. Neka je $f:\ A\to B$ homomorfizam komutativnih prstena sa jedinicom. Tada ([[Direktna i inverzna slika skupa|*]])
- $(\mathrm{Ker}\,f) \triangleleft A$ ^131642
-  $J\triangleleft B\quad\Rightarrow\quad f^{-1}[J]\triangleleft A$ ^7dc661
-  $I\triangleleft A\ \ \text{ i }\ \ f \text{ je "na"}\quad\Rightarrow\quad f[J]\triangleleft B$ ^2b3501

> Dokaz:
> - Neka $x,\,y\in \mathrm{Ker}\, f,\ \ a\in A$
>   $f(x+y)=f(x)+'f(y)=0_{B}+0_{B}=0_{B}\quad\Rightarrow\quad x+y\in \mathrm{Ker}\, f$
>   $f(a\cdot x)=f(a)\cdot' f(x)=f(a)\cdot 0_{B}=0_{B}\quad\Rightarrow\quad a\cdot x\in \mathrm{Ker}\,f$
>   $\:$
> - Neka je $J$ ideal u $B$ i neka su $x,\,y\in f^{-1}[J],\ \ a\in A$.
>   Tada $f(x),\,f(y)\in J$, a $f(a)\in B$ stoga 
>   $f(x)+'f(y)=f(x+y)\in J\quad\Rightarrow\quad x+y\in f^{-1}[J]$
>   $f(a)\cdot'f(y)=f(a\cdot x)\in J\quad\Rightarrow\quad a\cdot x\in f^{-1}[J]$
>   $\:$
> - Neka je $I$ ideal u $A$ i neka su $u,\,v\in f[I],\ \ b\in B$.
>   Tada $\exists x,\,y\in I\ \ :\ \ f(x)=u,\,f(y)=v$
>   takođe jer je $f$ "na", $\ \:$ $\exists a\in A\quad f(a)=b$ 
>   $x+y\in I\quad \Rightarrow\quad f(x+y)=f(x)+'f(y)=u+'v\in f[I]$
>   $x\in I,\ a\in A\quad\Rightarrow\quad f(a\cdot x)=f(a)\cdot'f(x)=b\cdot' u\in f[I]$

$\:$
**Stav**. Neka je $f:\ A\to B$ homomorfizam komutativnih prstena sa jedinicom. Tada $\mathrm{Ker}\,f=\{0_{A}\}\quad\Leftrightarrow\quad f$ je "1-1". ^2420ae

$\:$
> Napomena: [[Potprsten i ideal#^15271e|Stav]] se dokazuje pomoću homomorfizma.

$\:$
### Izomorfizam
**Def**. Homomorfizam komutativnih prstena sa jedinicom je **izomorfizam**, ako je bijekcija. Oznaka: $A\cong B$.
> Napomena: [[Potprsten i ideal#Kongruencija po idealu|kongruencije]]

$\:$
**Teorema** (o izomorfizmu). Neka je $f:\ A\to B$ homomorfizam komutativnih prstena sa jedinicom. Tada $f$ indukuje izomorfizam $\ \:$ $\tilde{f}:\ A/\mathrm{Ker}\,f\to\mathrm{Im}\,f$ $\ \:$ definisan sa $\ \:$ $\tilde{f}(a+\mathrm{Ker}\,f):=f(a)$ $\ \:$ i važi $\ \:$ $A/\mathrm{Ker}\,f \cong \mathrm{Im}\, f$. ^023ba8
> Dokaz: Prvo pokažemo da je $\tilde{f}$ dobro definisana $(\Rightarrow)$, kao i da je "1-1" $(\Leftarrow)$:
> $a+\mathrm{Ker}\,f=b+\mathrm{Ker}\,f\quad\Leftrightarrow\quad a-b\in \mathrm{Ker}\,f\quad\Leftrightarrow\quad f(a-b)=0$
> $\Leftrightarrow\quad f(a)=f(b)\quad\Leftrightarrow\quad\tilde{f}(a+\mathrm{Ker}\,f)=\tilde{f}(b+\mathrm{Ker}\, f)$
> Jasno je da je $\tilde{f}$ "na".
> Da li $\tilde{1}$ slika $1_{A/\mathrm{Ker}\, f}$ u $1_{B}$?
> $\tilde{f}(1_{A}+\mathrm{Ker}\,f)=f(1_{A})=1_{B}$.
> Zaključujemo da je $\tilde{f}$ izomorfizam.

$\:$
**Stav**. $\mathbb{Z}_{m}\cong \mathbb{Z}/m\mathbb{Z}$ ^f4e2f8
> Dokaz:
> $\rho_{n}:\ \mathbb{Z}\to \mathbb{Z}_{n}$ def. sa $\rho_{n}(x)=x\,\mathrm{mod}\,n$ je homomorfizam.
> $\mathrm{Ker}\,\rho_{n}=m\mathbb{Z}$
> Iz teoreme o izomorfizmu dobije se tvrđenje.


$\:$
**Stav**. Nek su $A\cong B$ komutativni prsteni sa jedinicom. Tada $\big(U(A),\,\cdot\big)\cong\big(U(B),\,\cdot\big)$ ^8cba06
> Dokaz: ([[Invertibilni elementi u prstenu. Polje i domen#^d07f3d|*]])
> Neka je $f$ izomorfizam prstena.
> 
> Homomorfizam prstena slika invertibilni element u invertibilni?
> Neka je $a\in U(A)$, tada $\exists a'\in U(A)\ \ \:\ \ a\cdot a'=1_{A}$
> $f(a)\cdot f(a')=f(a\cdot a')=f(1_{A})=1_{B}\quad\Rightarrow\quad f(a)\in U(B)$ 
> Prema tome, $f[U(A)]\subseteq U(B)$
> Stoga, restrikcija $f\big|_{U(A)}:\ U(A)\to U(B)$ jeste homomorfizam grupa $\big(U(A),\,\cdot\big)$ i $\big(U(B),\,\cdot\big)$.
>
> "1-1": svojstvo se čuva na restrikciji.
>
> "na": kako je $f$ izomorfizam prstena, $\forall b\in U(b)\quad\exists a\in A\quad f(a)=b$,
> a koko je $b$ invertibilni $\exists b'\in U(B)\quad b'\cdot b=1_{B}$
> i za $b'\quad\exists \overline{a}\in A\quad f(\overline{a})=b'$
> imamo $1_{B}=b'\cdot b =f(\overline{a})\cdot f(a)=f(\overline{a}\cdot a)\quad\xRightarrow{{f} \text{ je "1-1"}}\quad \overline{a}\cdot a=1_{A}\quad\Rightarrow\quad a\in U(A)$.


