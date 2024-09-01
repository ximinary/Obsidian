#fax #math #a1 [deo poglavlja [[Niz brojeva|"niz brojeva"]]]
$\:$

**Def**. **Limes niza** $(x_{n})$ je $\lim\limits_{ n \to \infty }x_{n}=x\in\overline{\mathbb{R}}\quad \Leftrightarrow\quad \forall\varepsilon>0\quad\exists N\in \mathbb{N}\quad\forall n\geqslant N\quad x_{n}\in \mathrm{O}_{\varepsilon}(x)$

**Def**. 
- Ako $\exists\lim\limits_{ n \to \infty }x_{n}\in\mathbb{R}$, onda $(x_{n})$ **konvergira**.
- Ako $\exists\lim\limits_{ n \to \infty }x_{n}=\pm\infty$, onda $(x_{n})$ **određeno divergira**.
- Ako $\nexists\lim\limits_{ n \to \infty }x_{n}$, onda $(x_{n})$ **neodređeno divergira**.

[[analiza1_3_1.png|Stav]]. $f:\ (a,\,+\infty)\to\mathbb{R},\ \ x_{n}:=f(n).$
Tada $\exists\lim\limits_{ x \to +\infty }f(x)=L\quad\Rightarrow\quad\exists\lim\limits_{ n \to \infty }x_{n}=L$ ^ec8129

### Svojstva limesa niza
- [[analiza1_3_limNizSv1.png|1)]] Konvergentan niz je ograničen
- [[Limes funkcije#^2c8b48|2)]] $\lim\limits_{ n \to \infty }a_{n}=a\in\mathbb{R},\ \lim\limits_{ n \to \infty }b_{n}=b\in\mathbb{R}$. Tada:
   - $\exists\lim\limits_{ n \to \infty }(a_{n}+b_{n})=a+b$
    - $\exists\lim\limits_{ n \to \infty }a_{n}\, b_{n}=a\, b$
    - $\begin{align}\exists\lim\limits_{ n \to \infty }\frac{a_{n}}{b_{n}}=\frac{a}{b}\end{align}$
- [[analiza1_3_limNizSv5.png|3)]] $\lim\limits_{ n \to \infty }a_{n}=a\underset{(<)}{>}c\quad\Rightarrow\quad\exists N\in\mathbb{N}\ \ \ \forall n\geqslant N\ \ \ a_{n}\underset{(<)}{>}c$
- [[analiza1_3_limNizSv6.png|4)]] $\lim\limits_{ n \to \infty }a_{n}=a,\ \lim\limits_{ n \to \infty }b_{n}=b,\ \  \exists N_{1}\in\mathbb{N}\ \ \ \forall n\geqslant N_{1}\ \ \ a_{n}\leqslant b_{n}$
  Tada $a\leqslant b$.
- [[Limes funkcije#^dd4e68|5)]] $\exists N\in\mathbb{N}\quad \forall n>N\quad a_{n}\leqslant b_{n}\leqslant c_{n},$
   $\lim\limits_{ n \to \infty }a_{n}=\lim\limits_{ n \to \infty }c_{n}=a$. Tada $\exists \lim\limits_{ n \to \infty }b_{n}=a$.
- [[analiza1_3_limNizSv8.png|6)]] $\lim\limits_{ n \to \infty }\left|a_{n}\right|=0\quad \Leftrightarrow\quad\lim\limits_{ n \to \infty }a_{n}=0$
- 7\) ![[analiza1_3_limNizSv3.png]]

[[Limes funkcije#Neodređeni oblici|Neodređeni oblici]]

### [[Osnovni limesi#Limesi nizova|Osnovni limesi]]

### Limes monotonog niza
[[analiza1_3_limMonotNiza.png|Teorema]].  ^759dd8
1. $a_{n}\!\uparrow \mathrm{\ i\ ograničen}\quad\Rightarrow\quad\exists\lim\limits_{ n \to \infty }a_{n}= \mathrm{sup}\{ a_{n}\ |\ n\in\mathbb{N} \}$
2. $a_{n}\!\downarrow \mathrm{\ i\ ograničen}\quad\Rightarrow\quad\exists\lim\limits_{ n \to \infty }a_{n}= \mathrm{inf}\{ a_{n}\ |\ n\in\mathbb{N} \}$
3. $a_{n}\!\uparrow (\downarrow) \mathrm{\ i\ nije\ ograničen}\quad\Rightarrow\quad\exists\lim\limits_{ n \to \infty }a_{n}= +\infty\ (-\infty)$

### [[Podnizovi]]
### [[Košijev niz]]
---

### Rešavanje limesa niza
- Rešavanjem [[Limes funkcije#Rešavanje limesa funkcije|limesa funkcije]] i korišćenjem [[Limes niza#^ec8129|stava]].
  $\:$
- Skala. Za $\alpha>0,\ a>1\:\:$važi
  $\ln n \ll n^{\alpha} \ll a^{n}\ll n! \ll n^{n} \ll (n!)^{2},\quad n\to\infty$
  $\:$
- Teorema (Štolceva). $(a_{n}),\,(b_{n})$ su nizovi$;\ \:$ $b_{n}\!\uparrow;\ \:b_{n}\to+\infty,\ n\to\infty$. 
  $\begin{align}\exists\lim\limits_{ n \to \infty }\frac{a_{n}-a_{n-1}}{b_{n}-b_{n-1}}=L\in\overline{\mathbb{R}}\quad\Rightarrow\quad\exists\lim\limits_{ n \to \infty }\frac{a_{n}}{b_{n}}=L\end{align}$
  $\:$
- Stav. $(a_{n})$ je niz i $\lim\limits_{ n \to \infty }a_{n}=a$. Tada
  - $\begin{align}\lim\limits_{ n \to \infty }\frac{a_{1}+a_{2}+\dots+a_{n}}{n}=a\end{align}$
  - ako $a_{n}\ne0,$ onda $\ \ \begin{align}\lim\limits_{ n \to \infty }\frac{n}{\frac{1}{a_{1}}+\frac{1}{a_{2}}+\dots+\frac{1}{a_{n}}}=a\end{align}$
  - ako $a_{n}>0,$ onda $\ \ \begin{align}\lim\limits_{ n \to \infty }\sqrt[n]{a_{1}\,a_{2}\,\dots\,a_{n}}=a\end{align}$

$\:$
- Stav. $(a_{n})$ je pozitivan niz i $\begin{align}\lim\limits_{ n \to \infty }\frac{a_{n+1}}{a_{n}}=L\end{align}$
  Tada $\exists\lim\limits_{ n \to \infty }\sqrt[n]{a_{n}}=L$
  ___
- Limes niza zadatog rekurentno tražimo tako što:
  prvo dokazujemo postojanje pomoću [[Limes niza#^759dd8|teoreme]],
  a zatim menjamo svaki član niza sa $x$ (limes niza) u datoj jednačini, rešavamo i dobijamo $x$.
