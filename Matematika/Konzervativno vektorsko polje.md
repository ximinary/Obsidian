#fax #math #a3 [deo [[Krivolinijski integral|poglavlja "krivolinijski integral"]]]
$\:$

**Def**. [[Vektorska funkcija|Vektorsko polje]] $\mathbf{f}=\nabla f$ je **konzervativno** (gradijentno), a $f$ je **potencijal** tog polja.

**Teorema** (Uopštenje [[Veza između određenog integrala i izvoda. Njutn-Lajbnicova formula#^08f509|Njutn-Lajbnicove formule]]). Neka je $\mathbf{f}:\ D\to\mathbb{R}^{n}$ konzervativno neprekidno vektorsko polje ($\mathbf{f}=\nabla f$) i neka je $\mathcal{C}$ proizvoljna deo po deo glatka kriva koja spaja tačke $\mathbf{x},\,\mathbf{y}\in D$. Tada
$\begin{align}\int_{\mathcal{C}} \mathbf{f} \cdot d\mathbf{r} = f(\mathbf{y})-f(\mathbf{x})\end{align}$
> Dokaz: Neka je $\mathcal{C}$ parametrizovana sa $\mathbf{r}=(x_{1},\,x_{1},\,\dots,\,x_{n}):\ [a,\,b]\to\mathbb{R}^{n}$
> $\begin{align}\int_{\mathcal{C}} \mathbf{f} \cdot d\mathbf{r} = \int_{\mathcal{C}} \nabla f \cdot d\mathbf{r}= \int_{a}^{b} \sum\limits_{i=1}^{n} (f'_{x_{i}}\circ\mathbf{r})(t)\,x'_{i}(t)\,dt\end{align}$ $=$ \[[[Diferencijabilnost funkcije više promenljivih#^4816ca|*]]] $=$
> $\begin{align}=\int_{a}^{b} (f\circ\mathbf{r})'(t) \, dt=(f\circ\mathbf{r})(b)-(f\circ \mathbf{r})(a)=f(\mathbf{y})-f(\mathbf{x})\end{align}$

$\:$
**Teorema**. Neka je $\mathbf{f}:\ D\to\mathbb{R}^{n}$ neprekidno vektorsko polje. Tada su tvrđenja ekvivalentna:
1. $\mathbf{f}$ je konzervativno.
2. $\forall \mathbf{x},\,\mathbf{y}\in D$ $\quad$ za svaku deo po deo neprekidnu krivu $\mathcal{C}\subset D$ koja spaja $\mathbf{x}$ i $\mathbf{y}$ ista je vrednost $\begin{align}\int_{\mathcal{C}} \mathbf{f} \cdot d\mathbf{r} \end{align}$.
3. Za svaku zatvorenu deo po deo neprekidnu krivu $\mathcal{C}\subset D$ važi $\begin{align}\oint_{\mathcal{C}} \mathbf{f} \cdot d\mathbf{r} =0\end{align}$.  

> Dokaz:
> $\boxed{1. \Rightarrow 2.}$ Prethodna teorema.
> 
> $\boxed{2. \Rightarrow 3.}$ Neka je $\mathcal{C}$ zatvorena deo po deo neprekidna kriva.
> Neka su $\mathcal{C}_{1}\subset\mathcal{C}$ i $\mathcal{C}_{2}\subset\mathcal{C}$ krive koje spajaju tačke $\mathbf{x},\,\mathbf{y}\in\mathcal{C}$  ($\mathcal{C}_{1}\ne\mathcal{C}_{2}$).
> Tada $\mathcal{C}=\mathcal{C}_{1}\cup \mathcal{C}_{2}^{-}$, stoga $\begin{align}\int_{\mathcal{C}} \mathbf{f} \cdot d\mathbf{r}=\int_{\mathcal{C}_{1}} \mathbf{f} \cdot d\mathbf{r}+\int_{\mathcal{C}_{2}^{-}} \mathbf{f} \cdot d\mathbf{r}=\int_{\mathcal{C}_{1}} \mathbf{f} \cdot d\mathbf{r}-\int_{\mathcal{C}_{2}} \mathbf{f} \cdot d\mathbf{r} \xlongequal{\text{pretpostavka}} 0\end{align}$.
> 
> $\boxed{3. \Rightarrow 1.}$ Neka za svaku svaku zatvorenu deo po deo neprekidnu krivu $\mathcal{C}$ važi $\begin{align}\oint_{\mathcal{C}} \mathbf{f} \cdot d\mathbf{r} =0\end{align}$.
> 
> Izaberemo fiksiranu tačku $\mathbf{x}$, a $\mathbf{y}$ je proizvoljno.
> 
> Neka su $\mathcal{C}_{1}$ i $\mathcal{C}_{2}$ dve proizvoljne deo po deo neprekidne krive koje spajaju $\mathbf{x}$ i $\mathbf{y}$, tad za krivu $\mathcal{C}_{1}\cup \mathcal{C}_{2}^{-}$ važi pretpostavka. Stoga, $\begin{align}\int_{\mathcal{C}_{1}} \mathbf{f} \cdot d\mathbf{r}-\int_{\mathcal{C}_{2}} \mathbf{f} \cdot d\mathbf{r}=\int_{\mathcal{C}_{1}\cup\mathcal{C}_{2}^{-}} \mathbf{f} \cdot d\mathbf{r}=0\end{align}$, tj. vrednost $\begin{align}\int_{\mathcal{C}} \mathbf{f}\cdot d\mathbf{r} \end{align}$ ne zavisi od izbora krive.
> 
> Označimo sa $\mathcal{C}(\mathbf{x},\,\mathbf{y})$ proizvoljnu krivu sa početkom u $\mathbf{x}$ i krajem u $\mathbf{y}$.
> Zbog zaključka u prethodnom pasusu dobro je definisana fja $f:\ D\to\mathbb{R}$ sa $\begin{align}f(\mathbf{y}):=\int_{\mathcal{C}(\mathbf{x},\,\mathbf{y})}  \mathbf{f}\cdot d\mathbf{r} \end{align}$.
> 
> $\begin{align}f'_{x_{i}}(\mathbf{y})=\lim\limits_{ h \to 0 }\frac{f(\mathbf{y}+h\,\mathbf{e}_{i})-f(\mathbf{y})}{h}=\lim\limits_{ h \to 0 }\frac{\begin{align}\int_{\mathcal{C}(\mathbf{y},\,\mathbf{y}+h\mathbf{e}_{i})}\mathbf{f} \cdot d\mathbf{r}\end{align}}{h}=\end{align}$
> > Neka je kriva $\mathcal{C}(\mathbf{y},\,\mathbf{y}+h\mathbf{e}_{i})$ prava, tad nju možemo parametrizovati fjom $\mathbf{r}:\ [0,\,h]\to\mathbb{R}^{n}$ def. sa $\mathbf{r}(t)=\mathbf{y}+t\,\mathbf{e}_{i}$
> 
> $\begin{align}=\lim\limits_{ h \to 0 }\frac{\begin{align}\int_{0}^{h} (\mathbf{f}\circ \mathbf{r})(t) \cdot\mathbf{r}'(t)\, dt\end{align}}{h}=\lim\limits_{ h \to 0 }\frac{\begin{align}\int_{0}^{h} \mathbf{f}(\mathbf{y}+t\,\mathbf{e}_{i}) \cdot\mathbf{e}_{i}\, dt\end{align}}{h}=\end{align}$
> $=\Big[$ Iz [[Riman-integrabilnost funkcija i svojstva određenog integrala#^88105f|teoreme]] $\exists \xi$ između $0$ i $h$ $\Big]=$
>  $\begin{align}=\lim\limits_{ h \to 0 }\frac{h\,\mathbf{f}(\mathbf{y}+\xi\,\mathbf{e}_{i})\cdot\mathbf{e}_{i}}{h}=\lim\limits_{ h \to 0 }\Big(\,\mathbf{f}(\mathbf{y}+\xi\,\mathbf{e}_{i})\cdot\mathbf{e}_{i}\Big)=\mathbf{f}(\mathbf{y})\cdot\mathbf{e}_{i}\end{align}$ 
> 
> Stoga, $\mathbf{f}=\nabla f$

$\:$
> Napomena: Ako važi jedan od uslova $2.$ i $3.$ u prethodnoj teoreme, za dati gradijent možemo naći polaznu funkciju do na koeficijent.

$\:$
**Posledica** (prethodne teoreme i [[Integralna veza skupa i njegove granice#Grinova formula|Grinove formule]]). Neka je $\mathbf{f}=(P,\,Q):\ D\to\mathbb{R}^{2}$ neprekidno vektorsko polje, takvo da su $P'_{y}$ i $Q'_{x}$ neprekidni.
Tada $\mathbf{f}$ je konzervativno akko $P'_{y}=Q'_{x}$

**Posledica** (prethodne teoreme i [[Integralna veza skupa i njegove granice#Stoksova formula|Stoksove formule]]). Neka je $\mathbf{f}=(P,\,Q,\,R):\ D\to\mathbb{R}^{3}$ neprekidno (zajedno sa parcijalnim izvodima) vektorsko polje definisano na prosto-povezanoj oblasti $D$.
Tada $\mathbf{f}$ je konzervativno akko $\nabla\times \mathbf{f}=\mathbf{0}$