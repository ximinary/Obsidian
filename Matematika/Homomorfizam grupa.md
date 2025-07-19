#fax #math #alg  [deo [[Grupa|poglavlja "grupa"]]]
$\:$

**Def**. Neka su $(G,\,\cdot)$ i $(H,\,*)$ grupe. Funkcija $f:\ G\to H$, takva da $\forall x,\,y\in G\quad f(x\cdot y)=f(x)*f(y)$,  zove se  **homomorfizam grupa** $G$ i $H$.

> Napomena: Slično [[Grupa#Izomorfizam grupa|izomorfizmu]] neutral se slika u neutral ([[Grupa#^60085a|*]]), a slika inverza jednaka je inverzu slike ([[Grupa#^9b7621|*]]).

$\:$
**Def**. Neka je $f:\ G\to H$ homomorfizam grupa. 
- **Jezgro homomorfizma** $f$ je $\mathrm{Ker}\,f:=\Big\{g\in G\ \Big|\ f(g)=e_{H}\Big\}$
- **Slika homomorfizma** $f$ je $\mathrm{\mathrm{Im}\,}\,f:=\Big\{h\in H\ \Big|\ \exists g\in G\quad h=f(g)\Big\}$

**Stav**. Neka je $f:\ G\to H$ homomorfizam. Tada $(\mathrm{Ker}\,f)\triangleleft G$

> Dokaz: 
> Prvo, pomoću [[Grupa#^2ea486|stava]] pokažemo $(\mathrm{Ker}\,f)\leqslant G$
> Jer $f(e_{G})=e_{H}$, $\ \:$ $\mathrm{Ker}\,f\ne\varnothing$
> Neka su $x,\,y\in \mathrm{Ker}\,f$, $\ \:$ tj. $f(x)=f(y)=e_{H}$
> $f(x\cdot y^{-1})=f(x)*f(y)^{-1}=e_{H}*e_{H}^{-1}=e_{H}$
> tj. $x\cdot y^{-1}\in \mathrm{Ker}\, f$. 
> Odakle sledi  $(\mathrm{Ker}\,f)\leqslant G$
> 
> Dalje, pomoću [[Normalne podgrupe#^b96173|stava]] ([[Normalne podgrupe#^c2938d|2.]]$\Rightarrow$[[Normalne podgrupe#^39f461|1.]]) pokažemo $(\mathrm{Ker}\,f)\triangleleft G$.
> Zapravo, neka je $x\in \mathrm{Ker}\, f$. Tada $\forall g\in G\quad f(gxg^{-1})=f(g)f(x)f(g)^{-1}=f(g)e_{H}f(g)^{-1}=e_{H}$,
> tj. $g(\mathrm{Ker}\,f)g^{-1}\subseteq\mathrm{Ker}\,f$
> Dakle, $(\mathrm{Ker}\,f)\triangleleft G$


$\:$
**Stav**. Neka je $f:\ G\to H$ homomorfizam. Tada
$f$ je "1-1" $\quad\Leftrightarrow\quad$ $\mathrm{Ker}\,f=\{e_{G}\}$ ^859a1b

> Dokaz: 
> $\boxed{\Rightarrow}$ Neka je $\mathrm{Ker}\,f\ne \{e_{G}\}$, $\ \:$ tj. $\exists x\in \mathrm{Ker}\, f\quad x\ne e_{G}$
> $f(e_{G})=f(x)=e_{H}$, $\ \:$ tj. $f$ nije "1-1"
> $\boxed{\Leftarrow}$ Neka je $\mathrm{Ker}\,f=\{e_{G}\}$.
> Pretpostavimo da za neke $x,\,y\in G\quad f(x)=f(y)$
> Tada $f(x\cdot y^{-1})=f(x)*f(y)^{-1}=f(x)*f(x)^{-1}=e_{H}$
> tj. $x\cdot y^{-1}\in \mathrm{Ker}\,f$, a jer je $\mathrm{Ker}\,f=\{e_{G}\}$, $\ \:$ $x\cdot y^{-1}=e_{G}$.
> Odakle je $x=y$, tj. je $f$ "1-1"

$\:$
**Stav**. Neka je $f:\ G\to H$ homomorfizam. Tada $(\mathrm{Im}\,f)\leqslant H$
> Dokaz:
> Kako je $f(e_{G})=e_{H}$, $\ \:$ $\mathrm{Im}\,\ne \varnothing$.
> Neka su $y_{1},\,y_{1}\in H$, tad 
> $\exists x_{1},\,x_{2}\in G\ \ :\ \ y_{1}=f(x_{1})\ \text{ i }\ y_{2}=f(x_{2})$
> $y_{1}* y_{2}^{-1}=f(x_{1})* f(x_{2})^{-1}=f(x_{1}\cdot x_{2}^{-1})\in \mathrm{Im}\, f$
> Iz [[Grupa#^2ea486|stava]] imamo $(\mathrm{Im}\,f)\leqslant H$


$\:$
**Teorema**. Neka je $f:\ G\to H$ homomorfizam grupa. Tada $f$ indukuje izomorfizam $\ \:$ $\tilde{f}:\ G/\mathrm{Ker}\,f\to\mathrm{Im}\,f$ $\ \:$ definisan sa $\ \:$ $\tilde{f}(x\mathrm{Ker}\,f):=f(x)$ $\ \:$ i važi $\ \:$ $G/\mathrm{Ker}\,f \cong \mathrm{Im}\, f$.
> Dokaz: Prvo pokažemo da je $\tilde{f}$ dobro definisana.
> Neka su $x\mathrm{Ker}\,f=y\mathrm{Ker}\,f$. Iz [[Red grupe i elementa. Indeks podgrupe#^a82139|stava]], $xy^{-1}\in\mathrm{Ker}\,f$, tj. $f(x^{-1}y)=e_{H}$
> $e_{H}=f(x^{-1}y)=f(x)^{-1}*f(y)\quad\Rightarrow\quad f(x)=f(y)\quad\Rightarrow\quad \tilde{f}(x\mathrm{Ker}\,f)=\tilde{f}(y\mathrm{Ker}\,f)$
> 
> $\tilde{f}$ je homomorfizam:
> $\tilde{f}\big((x\mathrm{Ker}\,f)\cdot(y\mathrm{Ker}\,f)\big)=\tilde{f}\big((xy)\mathrm{Ker}\,f\big)=f(xy)=f(x)*f(y)=\tilde{f}(x\mathrm{Ker}\,f)*\tilde{f}(y\mathrm{Ker}\,f)$
> 
> Iz definicije $\tilde{f}$ je jasno da $\mathrm{Im}\, f=\mathrm{Im}\,\tilde{f}$, tj. je $\tilde{f}$ "na".
> Da bismo pokazali da je $\tilde{f}$ "1-1" koristimo [[Homomorfizam grupa#^859a1b|stav]], tj. treba pokazati $\mathrm{Ker}\,\tilde{f}=\{\mathrm{Ker}\,f\}$ ($\mathrm{Ker}\,f=e_{G}\mathrm{Ker}\,f$ je neutral u grupi $G/\mathrm{Ker}\,f$).
> pps $\exists x\mathrm{Ker}\,f\ne \mathrm{Ker}\,f\ \ :\ \ \tilde{f}(x\mathrm{Ker}\,f)= e_{H}$. 
> $e_{H}=\tilde{f}(x\mathrm{Ker}\,f)=f(x)\quad\Rightarrow\quad x\in \mathrm{Ker}\, f\quad\Rightarrow\quad x\mathrm{Ker}\,f=\mathrm{Ker}\, f$ $\quad$ kontradikcija. 
> 
> $\tilde{f}$ je bijekcija i samim tim je izomorfizam.


$\:$
**Posledica** (prethodne i [[Red grupe i elementa. Indeks podgrupe#^cd291f|Lagranžove teoreme]]). Neka je $f:\ G\to H$ homomorfizam grupa. Tada $|G|=|\mathrm{Ker}\,f|\cdot|\mathrm{Im}\,f|$
