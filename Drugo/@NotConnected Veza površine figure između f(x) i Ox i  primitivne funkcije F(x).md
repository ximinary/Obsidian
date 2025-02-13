Neka je $f:(c,\,d)\to[0,\,+\infty)$ neprekidna funkcija. $[a,\,b]\subset(c,\,d)$.
$\Phi = \big\{ (x,\,y)\in\mathbb{R}^{2}\ \big|\ a\leqslant x\leqslant b,\ \ 0\leqslant y \leqslant f(x) \big\}$ — figura ograničena sa $f(x)$ i $\mathrm{O}x$ na intervalu $[a,\,b]$.
$P(\Phi)$ — površina figure.

$t\in[a,\,b]$
$A(t)=\big\{ (x,\,y)\in\mathbb{R}^{2}\ \big|\ a\leqslant x\leqslant t,\ \ 0\leqslant y \leqslant f(x) \big\}$ — figura na intervalu $[a,\,t]$, deo figure $\Phi$.
$P(t)$ — površina figure $A(t)$.

$P: (a,\,b)\to[0,\,+\infty)$ $\quad\quad$ $P(a)=0$ $\quad\quad$ $P(b)=P(\Phi)$

$\:$
$\forall t\in[a,\,b)\quad\exists h>0\quad (t+h)\in[a,\,b)$

$\begin{align}M = \max_{t\,<\,x\,<\,t+h} f(x).\quad \exists 0\leqslant\theta_{1}\leqslant1\ \ : \ \ M=f(t+\theta_{1}h)\end{align}$
$\begin{align}m = \min_{t\,<\,x\,<\,t+h} f(x).\quad \exists 0\leqslant\theta_{2}\leqslant1\ \ : \ \ m=f(t+\theta_{2}h)\end{align}$

Površina figure na intervalu $[t,\,t+h]$ je $P(t+h)-P(t)$. I važi:

$m\,h\leqslant P(t+h)-P(t) \leqslant M\,h\quad\big|:h$

$\begin{align}f(t+\theta_{2}h)\leqslant \frac{P(t+h)-P(t)}{h} \leqslant f(t+\theta_{1}h)\end{align}\quad\big|\,h\to0$

$f(t)\leqslant P'(t)\leqslant f(t)$

Dakle, $\forall t\in[a,\,b)\quad P'(t)=f(t)$,
tj $P$ je primitivna za $f$ na $(a,\,b)$

Neka je $F:(c,\,d)\to\mathbb{R}$ proizvoljna primitivna za $f$ na $(c,\,d)\supset[a,\,b]$,
tada $\forall t \in [a,\,b)\quad P(t)=F(t)+C,\quad C\in\mathbb{R}$

$P(a)= 0\quad \Rightarrow\quad C=- F(a)\quad \Rightarrow\quad P(t)=F(t)-F(a)$

Konačno, površina figure ograničene sa $f(x)$ i $\mathrm{O}x$ na intervalu $[a,\,b]\subset(c,\,d)$ je $F(b)-F(a)$, gde je $F$ proizvoljna primitivna za $f$ na $(c,\,d)$