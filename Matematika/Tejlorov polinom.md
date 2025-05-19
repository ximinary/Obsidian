#fax #math #a1 [deo poglavlja [[Izvod|"izvod"]]]
$\:$

**Def**. $A\subseteq \mathbb{R}$, $\ \:$ $f:\ A\to\mathbb{R}$ je $n$ puta diferencijabilna funkcija. Tejlorov polinom funkcije $f$ u $\mathrm{O}(x_{0})$ stepena $n$ je $\begin{align}P_{n}(x,\,x_{0};\,f):=f(x_{0})+f'(x_{0})(x-x_{0})+\frac{f''(x_{0})}{2!}(x-x_{0})^{2}+\dots+\frac{f^{(n)}(x_{0})}{n!}(x-x_{0})^{n}=\end{align}$
$\quad\quad\quad\quad\quad\ \ \ \,\begin{align}=\sum\limits_{k=0}^{n}\frac{f^{(k)}(x_{0})}{k!}(x-x_{0})^{k}\end{align}$

**Def**. Maklorenov polinom je Tejlorov polinom u $x_{0}=0$ $\begin{align}P_{n}(x,0;\,f):=f(0)+f'(0)\,x+\frac{f''(0)}{2!}\,x^{2}+\dots+\frac{f^{(n)}(0)}{n!}\,x^{n}=\end{align}$
$\quad\quad\quad\quad\quad\ \begin{align}=\sum\limits_{k=0}^{n}\frac{f^{(k)}(0)}{k!}\,x^{k}\end{align}$

> Idea: aproksimacija nepolinomne funkcije polinomnoj.

[[analiza1_2_8.png|Stav]]. $P(x)=P_{n}(x,\,x_{0};\,f)$ — Tejlorov polinom funkcije $f$ u $\mathrm{O}(x_{0})$ stepena $n$. Tada $\forall k=\overline{0,\,n}\quad P^{(k)}(x_{0})=f^{(k)}(x_{0})$

### [[analiza1_2_Tejlor.png|Maklorenov polinom osnovnih funkcija]] ([[analiza1_2_izvodiVisegReda.png|*]])

### Ostatak Tejlorovog polinoma
**Def**. Ostatak Tejlorovog polinoma funkcije $f$ u $\mathrm{O}(x_{0})$ stepena $n$ je $\begin{align}R_{n}(x,\,x_{0};\,f):=f(x)-P_{n}(x,\,x_{0};\,f)\end{align}$

[[analiza1_2_peanovOblikOst.png|Teorema]] (Peanov oblik ostatka). $f\,\mathcal{C}^{n}\,\mathrm{O}(x_{0})\ \ \Rightarrow\ \ R_{n}(x,\,x_{0};\,f)=o\big((x-x_{0})^{n}\big),\ \ x\to x_{0}$

> Posledica:
> - $\begin{align}e^{x}=\sum\limits_{k=0}^{n}\frac{x^{k}}{k!}+o(x^{n}),\ \ x\to 0\end{align}$
> - $\begin{align}\ln(1+x)=\sum\limits_{k=1}^{n}(-1)^{k-1}\frac{x^{k}}{k}+o(x^{n}),\ \ x\to 0\end{align}$
> - $\begin{align}(1+x)^{\alpha}=\sum\limits_{k=0}^{n}\binom{\alpha}{k}x^{k}+o(x^{n}),\ \ x\to 0\end{align}$
> - $\begin{align}\sin x= x-\frac{x^{3}}{3!}+\frac{x^{5}}{5!}+\dots+(-1)^{k}\,\frac{x^{2k+1}}{(2k+1)!}+o(x^{2k+2}),\ \ x\to 0\end{align}$
> - $\begin{align}\cos x= 1-\frac{x^{2}}{2!}+\frac{x^{4}}{4!}+\dots+(-1)^{k}\,\frac{x^{2k}}{(2k)!}+o(x^{2k+1}),\ \ x\to 0\end{align}$

[[analiza1_2_lagranževOblikOst.png|Teorema]] (Lagranžev oblik ostatka). $\begin{align}f\,\mathcal{C}^{n+1}\,\mathrm{O}(x_{0})\ \ \Rightarrow\ \ R_{n}(x,\,x_{0};\,f)=\frac{f^{(n+1)}(\xi)}{(n+1)!}(x-x_{0})^{n+1}\end{align}$ 
za neko $\xi$ između $x$ i $x_{0}$ ^ddcb73
---
[[Asimptota]]

### Tejlorov polinom funkcije više promenljivih

**Def**. $A\subseteq \mathbb{R}^{n}$, $\ \:$ $f:\ A\to\mathbb{R}$ ima sve parcijalne izvode do reda $k$, koje su neprekidni. Tejlorov polinom funkcije $f$ u $\mathrm{O}(\mathbf{x}^{0})$ stepena $k$ je  $\begin{align}&P_{k}(\mathbf{x},\,\mathbf{x}_{0};\,f):=f(\mathbf{x}_{0})+\Bigg(\frac{\partial f}{\partial x_{1}}(\mathbf{x}^{0})(x_{1}-x_{1}^{0})+\frac{\partial f}{\partial x_{2}}(\mathbf{x}^{0})(x_{2}-x_{2}^{0})+\dots+\frac{\partial f}{\partial x_{n}}(\mathbf{x}^{0})(x_{n}-x_{n}^{0})\Bigg)+\\&+\frac{1}{2!}\Bigg(\frac{\partial^{2} f}{\partial x_{1}\!^{2}}(\mathbf{x}^{0})(x_{1}-x_{1}^{0})^{2}+\frac{\partial^{2} f}{\partial x_{2}\!^{2}}(\mathbf{x}^{0})(x_{2}-x_{2}^{0})^{2}+\dots+\frac{\partial^{2} f}{\partial x_{n}\!^{2}}(\mathbf{x}^{0})(x_{n}-x_{n}^{0})^{2}+\ \\&\quad\quad\quad\ +2\frac{\partial^{2} f}{\partial x_{1}\,\partial x_{2}}(\mathbf{x}^{0})(x_{1}-x_{1}^{0})(x_{2}-x_{2}^{0})+2\frac{\partial^{2} f}{\partial x_{1}\,\partial x_{3}}(\mathbf{x}^{0})(x_{1}-x_{1}^{0})(x_{3}-x_{3}^{0})+\dots+2\frac{\partial^{2} f}{\partial x_{n-1}\,\partial x_{n}}(\mathbf{x}^{0})(x_{n-1}-x_{n-1}^{0})(x_{n}-x_{n}^{0})\Bigg)+\\&+\dots+\frac{1}{k!}\underset{\alpha_{1}+\alpha_{2}+\dots+\alpha_{n}=k}{\underset{\alpha_{i}\in\mathbb{N}_{0},\ \ \forall i=\overline{1,n}}{\sum}}\Bigg(\binom{k}{\alpha_{1},\,\alpha_{2},\,\dots,\,\alpha_{n}}\frac{\partial^{k}f}{\partial x_{1}\!^{\alpha_{1}}\,\partial x_{2}\!^{\alpha_{2}}\cdots\partial x_{n}\!^{\alpha_{n}}}(\mathbf{x}^{0})(x_{1}-x_{1}^{0})^{\alpha_{1}}(x_{2}-x_{2}^{0})^{\alpha_{2}}\cdots(x_{n}-x_{n}^{0})^{\alpha_{n}}\Bigg)=\end{align}$

$\begin{align}=f(\mathbf{x}_{0})+\sum\limits_{i=1}^{k}\frac{1}{i!}\Bigg(\frac{\partial f}{\partial x_{1}}(\mathbf{x}^{0})(x_{1}-x_{1}^{0})+\frac{\partial f}{\partial x_{2}}(\mathbf{x}^{0})(x_{2}-x_{2}^{0})+\dots+\frac{\partial f}{\partial x_{n}}(\mathbf{x}^{0})(x_{n}-x_{n}^{0})\Bigg)^{i}=\end{align}$

$\begin{align}=\boxed{\sum\limits_{i=0}^{k}\frac{\Big((\mathbf{x}-\mathbf{x}^{0})\cdot\nabla\Big)^{i}f(\mathbf{x}^{0})}{i!}}\end{align}$
$\:$
**Def**. Ostatak Tejlorovog polinoma funkcije $f$ u $\mathrm{O}(\mathbf{x}_{0})$ stepena $k$ je $\begin{align}R_{k}(\mathbf{x},\,\mathbf{x}_{0};\,f):=f(\mathbf{x})-P_{k}(\mathbf{x},\,\mathbf{x}_{0};\,f)\end{align}$

**Teorema** (Peanov oblik ostatka). $f:\ \mathbb{R}^{n}\to\mathbb{R}$ ima sve parcijalne izvode do reda $k+1$, koje su neprekidne. Tada $R_{k}(\mathbf{x},\,\mathbf{x}_{0};\,f)=o\big(||\mathbf{x}-\mathbf{x}_{0}||^{k}\big),\ \ \mathbf{x}\to \mathbf{x}_{0}$

> Dokaz: 
> Neka je $\mathbf{h}=\mathbf{x}-\mathbf{x}^{0}$ i neka je $\varphi:\ [0,\,1]\to\mathbb{R}$ takva da $\varphi(t)=f(\underbrace{\mathbf{x}^{0}+\mathbf{h}\,t}_{g(t)})$
> 
> Nađemo Tejlorov polinom stepena $k$ funkcije $\varphi$ u $t=0$ i njegov Lagranžev ostatak:
> $\begin{align}\varphi(t)=\varphi(0)+\varphi'(0)\,t+\frac{\varphi''(0)}{2!}\,t^{2}+\dots+\frac{\varphi^{(k)}(0)}{k!}\,t^{k}+\frac{\varphi^{(k+1)}(\xi)}{(k+1)!}t^{k+1}\end{align}$, 
> za neko $\xi$ između $0$ i $t$.
> 
> $\begin{align}\varphi'(t)&=(f\circ g)'(t)=df(\mathbf{x}^{0}+\mathbf{h}\,t)\,dg(t)=df(\mathbf{x}^{0}+\mathbf{h}\,t)\,\mathbf{h}=\nabla\!f(\mathbf{x}^{0}+\mathbf{h}\,t)\cdot\mathbf{h}=\\&=\frac{\partial f}{\partial x_{1}}(\mathbf{x}^{0}+\mathbf{h}\,t)\,h_{1}+\frac{\partial f}{\partial x_{2}}(\mathbf{x}^{0}+\mathbf{h}\,t)\,h_{2}+\dots+\frac{\partial f}{\partial x_{n}}(\mathbf{x}^{0}+\mathbf{h}\,t)\,h_{n}\begin{array}{}\ \\ \ \\\ \end{array}\end{align}$
>
> odakle indukcijom se dobija:
> $\begin{align}\forall i=\overline{1,k\!+\!1}\quad\varphi^{(i)}(t)=\Big(\nabla\!f(\mathbf{x}^{0}+\mathbf{h}\,t)\cdot\mathbf{h}\Big)^{i}\end{align}$
> 
> $\begin{align}f(\mathbf{x})=\varphi(1)&=\varphi(0)+\varphi'(0)+\frac{\varphi''(0)}{2!}+\dots+\frac{\varphi^{(k)}(0)}{k!}+\frac{\varphi^{(k+1)}(\xi)}{(k+1)!}=\\&=\sum\limits_{i=1}^{k}\frac{1}{i!}\Big(\nabla\!f(\mathbf{x}^{0}+\mathbf{h}\,t)\cdot\mathbf{h}\Big)^{i}+\underbrace{\frac{1}{(k+1)!}\Big(\nabla\!f(\mathbf{x}^{0}+\mathbf{h}\,\xi)\cdot\mathbf{h}\Big)^{k+1}}_{=R_{k}(\mathbf{x},\ \mathbf{x}^{0};\ f),\quad\xi\in(0,\,1)}\end{align}$
> 
> Da li $R_{k}(\mathbf{x},\,\mathbf{x}_{0};\,f)=o\big(||\mathbf{x}-\mathbf{x}_{0}||^{k}\big),\ \ \mathbf{x}\to \mathbf{x}_{0}$ ?
> Tj. treba pokazati da sledeći limes jednak $0$:
> 
> $\begin{align}\lim\limits_{ \mathbf{h} \to 0 }\frac{\Big(\nabla\!f(\mathbf{x}^{0}+\mathbf{h}\,\xi)\cdot\mathbf{h}\Big)^{k+1}}{||h||^{k}}=\lim\limits_{ \mathbf{h} \to 0 }\frac{\underset{\alpha_{1}+\alpha_{2}+\dots+\alpha_{n}=k}{\underset{\alpha_{i}\in\mathbb{N}_{0},\ \ \forall i=\overline{1,n}}{\sum}}\Bigg(\binom{k}{\alpha_{1},\,\alpha_{2},\,\dots,\,\alpha_{n}}\frac{\partial^{k+1}f}{\partial x_{1}\!^{\alpha_{1}}\,\partial x_{2}\!^{\alpha_{2}}\cdots\partial x_{n}\!^{\alpha_{n}}}(\mathbf{x}^{0}+\mathbf{h}\xi)\,h_{1}^{\alpha_{1}}\,h_{2}^{\alpha_{2}}\cdots h_{n}^{\alpha_{n}}\Bigg)}{||h||^{k}}\end{align}$
>
> >$\begin{align}\left|\frac{h_{i_{1}}h_{i_{2}}\cdots h_{i_{k+1}}}{||\mathbf{h}||^{k}}\right|\leqslant\left|\frac{||\mathbf{h}||^{k+1}}{||\mathbf{h}||^{k}}\right|=||\mathbf{h}||\to0,\quad\mathbf{h}\to\mathbf{0}\end{align}$
> >
> > Iz neprekidnosti parcijalnih izvoda:
> > $\begin{align}\frac{\partial^{k+1}f}{\partial x_{1}\!^{\alpha_{1}}\,\partial x_{2}\!^{\alpha_{2}}\cdots\partial x_{n}\!^{\alpha_{n}}}(\mathbf{x}^{0}+\mathbf{h}\xi)\to\frac{\partial^{k+1}f}{\partial x_{1}\!^{\alpha_{1}}\,\partial x_{2}\!^{\alpha_{2}}\cdots\partial x_{n}\!^{\alpha_{n}}}(\mathbf{x}^{0}),\quad\mathbf{h}\to\mathbf{0}\end{align}$