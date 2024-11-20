#fax #math #a2 [deo [[Analiza|analize]]]


### Veza površine figure između $f(x)$ i $\mathrm{O}x$ i  [[Neodređeni integral#Primitivna funkcija|primitivne funkcije]] $F(x)$

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

### Definicija određenog integrala
$f:\ [a,\,b]\to\mathbb{R}$

**Def**. Neka su $a=x_{0}<x_{1}<\dots<x_{n}=b$. Skup $\mathcal{P}=\Big\{ [x_{i-1},\,x_{i}]\ \Big|\ i=\overline{1,n} \Big\}$ je **podela** intervala $[a,\,b]$.

$x_{0},\,x_{1},\,\dots,\,x_{n}$ su **podeove tačke** podele $\mathcal{P}$.

$\begin{align}\lambda(\mathcal{P})=\max_{i=\overline{1,\,n}}(x_{i}-x_{i-1})\end{align}\ \:$ je **parametar podele** $\mathcal{P}$.

$\mathcal{P}[a,\,b]$ — skup svih podela intervala $[a,\,b]$.

$\mathcal{P},\,\mathcal{P}'\in\mathcal{P}[a,\,b]$. $\ \:$ $\mathcal{P}'$ je **finija** (**grublja**) podela od $\mathcal{P}$ ako je skup podeovih tačaka podele $\mathcal{P}'$ nadskup (podskup) skupa podeovih tačaka podele $\mathcal{P}$.

**Stav**. $\forall\mathcal{P}',\,\mathcal{P}''\in\mathcal{P}[a,\,b]\quad\exists\mathcal{P}\in\mathcal{P}[a,\,b]\ \ :\ \ \mathcal{P}$ je finija i od $\mathcal{P}'$ i od $\mathcal{P}''$
(Skup podeonih tačaka $\mathcal{P}$ je unija podeonih tačaka $\mathcal{P}'$ i $\mathcal{P}''$).
Tada $\mathcal{P}$ je **superpozicija podela** $\mathcal{P}'$ i $\mathcal{P}''$.

$\xi_{i}\in[x_{i-1},\,x_{i}],\quad \forall i=\overline{1,n}$. Tada su
$\xi=(\xi_{1},\,\xi_{2},\,\dots,\,\xi_{n})$ istaknute tačke podele $\mathcal{P}$.

$(\mathcal{P},\,\xi)$ — podela sa istaknutim tačkama intervala $[a,\,b]$

**Def**. Neka je $f:\ [a,\,b]\to\mathbb{R}\ \:$ i $\ \:(\mathcal{P},\,\xi)$ podela sa istaknutim tačkama intervala $[a,\,b]$. Zbir $\begin{align}\sigma(f,\,\mathcal{P},\,\xi)=\sum\limits_{i=1}^{n}(x_{i}-x_{i-1})\,f(\xi_{i})\end{align}$ je **integralna suma**.

---
**Definicija** (pomoću integralnih suma). Neka je $f:\ [a,\,b]\to\mathbb{R}$. $\ \:$ $I\in\mathbb{R}$ je limes integralnih suma $\sigma(f,\,\mathcal{P},\,\xi)$ kad $\lambda(\mathcal{P})\to0$, ako
$\begin{align}\forall\varepsilon>0\quad\exists\delta>0\quad\forall\binom{(\mathcal{P,\,\xi} )\ \text{— podela sa istaknutim tačkama}}{\text{ intervala }[a,\,b]\text{ takva da } \mathcal{P}(\lambda)<\delta}\quad \Big|I-\sigma(f,\,\mathcal{P},\,\xi)\Big|<\varepsilon\end{align}$
$\:$
Tada je $\begin{align}I=\int_{a}^{b} f(x) \, dx \end{align}$ $\:$ Rimanov (određeni) integral fje $f$ na $[a,\,b]$.

Ako postoji Rimanov integral (odnosno limes), $f$ je Riman-integrabilna na $[a,\,b]$. Oznaka $f\,R\,[a,\,b]$

**Stav**. Ako $f:\ [a,\,b]\to\mathbb{R}$ nije ograničena na $[a,\,b]$ onda $\begin{align}\nexists\int_{a}^{b} f(x) \, dx \end{align}$
___
Neka je $f:\ [a,\,b]\to\mathbb{R}$ ograničena i $\mathcal{P}$ je podela intervala $[a,\,b]$.
$\forall i=\overline{1,n}\quad\quad\begin{array}{}m_{i}:=\inf\{ f(x)\ \big|\ x_{i-1}\leqslant x\leqslant x_{i} \}\\M_{i}:=\sup\{ f(x)\ \big|\ x_{i-1}\leqslant x\leqslant x_{i} \}\end{array}$

**Def**. 
$\begin{align}s(f,\,\mathcal{P})=\sum\limits_{i=1}^{n}m_{i}(x_{i}-x_{i-1})\end{align}$ $\quad$ je **donja Darbuova suma**;
$\begin{align}S(f,\,\mathcal{P})=\sum\limits_{i=1}^{n}M_{i}(x_{i}-x_{i-1})\end{align}$ $\quad$ je **gornja Darbuova suma**.

**Stav**. $\forall\mathcal{P}',\,\mathcal{P}''\in\mathcal{P}[a,\,b]\quad s(f,\,\mathcal{P'})\leqslant S(f,\,\mathcal{P''})$
> Dokaz: Neka je $\mathcal{P}$ superpozicija podela $\mathcal{P}'$ i $\mathcal{P}''$,
> tada treba pokazati: $s(f,\,\mathcal{P'})\overset{1.}{\leqslant} s(f,\,\mathcal{P})\overset{2.}{\leqslant} S(f,\,\mathcal{P})\overset{3.}{\leqslant} S(f,\,\mathcal{P''})$
>1. Neki interval podele $\mathcal{P'}$ može da sadrži dve ili više podeone tačke podele $\mathcal{P}$.
>   Neka je $\hat{x}_{i}$ podeona tačka podele $\mathcal{P}$ takva da $\hat{x}_{i}\in[x_{i-1},\,x_{i}]\in\mathcal{P}'$.
>   Tada sabirku $m_{i}(x_{i}-x_{i-1})$ sume $s(f,\,\mathcal{P}')$ odgovaraju dva sabirka $m'_{i}(\hat{x}_{i}-x_{i-1})$, $m''_{i}(x_{i}-\hat{x}_{i})$ sume $s(f,\,\mathcal{P})$.
>   i jer je $m_{i}$ infinum na celom intervalu, važi $m_{i}\leqslant m'_{i},\,m''_{i}$, odakle
>   $m_{i}(x_{i}-x_{i-1})\ \leqslant\ m'_{i}(\hat{x}_{i}-x_{i-1})\ +\ m''_{i}(x_{i}-\hat{x}_{i})$
>   Slično za intervale sa više tačaka. Dakle, važi 1.
>  2. $m_{i}\leqslant M_{i}$. Odakle sledi 2.
>  3. 3\. je slično kao i 1.

$\:$

Odakle,
- $\{ s(f,\,\mathcal{P})\ |\ \mathcal{P}\in\mathcal{P}[a,\,b] \}$ je neprazan i ograničen odozgo sa $S(f,\,\mathcal{P''})$
  $\Rightarrow\quad\exists\sup\{ s(f,\,\mathcal{P})\ |\ \mathcal{P}\in\mathcal{P}[a,\,b] \}=:I_{*}$ — **donji Rimanov integral**.
  $\:$
- $\{ S(f,\,\mathcal{P})\ |\ \mathcal{P}\in\mathcal{P}[a,\,b] \}$ je neprazan i ograničen odozdo sa $s(f,\,\mathcal{P'})$
  $\Rightarrow\quad\exists\inf\{ S(f,\,\mathcal{P})\ |\ \mathcal{P}\in\mathcal{P}[a,\,b] \}=:I^{*}$ — **gornji Rimanov integral**.

Važi $I_{*}\leqslant I^{*}$.

**Teorema** (Definicija pomoću Darbuovih suma). Ako $I_{*}=I^{*}=I$ onda je $I=\begin{align}\int_{a}^{b} f(x) \, dx \end{align}$ Rimanov integral fje $f$ na $[a,\,b]$.

**Stav**. $f:\ [a,\,b]\to\mathbb{R}$ ograničena fja. Tada
$f\,R\,[a,\,b]\quad\Leftrightarrow\quad\forall\varepsilon>0\quad\exists\mathcal{P}\in\mathcal{P}[a,\,b]\ \ :\ \ S(f,\,\mathcal{P})-s(f,\,\mathcal{P})<\varepsilon$
> Dokaz: $\boxed{\Rightarrow}$ Neka je $\begin{align}I=\int_{a}^{b} f(x) \, dx \end{align}$
> Iz definicija supremuma i infinuma:
> - $\forall\varepsilon>0\quad\begin{align}\exists\mathcal{P}'\in\mathcal{P}[a,\,b]\ \ :\ \ S(f,\,\mathcal{P}')<I + \frac{\varepsilon}{2}\end{align}$
> - $\forall\varepsilon>0\quad\begin{align}\exists\mathcal{P}''\in\mathcal{P}[a,\,b]\ \ :\ \ s(f,\,\mathcal{P}'')>I - \frac{\varepsilon}{2}\end{align}$
> 
> Neka je $\mathcal{P}$ superpozicija $\mathcal{P}'$ i $\mathcal{P}''$, tada
> - $\begin{align}S(f,\,\mathcal{P})\leqslant S(f,\,\mathcal{P}')<I + \frac{\varepsilon}{2}\quad\Rightarrow\quad S(f,\,\mathcal{P})<I + \frac{\varepsilon}{2}\end{align}$
> - $\begin{align}I - \frac{\varepsilon}{2}< s(f,\,\mathcal{P}'') \leqslant s(f,\,\mathcal{P})\quad\Rightarrow\quad -s(f,\,\mathcal{P})<-I + \frac{\varepsilon}{2}\end{align}$
>  
>  Odakle, $S(f,\,\mathcal{P})-s(f,\,\mathcal{P})<\varepsilon$
>  $\:$
>  $\boxed{\Leftarrow}$ Pretpostavimo $\begin{align}\nexists\int_{a}^{b} f(x) \, dx\quad\Rightarrow\quad I_{*}<I^{*}\end{align}$.
>  
>  Treba naći $\varepsilon$, takav da $\forall\mathcal{P}\in\mathcal{P}[a,\,b]\quad S(f,\,\mathcal{P})-s(f,\,\mathcal{P})\geqslant\varepsilon$.
>  
>  $\exists c,\,d\in\mathbb{R}\ \ :\ \ \forall\mathcal{P}\in\mathcal{P}[a,\,b]\quad s(f,\,\mathcal{P})\leqslant I_{*}<c<d<I^{*}\leqslant S(f,\,\mathcal{P})$
>   - $S(f,\,\mathcal{P}) > d$
>  - $-s(f,\,\mathcal{P}) > -c$
>
>Odakle, $S(f,\,\mathcal{P})-s(f,\,\mathcal{P}) > d-c$.
>$\varepsilon:=d-c$