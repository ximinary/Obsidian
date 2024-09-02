#fax #math #a1 [deo poglavlja [[Niz brojeva|"niz brojeva"]]]
$\:$

**Def**. $(a_{\varphi(n)})$ je podniz niza $(a_{n})$ ako je  $\varphi:\mathbb{N}\to\mathbb{N}$ strogo rastuća.

**(!)** Za strogo rastuću fju $\varphi:\mathbb{N}\to\mathbb{N}$ važi $\varphi(n)\geqslant n$.

**Def**. $b$ je tačka nagomilavanja niza $(a_{n})$ ako $\exists (a_{\varphi(n)})$ — podniz, takav da $\lim\limits_{ n \to \infty }a_{\varphi(n)}=b$

**Def**. Ako je $A$ skup tačaka nagomilavanja niza $(a_{n})$, onda:
- $\underset{n\to \infty}{\overline{\text{lim} }}\ a_{n}:= \max A$ — limes superior (gornji limes)
- $\underset{n\to \infty}{\underline{\text{lim} }}\ a_{n}:= \min A$ — limes inferior (donji limes)
$\:$

[[analiza1_3_6.png|Stav]]. $\begin{align}\lim\limits_{ n \to \infty }a_{n}=a\in\overline{\mathbb{R}}\quad\Rightarrow\quad&\forall \text{podniz\ } (a_{\varphi(n)})\quad \lim\limits_{ n \to \infty }a_{\varphi(n)}=a&&\\ &\left(\underset{n\to \infty}{\overline{\text{lim} }}\ a_{n}=\underset{n\to \infty}{\underline{\text{lim} }}\ a_{n}=a\right)&&\end{align}$

Posledica. Niz $(a_{n})$ ima dve različite tačke nagomilavanja $\ \ \Rightarrow$
$\Rightarrow\ \ \nexists\lim\limits_{ n \to \infty }a_{n}$
$\:$

[[analiza1_3_7.png|Stav]]. $a\in\overline{\mathbb{R}}$ je tačka nagomilavanja niza $(a_{n})\quad\Leftrightarrow$
$\Leftrightarrow\quad\forall\varepsilon>0\quad$ beskonačno mogo članova niza $(a_{n})$ su u $\mathrm{O}_{\varepsilon}(a)$ 
$\:$

[[analiza1_3_BVT.png|Teorema]] (Bolcano-Vajerštrasova). Svaki ograničen niz $(a_{n})$ ima tačku nagomilavanja. ^dd96ed
