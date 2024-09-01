#fax #math #ds1 [deo [[Teorija skupova|teoriji skupova]]]
$\:$

$\lvert A \rvert$ — kardinalnost [skupa](Teorija%20skupova) $A$.

$\lvert A \rvert \in \mathbb{N}\quad \Leftrightarrow \quad A$ je konačan skup,
inače je beskonačan

**Teorema**. Skup $X$ je beskonačan ako postoji pravi podskup $Y$ $\ (Y \subset X)$, takav da su $X$ i $Y$ u bijekciji.

[[teorema. N je beskonačan.png|Teorema]]. Skup prirodnih brojeva je beskonačan.

**Def**.
- Skup je **prebrojiv** ako je u bijekciji sa [$\mathbb{N}$](Prirodni%20brojevi.md).
- Skup je **najviše prebrojiv** ako je konačan ili prebrojiv.
- Skup je **neprebrojiv** ako nije najviše prebrojiv.

Teorema.  [$\mathbb{N}$](Prirodni%20brojevi.md),  [$\mathbb{Z}$](Celi%20brojevi.md), svaki njihov beskonačan podskup, $\mathbb{N}^n$, $\ \mathbb{Z}^n$, $\:$ [$\mathbb{Q}$](Racionalni%20brojevi) $\subseteq \mathbb{Z} \times \mathbb{N}$ su prebrojivi skupovi.

Stav. $\exists f: \ \ X \stackrel{_{na}}{\to} \mathbb{N} \quad \Rightarrow \quad X$ je najviše prebrojiv.
$\quad \quad \ \exists f: \ \ \mathbb{N} \stackrel{_{1-1}}{\to} X \quad \Rightarrow \quad X$ je najviše prebrojiv.

[[teorema. R je neprebrojiv.png|Teorema]].  [$\mathbb{R}$](Realni%20brojevi.md) je neprebrojiv.

### Kardinalnost.

**Def**. $\lvert A \rvert \leq \lvert B \rvert \;$ ($A$ je je kardinalnosti manje ili jednako od $B$) ako $\ \exists f: \ \ A \stackrel{_{1-1}}{\to} B$

**Def**. $\lvert A \rvert = \lvert B \rvert \;$ ($A$ i $B$ su iste kardinalnosti) ako postoji bijekcija između $A$ i $B$.

**Def**. $\lvert A \rvert < \lvert B \rvert \;$ ($A$ je je kardinalnosti strogo manje od $B$) ako $\lvert A \rvert \leq \lvert B \rvert \;$ i $\; \lvert A \rvert \ne \lvert B \rvert$

Važi:
- $\lvert A \rvert = \lvert B \rvert \quad \Rightarrow \quad \lvert A \rvert \leq \lvert B \rvert \;$ i $\; \lvert B \rvert \leq \lvert A \rvert \;$
- $\lvert A \rvert \leq \lvert B \rvert \;$ i $\; \lvert B \rvert \leq \lvert C \rvert \quad \Rightarrow \quad \lvert A \rvert \leq \lvert C \rvert$
- $\lvert A \rvert = \lvert B \rvert \;$ i $\; \lvert B \rvert = \lvert C \rvert \quad \Rightarrow \quad \lvert A \rvert = \lvert C \rvert$

**Teorema (Kantor-Bernštajn)**. 
$\lvert A \rvert \leq \lvert B \rvert \;$ i $\; \lvert B \rvert \leq \lvert A \rvert \quad \Rightarrow \quad \lvert A \rvert = \lvert B \rvert$

| Skup                           | Kardinalnost           |
| ------------------------------ | ---------------------- |
| Konačan                        | Broj elemenata         |
| Prebrojiv                      | $\aleph_0$ — alef nula |
| $\mathbb{R}$,  $\mathcal{P}(\mathbb{N})$ | $c$ — moć kontinuuma   |

Ako je $n \in \mathbb{N}$, tada važi $\ \ n < \aleph_0 < c$