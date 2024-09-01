#fax #math #ds1[deo [[Brojevi|poglavlja "brojevi"]]]
$\:$

### Peanove aksiome
- P1. $\:\:$$0$ je prirodan broj.
- P2. $\:\:$Ako je $x$ prirodan broj tada je i njegov sledbenik $x'$ prirodan broj.
- P3. $\:\:$Ako su $x$ i $y$ prirodni brojevi takvi da je $x' = y'$ onda $x=y$.
- P4. $\:\:$Za svaki  prirodni broj $x$ važi $x'\ne0$.
- P5.  $\:\:$Neka je $\Phi$ svojstvo prirodnih brojeva takvo da
  1. važi $\Phi(0)$
  2. za svaki prirodni broj $x$ ako važi $\Phi(x)$ onda važi i $\Phi(x')$

	 tada $\Phi(x)$ važi za svaki prirodni broj $x$.

$\mathbb{N}=\{ 0,\, 1,\, 2,\, 3,\, \dots \}$
### Fon Nojmanov model
- $0=\varnothing$
- $n' = n \cup\{ n \}$

Tada:
$1 = \{ 0 \} = \{ \varnothing \}$
$2 = \{ 0,\, 1 \}=\{ \varnothing,\, \{ \varnothing \} \}$
$3 = \{ 0,\, 1,\, 2 \} = \{ \varnothing,\, \{ \varnothing \},\, \{ \varnothing,\, \{ \varnothing \} \} \}$
$4= \{ 0,\, 1,\, 2,\, 3 \} = \{ \varnothing,\, \{ \varnothing \},\, \{ \varnothing,\, \{ \varnothing \} \},\, \{ \varnothing,\, \{ \varnothing \},\, \{ \varnothing,\, \{ \varnothing \} \} \} \}$
$\dots$

[[FNM teorema.png|Teorema]]. Fon Nojmanov model zadovoljava [[Prirodni brojevi#Peanove aksiome|Peanove aksiome]].

### [[Matematička indukcija]]

### Operacije $+$ i $\,\cdot\,$ u prirodnim brojevima
**Def**. **Sabiranje** prirodnih brojeva:
- $x + 0 = x$
- $x+y\,' = (x+y)'$

[[prirodni br osbine sabiranja.png|Osobine]]: $\forall x,\,y,\,z \in \mathbb{N}$
1. $x + (y + z) =(x + y) + z$
2. $x + 0 = 0 + x = x$
3. $x + 1 = 1 + x$
4. $x + y = y + x$
5. $x + y = 0 \quad \Rightarrow \quad x = 0 \ \ \mathrm{i}\ \ y = 0$
6. $x + z =y + z \quad \Rightarrow \quad x = y$

**Def**. **Množenje** prirodnih brojeva:
- $x \cdot 0 = 0$
- $x\cdot y\,' = x\cdot y + x$

[[prirodni br osbine množenja.png|Osobine]]: $\forall x,\,y,\,z \in \mathbb{N}$
1. $x \cdot (y + z) = x\cdot y + x\cdot z$
2. $x \cdot (y \cdot z) =(x \cdot y) \cdot z$
3. $(x + y) \cdot z = x\cdot z + y\cdot z$
4. $0 \cdot x = 0$
5. $1 \cdot x = x$
6. $x\cdot y = y\cdot x$
7. $x \cdot y = 0 \quad \Rightarrow \quad x = 0 \ \ \mathrm{ili}\ \ y = 0$

### [[Deljivost]]

### [[Euklidsko deljenje]]

### [[Euklidov algoritam]]

### [[Prost broj]]