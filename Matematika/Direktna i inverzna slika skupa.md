#fax #math #ds1 [deo [[Funkcija|poglavlja "funkcija"]]] 
$\:$

Neka je $f:\ \ X \to Y$ [funkcija](Funkcija)
**Def**. $A \subseteq X$. **Direktna slika** skupa $A$ je skup $f[A]=\{ f(x)\ | \ x\in A\}$
**Def**. $B \subseteq Y$. **Inverzna slika** skupa $B$ je skup $f^{-1}[B]=\{ x \in X\ | \ f(x)\in B\}$
*($f^{-1}[B]$ je samo oznaka $f$ ne mora da ima [inverz](Inverzna%20funkcija))*

$y \in f[A] \ \ \Leftrightarrow \ \ \exists x\in A \ : \ f(x) =y$
$x \in f^{-1}[B] \ \ \Leftrightarrow \ \ f(x)\in B$

[Primer](direktna%20i%20inverzna%20slika%20primer%201.png)

Stav. Neka je $f:\ \ X \to Y$ [funkcija](Funkcija). $A, \, B\subseteq X;\ \ C,\, D\subseteq Y$. Tada
1. $f[\varnothing] = \varnothing ,\ \ f^{-1}[\varnothing] = \varnothing$
2. $A \subseteq B \ \ \Rightarrow\ \ f[A]\subseteq f[B]$
3. $C \subseteq D \ \ \Rightarrow\ \ f^{-1}[C]\subseteq f^{-1}[D]$

> Dokaz:
> 1. pps $\exists y \in f[\varnothing]\ \ \ \ \exists x\in \varnothing \ : \ f(x) =y \ \:$ — kontradikcija
> 2. $y \in f[A] \ \ \Rightarrow\ \ \exists x\in A \subseteq B \ : \ f(x) = y$
>    $\exists x\in B\ : \ f(x) = y\ \ \Rightarrow\ \ y \in f[B]$
> 3. $x \in f^{-1}[C] \ \ \Rightarrow\ \ f(x) \in C \subseteq D$
>    $f(x) \in D\ \ \Rightarrow\ \ x \in f^{-1}[D]$


Stav. Neka je $f:\ \ X \to Y$ [funkcija](Funkcija). $A, \, B\subseteq X;\ \ C,\, D\subseteq Y$. Tada
1. $A \subseteq f^{-1}[f(A)]$ $\quad\quad\quad\quad\quad$(jednakost ako je $f$ "1-1")
2. $f[f^{-1}(C)] \subseteq C$ $\quad\quad\quad\quad\quad$(jednakost ako je $f$ "na")
3. $f[A\cup B] = f[A] \cup f[B]$ $\ \ \ \ \ \,$([dokaz](direktna%20i%20inverzna%20slika%20primer%202.png))
4. $f[A\cap B] \subseteq f[A] \cap f[B]$ $\ \ \ \ \ \,$(jednakost ako je $f$ "1-1")
5. $f[A\,\setminus\,\!B] \supseteq f[A] \,\setminus\,\! f[B]$ $\ \ \ \ \ \,$(jednakost ako je $f$ "1-1")
6. $f^{-1}[C\cup D] = f^{-1}[C] \cup f^{-1}[D]$
7. $f^{-1}[C\cap D] = f^{-1}[C] \cap f^{-1}[D]$
8. $f^{-1}[C\,\setminus\,\!D] = f^{-1}[C]\,\setminus\,\!f^{-1}[D]$