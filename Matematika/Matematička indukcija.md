#fax #math #ds1 [deo [[Prirodni brojevi|poglavlja "prirodni brojevi"]]]
$\:$

Sledeći principi su ekvivalentni. 
### Princip matematičke indukcije ([[Prirodni brojevi#Peanove aksiome|P5.]])

Neka je $\Phi$ svojstvo prirodnih brojeva takvo da
  - važi $\Phi(0)$
  - za svaki prirodni broj $n$ $\Big[$ ako važi $\Phi(n)$ onda važi i $\Phi(n')$ $\Big]$

tada $\Phi(n)$ važi za svaki prirodni broj $n$.

### Princip potpune indukcije
Neka je $\Phi$ svojstvo prirodnih brojeva takvo da 
-  za svaki prirodni broj $n$  $\Big[$ ako važi $\forall k<n \ \ \Phi(k)$ onda važi i $\Phi(n)$ $\Big]$

tada $\Phi(n)$ važi za svaki prirodni broj $n$.

[[PPI teorema.png|Teorema]]. PMI $\quad \Rightarrow \quad$ PPI

### Princip najmanjih elemenata
- [[Relacija poretka]]: $\forall n\in \mathbb{N} \ \ \ n< n'$

Neka je $A \ne \varnothing,\ \ A \subseteq \mathbb{N} \ \:$ tada u $A$ postoji [[Relacija poretka#Najmanji, najveći, minimalni, maksimalni|najmanji element]].

[[PNE teorema.png|Teorema]]. PPI $\quad \Rightarrow \quad$ PNE

### Još varijacije matematičke indukcije
1. Neka je $\Phi$ svojstvo prirodnih brojeva takvo da
	  - važi $\Phi(k)$ za neko $k\in \mathbb{N}$
	  - za svaki prirodni broj $n\geqslant k$ $\Big[$ ako važi $\Phi(n)$ onda važi i $\Phi(n')$ $\Big]$

	tada $\Phi(n)$ važi za svaki prirodni broj $n\geqslant k$.
2.  Neka je $\Phi$ svojstvo prirodnih brojeva takvo da
	  - važe $\Phi(0),\,\Phi(1),\, \dots,\, \Phi(k-1)$ za neko $k\in \mathbb{N}$
	  - za svaki prirodni broj $n\geqslant k$ $\Big[$ ako važe $\Phi(n-k),\,\Phi(n-k+1),\, \dots,\, \Phi(n-1)$ onda važi i $\Phi(n)$ $\Big]$

	tada $\Phi(n)$ važi za svaki prirodni broj $n$.