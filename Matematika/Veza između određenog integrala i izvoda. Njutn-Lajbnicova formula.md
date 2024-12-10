#fax #math #a2 [deo poglavlja [[Određeni integral|"određeni integral"]]]
$\:$

Oznake za sledeće teoreme:
$f\,\mathcal{R}\,[a,\,b]$;$\quad$ $\varphi:[a,\,b]\to\mathbb{R}$ def. sa $\begin{align}\varphi(x)=\int_{a}^{x} f(t) \, dt \end{align}$

**Teorema**. $\varphi\,\mathcal{C}\,[a,\,b]$.
> Dokaz: Neka je $\ \:$ $\begin{align}M=\sup_{x\in[a,\,b]}|f(x)|>0\end{align}$
> $x_{0}\in[a,\,b]$ — proizvoljno. Treba dokazati $f\,\mathcal{C}\,x_{0}$, tj.
> $\forall \varepsilon>0\quad\exists\delta>0\quad\forall x\in[a,\,b]\cap (x_{0}-\delta,\,x_{0}+\delta)\quad|\varphi(x)-\varphi(x_{0})|<\varepsilon$
> 
> Za proizvoljno $\varepsilon>0$ naći $\delta>0$.
> 
> $\begin{align}|\varphi(x)-\varphi(x_{0})|<\left|\int_{a}^{x} f(t) \, dt-\int_{a}^{x_{0}} f(t) \, dt\right|=\end{align}$
> $\begin{align}=\left|\int_{x_{0}}^{x} f(t) \, dt\right|\leqslant\left|\int_{x_{0}}^{x} \big|f(t)\big| \, dt\right|\leqslant M\cdot|x-x_{0}|<\varepsilon\end{align}$
> 
> $\begin{align}|x-x_{0}|<\frac{\varepsilon}{M}=:\delta\end{align}$

$\:$
Teorema. $f\,\mathcal{C}\,[a,\,b]\quad\Rightarrow\quad \varphi\,\mathcal{C}^{1}\,[a,\,b]$, i važi
$\forall x\in(a,\,b)\quad\varphi'(x)=f(x)$; $\quad$ $\varphi'_{+}(a)=f(a)$; $\quad$ $\varphi'_{-}(b)=f(b)$ ^634405
> Dokaz:
> $x\in[a,\,b]$ proizvoljno
> $h\in[a-x,\,b-x]$ da važi $x+h\in[a,\,b]$
> 
> $\begin{align}\lim\limits_{ h \to 0 }\frac{\varphi(x+h)-\varphi(x)}{h}=\lim\limits_{ h \to 0 }\frac{\int_{a}^{x+h} f(t) \, dt-\int_{a}^{x} f(t) \, dt}{h}=\lim\limits_{ h \to 0 }\frac{\int_{x}^{x+h} f(t) \, dt}{h}=\end{align}$
> > Iz [[Riman-integrabilnost funkcija i svojstva određenog integrala#^88105f|stava]] i zbog toga što važi $f\,\mathcal{C}\,[a,\,b]$ dobijamo:
> > Postoji $c$ između ili jednako $x$ i $x+h$  takvo da $\begin{align}\int_{x}^{x+h} f(t) \, dt= f(c)\cdot(x+h-x)=f(c)\cdot h\end{align}$
> 
> $\begin{align}=\lim\limits_{ h \to 0 }\frac{f(c)\cdot h}{h}=\lim\limits_{ h \to 0 }f(c)\xlongequal{h\to0\ \Rightarrow\ c\to x}f(x)\end{align}$
> 
> Kad $x=a$, $h\in[0,\,b-a]$. Imamo desni limes i $\varphi'_{+}(a)=f(a)$;
> Kad $x=b$, $h\in[a-b,\,0]$. Imamo levi limes i $\varphi'_{-}(b)=f(b)$;
> Kad $x\in(a,\,b)$, dobijamo $\varphi'(x)=f(x)$
> 
> Jer $\varphi'(x)=f(x)$ i $f\,\mathcal{C}\,[a,\,b]$, dobija se da $\varphi'\,\mathcal{C}\,[a,\,b]$ tj. $\varphi\,\mathcal{C}^{1}\,[a,\,b]$

$\:$

**Posledica**. Teorema. $f\,\mathcal{C}\,(a,\,b)\quad\Rightarrow\quad \exists F:\ (a,\,b)\to\mathbb{R}$ $\ \:$ — [[Neodređeni integral#Primitivna funkcija|primitivna]] za $f$ na $[a,\,b]$
> Dokaz: 
> $x_{0}\in(a,\,b)$ $\ \:$ proizvoljno.
> $F:\ (a,\,b)\to\mathbb{R}$ def. sa $\begin{align}F(x)=\int_{x_{0}}^{x} f(t) \, dt \end{align}$
> $F$ je korektno definisana jer $f\,\mathcal{C}\,[a,\,b]\quad\Rightarrow\quad f\,\mathcal{R}\,[a,\,b]$ 
>___
>$x\in(a,\,b)$ proizvoljno
> $h\in(a-x,\,b-x)$ da važi $x+h\in(a,\,b)$
> 
> $\begin{align}\lim\limits_{ h \to 0 }\frac{F(x+h)-F(x)}{h}=\lim\limits_{ h \to 0 }\frac{\int_{x_{0}}^{x+h} f(t) \, dt-\int_{x_{0}}^{x} f(t) \, dt}{h}=\lim\limits_{ h \to 0 }\frac{\int_{x}^{x+h} f(t) \, dt}{h}=\end{align}$
> 
> $\begin{align}\xlongequal{\text{kao i u prethodnoj teoremi}}f(x)\end{align}$
> 
> Dakle, $\forall x\in(a,\,b)\quad F'(x)=f(x)$. 
> Tj. $F$ je primitivna za $f$ na $[a,\,b]$

$\:$
**Teorema** (Njutn-Lajbnicova formula). Neka je $f\,\mathcal{C}\,[a,\,b]$ i neka je $F:[a,\,b]$ neka primitivna za $f$ na $[a,\,b]$. Tada $\begin{align}\int_{a}^{b} f(x) \, dx =F(b) - F(a)\end{align}$ ^08f509
> 
> $F$ je primitivna za $f$ na $[a,\,b]\quad\Leftrightarrow$
> - $\forall x\in(a,\,b)\quad F'(x)=f(x)$
> - $F'_{+}(a)=f(a)$
> - $F'_{-}(b)=f(b)$

> Dokaz:
> Iz [[Veza između određenog integrala i izvoda. Njutn-Lajbnicova formula#^634405|teoreme]] $\exists\varphi:\ [a,\,b]\to\mathbb{R}$ $\ \:$ — primitivna za $f$ na $[a,\,b]$
> $F$ i $\varphi$ su primitivne $\quad\Rightarrow$
> $\forall x\in[a,\,b] \quad\varphi(x)=F(x)+C,\quad C\in\mathbb{R}$
> 
> $\varphi(a)=0\quad\Rightarrow\quad C =- F(a)$
> $\begin{align}\varphi(b)=\int_{a}^{b} f(x) \, dx \quad \Rightarrow\quad\int_{a}^{b} f(x) \, dx =F(b)+C=F(b)-F(a)\end{align}$