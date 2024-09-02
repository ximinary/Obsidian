#fax #math #a1 [deo poglavlja [[Izvod|"izvod"]]]
$\:$

**Def**. $f$ je diferencijabilna $n$ puta. Tejlorov polinom funkcije $f$ u $\mathrm{O}(x_{0})$ stepena $n$ je $\begin{align}P_{n}(x,\,x_{0};\,f):=f(x_{0})+f'(x_{0})(x-x_{0})+\frac{f''(x_{0})}{2!}(x-x_{0})^{2}+\dots+\frac{f^{(n)}(x_{0})}{n!}(x-x_{0})^{n}=\end{align}$
$\quad\quad\quad\quad\quad\ \ \ \,\begin{align}=\sum\limits_{k=0}^{n}\frac{f^{(k)}(x_{0})}{k!}(x-x_{0})^{k}\end{align}$

**Def**. Maklarenov polinom je Tejlorov polinom u $x_{0}=0$ $\begin{align}P_{n}(x,0;\,f):=f(0)+f'(0)\,x+\frac{f''(0)}{2!}\,x^{2}+\dots+\frac{f^{(n)}(0)}{n!}\,x^{n}=\end{align}$
$\quad\quad\quad\quad\quad\ \begin{align}=\sum\limits_{k=0}^{n}\frac{f^{(k)}(0)}{k!}\,x^{k}\end{align}$

> Idea: aproksimacija nepolinomne funkcije polinomnoj.

[[analiza1_2_8.png|Stav]]. $P(x)=P_{n}(x,\,x_{0};\,f)$ — Tejlorov polinom funkcije $f$ u $\mathrm{O}(x_{0})$ stepena $n$. Tada $\forall k=\overline{0,\,n}\quad P^{(k)}(x_{0})=f^{(k)}(x_{0})$

### [[analiza1_2_Tejlor.png|Maklarenov polinom osnovnih funkcija]] ([[analiza1_2_izvodiVisegReda.png|*]])

### Ostatak Tejlorovog polinoma
**Def**. Ostatak Tejlorovog polinoma funkcije $f$ u $\mathrm{O}(x_{0})$ stepena $n$ je $\begin{align}R_{n}(x,\,x_{0};\,f):=f(x)-P_{n}(x,\,x_{0};\,f)\end{align}$

[[analiza1_2_peanovOblikOst.png|Teorema]] (Peanov oblik ostatka). $f\,\mathcal{C}^{n}\,\mathrm{O}(x_{0})\ \ \Rightarrow\ \ R_{n}(x,\,x_{0};\,f)=o\big((x-x_{0})^{n}\big),\ \ x\to x_{0}$

> Posledica:
> - $\begin{align}e^{x}=\sum\limits_{k=0}^{n}\frac{x^{k}}{k!}+o(x^{n}),\ \ x\to 0\end{align}$
> - $\begin{align}\ln(1+x)=\sum\limits_{k=1}^{n}(-1)^{k}\frac{x^{k}}{k}+o(x^{n}),\ \ x\to 0\end{align}$
> - $\begin{align}(1+x)^{\alpha}=\sum\limits_{k=1}^{n}\binom{\alpha}{k}x^{k}+o(x^{n}),\ \ x\to 0\end{align}$
> - $\begin{align}\sin x= x-\frac{x^{3}}{3!}+\frac{x^{5}}{5!}+\dots+(-1)^{k}\,\frac{x^{2k+1}}{(2k+1)!}+o(x^{2k+2}),\ \ x\to 0\end{align}$
> - $\begin{align}\cos x= 1-\frac{x^{2}}{2!}+\frac{x^{4}}{4!}+\dots+(-1)^{k}\,\frac{x^{2k}}{(2k)!}+o(x^{2k+1}),\ \ x\to 0\end{align}$

[[analiza1_2_lagranževOblikOst.png|Teorema]] (Lagranžev oblik ostatka). $\begin{align}f\,\mathcal{C}^{n+1}\,\mathrm{O}(x_{0})\ \ \Rightarrow\ \ R_{n}(x,\,x_{0};\,f)=\frac{f^{n+1}(\xi)}{(n-1)!}(x-x_{0})^{n+1}\end{align}$ 
za neko $\xi$ između $x$ i $x_{0}$
---
[[Asimptota]]