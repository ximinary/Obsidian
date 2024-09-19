#fax #math #laag [deo [[Linearna algebra|linearne algebre]]]
$\:$

**Def**. **Sistem linearnih jednačina** u promenljivima $x_{1},\,x_{2},\,\dots,\,x_{n}$ je:
$\begin{cases}a_{11}\,x_{1}+a_{12}\,x_{2}+\dots+a_{1n}\,x_{n}=b_{1}\\a_{21}\,x_{1}+a_{22}\,x_{2}+\dots+a_{2n}\,x_{n}=b_{2}\\\dots\\a_{m1}\,x_{1}+a_{m2}\,x_{2}+\dots+a_{mn}\,x_{n}=b_{m}\end{cases}$

Kraće: $\begin{align}\sum\limits_{j=1}^{n}a_{ij}\,x_{j}=b_{i},\quad \forall i=\overline{1,m}\end{align}$

Matrični oblik: $\boxed{\mathcal{A}\,x=b}$, gde 

$\mathcal{A}=\left(\begin{array}{c}a_{11}&a_{12}&\dots&a_{1n}\\a_{21}&a_{22}&\dots&a_{2n}\\\dots&\dots&\dots&\dots\\a_{m1}&a_{m2}&\dots&a_{mn}\end{array}\right)$ — **matrica sistema**

$x=\left(\begin{array}{}x_{1}\\x_{2}\\\dots\\x_{n}\end{array}\right)\quad\quad b=\left(\begin{array}{}b_{1}\\b_{2}\\\dots\\b_{m}\end{array}\right)$

**Def**. **Proširena matrica sistema**: $\mathcal{A}_{p}=\Big(\ \mathcal{A}\ \,\Big|\ \ b\,\ \Big)= \left(\begin{array}{cccc|c}a_{11}&a_{12}&\dots&a_{1n}&b_{1}\\a_{21}&a_{22}&\dots&a_{2n}&b_{2}\\\dots&\dots&\dots&\dots\dots\\a_{m1}&a_{m2}&\dots&a_{mn}&b_{m}\end{array}\right)$

Rešenje sistema je **svaka** uređena $n$-torka $(c_{1},\,c_{1},\,\dots,\,c_{n})$, takva da zamenom $x_{i}:=c_{i},\ \ \forall i=\overline{1,n}$ važi svaka jednačina u sistemu.

Kada je $m=n$ i $\mathcal{A}$ je invertibilna rešenje je $x=\mathcal{A}^{-1}\,b$
___
Prelazak na [[Linearni operator|LO]]:

$U$ i $V$ su [[Vektorski prostor|VP]] nad $\mathbb{F}$,
$e=\{ e_{1},\,e_{2},\,\dots,\,e_{n} \}$ je baza $U$,
$f=\{ f_{1},\,f_{2},\,\dots,\,f_{m} \}$ je baza $V$.
Tada $\exists A\in\mathrm{Hom}(U,\,V)$, takav da $\varphi_{e,\,f}(A)=\mathcal{A}$.

Rešavanje sistema se svodi na određivanje $u\in U\ \ :\ \ \kappa_{f}\Big(A(u)\Big)=b$, tada $x= \kappa_{e}(u)$ za svako pronađeno $u$.

**Teorema** (Kroneker-Kapelijva) uslovi gore.
Sledeći iskazi su ekvivalentni:
- sistem ima rešenja
- $\exists v\in \mathrm{Im}\,A\ \ :\ \ \kappa_{f}(v)=b$
- $\mathrm{rang}\,\mathcal{A}=\mathrm{rang}\,\mathcal{A}_{p}$

Posledica. Ako $\mathrm{rang}\,\mathcal{A}=n$ (tj. $V=\mathrm{Im}\,A$), sistem ima rešenja.
___
**Def**. Sistem je **Kramerov** ako $m=n=\mathrm{rang}\,\mathcal{A}.$

**Teorema**. Kramerov sistem uvek ima jedinstveno rešenje: $\begin{align}x_{i}=\frac{\Delta_{i}}{\Delta}\end{align},\ \ \forall i=\overline{1,n}$

gde je $\Delta =\det\mathcal{A},\quad\Delta_{i}=\det[a_{1},\,a_{2},\,\dots,\,a_{i-1},\,b,\,a_{i+1},\,\dots,\,a_{n}], \ \ \forall i = \overline{1,n}$
___
Homogeni sistem $\mathcal{A}\,x=\mathbf{0}$, $\ \:$ $\mathrm{rang}\,\mathcal{A}=r$:
- Skup rešenja je jezgro LO $A$:
  Ako je $v=(v_{1},\,v_{2},\,\dots,\,v_{n-r})$ baza $\mathrm{Ker}\, A$, tada je svako rešenje sistema oblika $x= \kappa_{e}\Big(\sum\limits_{i=1}^{n-r}\lambda_{i}\,v_{i}\Big),\ \ \lambda_{i}\in\mathbb{F}$
- Ima bar jedno rešenje $x=\mathbf{0}$ — trivijalno rešenje.
- $m<n\quad\Rightarrow\quad \exists$ netrivijalno rešenje
___
Nehomogeni sistem $\mathcal{A}\,x=b,\ \ b\ne\mathbf{0}$:
Svakom nehomogenom sistemu pridružen je homogeni:  $\mathcal{A}\,x=\mathbf{0}$.

Teorema. Ako $\mathrm{rang}\,\mathcal{A}=\mathrm{rang}\,\mathcal{A}_{p} = r$ onda svako rešenje sistema $\mathcal{A}\,x=b$ je oblika: $\begin{align}x=\kappa_{e}\Big(v_{0}+\sum\limits_{i=1}^{n-r}\lambda_{i}\,v_{i}\Big)\end{align}$, 

gde je  $v=(v_{1},\,v_{2},\,\dots,\,v_{n-r})$ baza $\mathrm{Ker}\, A$, 
i $\kappa_{e}(v_{0})$ je neko rešenje $\bigg($tj. $\kappa_{f}\Big(A(v_{0})\Big)=b\bigg)$ 
___
### Gausova metoda rešavanja sistema
Napomena: [[Rang matrice. Elementarne transformacije#Elementarne transformacije|elementarne transformacije]]

$\Big(\ \mathcal{A}\ \,\Big|\ \ b\,\ \Big)\overset{\text{elementarne transformacije}}{\overset{\text{nad vrstama}}{\sim}}\left(\begin{array}{c c | c}\mathbb{I}_{r}&\mathcal{C}&b'\\\mathcal{O}&\mathcal{O}&b''\end{array}\right)$

Ako $b''\ne\mathbf{0}$, sistem nema rešenja.

Ako $b''=\mathbf{0}$, sistem ima rešenja.
$b'=\left(\begin{array}{}b'_{1}\\b'_{2}\\\dots\\b'_{r}\end{array}\right)$, $\quad\quad$ $\mathcal{C}=\left(\begin{array}{c}c_{11}&c_{12}&\dots&c_{1(n-r)}\\c_{21}&c_{22}&\dots&c_{2(n-r)}\\\dots&\dots&\dots&\dots\\c_{r1}&c_{r2}&\dots&c_{r(n-r)}\end{array}\right)$

Rešenja su:
$\begin{cases}x_{1}=b'_{1}-(c_{11}\,t_{1}+c_{12}\,t_{2}+\dots+c_{1(n-r)}\,t_{n-r})\\ x_{2}=b'_{2}-(c_{21}\,t_{1}+c_{22}\,t_{2}+\dots+c_{2(n-r)}\,t_{n-r})\\ \dots\\x_{r}=b'_{r}-(c_{r1}\,t_{1}+c_{r2}\,t_{2}+\dots+c_{r(n-r)}\,t_{n-r})\\ x_{r+1}=t_{1}\\ x_{r+2}=t_{2}\\ \dots \\ x_{n}=t_{n-r}\end{cases}$

$t_{1},\,t_{2},\,\dots,\,t_{n-r}\in\mathbb{F}$ su slobodni parametri.
Dimenzija skupa rešenja je $n-r$.

$x = \left(\begin{array}{}b'_{1}\\b'_{2}\\\dots\\b'_{r}\\0\\0\\\dots\\0\end{array}\right)+t_{1}\left(\begin{array}{}-c'_{11}\\-c'_{21}\\\dots\\-c'_{r1}\\1\\0\\\dots\\0\end{array}\right)+t_{2}\left(\begin{array}{}-c'_{12}\\-c'_{22}\\\dots\\-c'_{r2}\\0\\1\\\dots\\0\end{array}\right)+\dots+t_{n-r}\left(\begin{array}{}-c'_{1(n-r)}\\-c'_{2(n-r)}\\\dots\\-c'_{r(n-r)}\\0\\0\\\dots\\1\end{array}\right)\,=$
$=w_{0}+t_{1}\,w_{1}+t_{2}\,w_{2}+\dots+t_{n-r}\,w_{n-r}=w_{0}+\sum\limits_{i=1}^{n-r}t_{i}\,w_{i}$

$w_{0}$ je partikularno rešenje
$w_{1},\,w_{2},\,\dots,\,w_{n-1}$ su rešenja homogenog sistema 