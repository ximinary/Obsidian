#fax #math #ds1 [deo [[Funkcija|poglavlja "funkcija"]]]
$\:$

Teorema. Ako su $f \subseteq A \times B\:$ i $\:g \subseteq B \times C\:$ [funkcije](Funkcija) tada [kompozicija relacija](Relacija#Kompozicija%20relacija) $g\,\!\circ\!f \subseteq A\times C$ je [funkcija](Funkcija) i važi $\forall x\in A\ \ \ (g\,\!\circ\!f)(x) = g(f(x))$
> Dokaz: pps $g\,\!\circ\!f$ nije funkcija tada važi $\exists a \in A, \ c_1,\ c_2\in C\ \ : \ \ (a,\ c_1), \ (a,\ c_2)\in g\,\!\circ\!f$.
$(a,\ c_1)\in g\,\!\circ\!f\ \ \Rightarrow \ \ \exists b_1\in B\ \ : \ \ (a,\ b_1) \in f\ \ \land \ \ (b_1,\ c_1)\in g$
$(a,\ c_2)\in g\,\!\circ\!f\ \ \Rightarrow \ \ \exists b_2\in B\ \ : \ \ (a,\ b_2) \in f\ \ \land \ \ (b_2,\ c_2)\in g$
$f$ je funkcija, $a\in Dom(f)\ \ \Rightarrow\ \ b_1 = f(a) = b_2$ 
$g$ je funkcija, $b_1=b_2$ $\ \ \Rightarrow\ \ c_1 = c_2$ 
Kontradikcija $\ \ \Rightarrow\ \ g\,\!\circ\!f$ je funkcija

**Def**. Ako su $f:\ \ X \to Y\:$ i $\:g:\ \ Y \to Z\:$  funkcije tada se funkcija $g\,\!\circ\!f:\ \ X \to Z\:$ zove **kompozicija** funkcija $f$ i $g$ i važi $\forall x\in A\ \ \ (g\,\!\circ\!f)(x) = g(f(x))$

[Primer](funkcija%20primer%202.png)

Stav. Ako su $f:\ \ A \to B$ , $\:g:\ \ B \to C\:$ i $\:h:\ \ C \to D\:$ funkcije tada važi $h\,\!\circ\!(g\,\!\circ\!f) = (h\,\!\circ\!g)\,\!\circ\!f$

[Stav](kompozicija%20funkcija%20stav.png). Neka su $f:\ \ A \to B\:$ i $\:g:\ \ B \to C\:$ funkcije tada
1. Ako je $g\,\!\circ\!f$ "1-1" onda je $f$ "1-1"
2. Ako je $g\,\!\circ\!f$ "na" onda je $g$ "na"
3. Ako su $f$ i $g$ "1-1" onda je $g\,\!\circ\!f$ "1-1"
4. Ako su $f$ i $g$ "na" onda je $g\,\!\circ\!f$ "na"

[Primer](kompozicija%20funkcija%20primer.png)