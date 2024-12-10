#fax #math #a2 [deo [[Analiza|analize]]]

### Podela

**Def**. Neka su $a=x_{0}<x_{1}<\dots<x_{n}=b$. Skup $\mathcal{P}=\Big\{ [x_{i-1},\,x_{i}]\ \Big|\ i=\overline{1,n} \Big\}$ je **podela** intervala $[a,\,b]$.

- $x_{0},\,x_{1},\,\dots,\,x_{n}$ su **podeove tačke** podele $\mathcal{P}$.

- $\begin{align}\lambda(\mathcal{P})=\max_{i=\overline{1,\,n}}(x_{i}-x_{i-1})\end{align}\ \:$ je **parametar podele** $\mathcal{P}$.

- $\mathcal{P}[a,\,b]$ — skup svih podela intervala $[a,\,b]$.
___
**Def**. $\mathcal{P},\,\mathcal{P}'\in\mathcal{P}[a,\,b]$. $\ \:$ $\mathcal{P}'$ je **finija** (**grublja**) podela od $\mathcal{P}$ ako je skup podeovih tačaka podele $\mathcal{P}'$ nadskup (podskup) skupa podeovih tačaka podele $\mathcal{P}$.

**Stav**. $\forall\mathcal{P}',\,\mathcal{P}''\in\mathcal{P}[a,\,b]\quad\exists\mathcal{P}\in\mathcal{P}[a,\,b]\ \ :\ \ \mathcal{P}$ je finija i od $\mathcal{P}'$ i od $\mathcal{P}''$
(Skup podeonih tačaka $\mathcal{P}$ je unija podeonih tačaka $\mathcal{P}'$ i $\mathcal{P}''$).
Tada $\mathcal{P}$ je **superpozicija podela** $\mathcal{P}'$ i $\mathcal{P}''$.

___

$\xi_{i}\in[x_{i-1},\,x_{i}],\quad \forall i=\overline{1,n}$. Tada su
$\xi=(\xi_{1},\,\xi_{2},\,\dots,\,\xi_{n})$ istaknute tačke podele $\mathcal{P}$.

**Def**. $(\mathcal{P},\,\xi)$ — **podela sa istaknutim tačkama** intervala $[a,\,b]$
### Definicija određenog integrala pomoću integralnih suma


**Def**. Neka je $f:\ [a,\,b]\to\mathbb{R}\ \:$ i $\ \:(\mathcal{P},\,\xi)$ podela sa istaknutim tačkama intervala $[a,\,b]$. Zbir $\begin{align}\sigma(f,\,\mathcal{P},\,\xi)=\sum\limits_{i=1}^{n}(x_{i}-x_{i-1})\,f(\xi_{i})\end{align}$ je **integralna suma**.

---
**Def**. Neka je $f:\ [a,\,b]\to\mathbb{R}$. $\ \:$ $I\in\mathbb{R}$ je limes integralnih suma $\sigma(f,\,\mathcal{P},\,\xi)$ kad $\lambda(\mathcal{P})\to0$, ako
$\begin{align}\forall\varepsilon>0\quad\exists\delta>0\quad\forall\binom{(\mathcal{P,\,\xi} )\ \text{— podela sa istaknutim tačkama}}{\text{ intervala }[a,\,b]\text{ takva da } \mathcal{P}(\lambda)<\delta}\quad \Big|I-\sigma(f,\,\mathcal{P},\,\xi)\Big|<\varepsilon\end{align}$
$\:$
Tada je $\begin{align}I=\int_{a}^{b} f(x) \, dx \end{align}$ $\:$ **Rimanov** (**određeni**) **integral** fje $f$ na $[a,\,b]$.

Ako postoji Rimanov integral (odnosno limes), $f$ je Riman-integrabilna ($\mathcal{R}$-integrabilna) na $[a,\,b]$. Oznaka $f\,\mathcal{R}\,[a,\,b]$

**Stav**. Ako $f:\ [a,\,b]\to\mathbb{R}$ nije ograničena na $[a,\,b]$ onda $\begin{align}\nexists\int_{a}^{b} f(x) \, dx \end{align}$

### Definicija određenog integrala pomoću Darbuovih suma
Neka je $f:\ [a,\,b]\to\mathbb{R}$ ograničena i $\mathcal{P}$ je podela intervala $[a,\,b]$. Tada
$\forall i=\overline{1,n}\quad\quad\begin{array}{}m_{i}:=\inf\limits_{x\in[x_{i-1},\,x_{i}]}f(x)\\M_{i}:=\sup\limits_{x\in[x_{i-1},\,x_{i}]}f(x)\end{array}$

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

### [[Riman-integrabilnost funkcija i svojstva određenog integrala]]

### [[Veza između određenog integrala i izvoda. Njutn-Lajbnicova formula]]

### [[Metode integracije (određeni integral)]]

### [[Primene određenog integrala]]