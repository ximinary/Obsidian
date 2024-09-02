#fax #math #a1 [deo poglavlja [[Niz brojeva|"niz brojeva"]]]
$\:$
**Def**. Niz $(a_{n})$ je Košijev ako $\forall\varepsilon>0\quad N\in\mathbb{N}\quad \forall m,\,n\geqslant N\quad\left|a_{m}-a_{n}\right|<\varepsilon$

[[analiza1_3_9.png|Stav 1]]. Košijev niz $(a_{n})$ je ograničen

[[analiza1_3_10.png|Stav 2]]. Košijev niz $(a_{n})$ koji ima [[Podnizovi|tačku nagomilavanja]] konvergira.
$\:$

Teorema. $(a_{n})$ je niz <u>realnih</u> brojeva. Tada:
$(a_{n})$ [[Limes niza|konvergira]] $\quad\Leftrightarrow \quad$ $(a_{n})$ je Košijev
>Dokaz:
>$\boxed\Rightarrow$
$\exists\lim\limits_{ n \to \infty }a_{n}=a\in\mathbb{R}\quad\Leftrightarrow\quad\forall \varepsilon>0\quad\exists N\quad\forall n\geqslant N\quad\left|a_{n}-a\right|<\frac{\varepsilon}{2}\quad\Rightarrow$
$\Rightarrow\quad\forall\varepsilon>0\quad\exists N\quad\forall m,\,n\geqslant N\quad \left|a_{n}-a_{m}\right|\leqslant\left|a_{n}-a\right|+\left|a_{m}-a\right|<\frac{\varepsilon}{2}+\frac{\varepsilon}{2}=\varepsilon$
>
>$\boxed\Leftarrow$ $\ \:$ $(a_{n})$ je Košijev $\ \overset{\text{Stav\ 1}}\Longrightarrow\ (a_{n})$ je ograničen $\overset{\text{Bolcano-Vajerštrasova}}{\overset{\text{teorema (*)}}\Longrightarrow}$
>$\Rightarrow \ \ \exists a$ — tačka nagomilavanja $\ \overset{\text{Stav\ 2}}\Longrightarrow\ (a_{n})\:$ konvergira
>
>([[Podnizovi#^dd96ed|*]])