#fax #math #ds1 #cs/ar [deo [[Iskazna logika|iskazne logike]]]
$\:$

1. **Negacija** iskaza $p$ je
   $\neg p$ ;   $\quad \overline{p}$ ;   $\quad$ **NOT** $p$:

| $p$ | $\neg p$ |
| :-: | :------: |
|  0  |    1     |
|  1  |    0     |

^b24d81

2. **Konjunkcija** iskaza $p$ i $q$ je
   $p \land q$ ;   $\quad p \cdot q$ ;   $\quad pq$ ;  $\quad p$ **AND** $q$:

| $p$ | $q$ | $p \land q$ |
| :-: | :-: | :---------: |
|  0  |  0  |      0      |
|  0  |  1  |      0      |
|  1  |  0  |      0      |
|  1  |  1  |      1      |

^96b28f

3. **Disjunkcija** iskaza $p$ i $q$ je
   $p \lor q$ ;   $\quad p+q$ ;  $\quad p$ **OR** $q$:

| $p$ | $q$ | $p \lor q$ |
| :-: | :-: | :--------: |
|  0  |  0  |     0      |
|  0  |  1  |     1      |
|  1  |  0  |     1      |
|  1  |  1  |     1      |

^66b381

4. **Eksluzivna disjunkcija** iskaza $p$ i $q$ je
   $p \underline{\vee} q$ ;   $\quad p \oplus q$ ;  $\quad p$ **XOR** $q$:

| $p$ | $q$ | $p \underline{\vee} q$ |
| :-: | :-: | :--------------------: |
|  0  |  0  |           0            |
|  0  |  1  |           1            |
|  1  |  0  |           1            |
|  1  |  1  |           0            |
5. **Implikacija** iskaza $p$ i $q$ je
   $p \Rightarrow q$ :

| $p$ | $q$ | $p \Rightarrow q$ |
| :-: | :-: | :---------------: |
|  0  |  0  |         1         |
|  0  |  1  |         1         |
|  1  |  0  |         0         |
|  1  |  1  |         1         |
6. **Ekvivalencija** iskaza $p$ i $q$ je
   $p \Leftrightarrow q$ ;   $\quad p \sim q$ ;  $\quad p$ **NXOR** $q$:

| $p$ | $q$ | $p \Leftrightarrow q$ |
| :-: | :-: | :-------------------: |
|  0  |  0  |           1           |
|  0  |  1  |           0           |
|  1  |  0  |           0           |
|  1  |  1  |           1           |
7. **Negacija konjunkcije** (Šeferova funkcija) iskaza $p$ i $q$ je
   $p \uparrow q$ ;   $\quad p$ **NAND** $q$:

| $p$ | $q$ | $p \uparrow q$ |
| :-: | :-: | :------------: |
|  0  |  0  |       1        |
|  0  |  1  |       1        |
|  1  |  0  |       1        |
|  1  |  1  |       0        |
8. **Negacija disjunkcije** (Pirsova funkcija) iskaza $p$ i $q$ je
   $p \downarrow q$ ;  $\quad p$ **NOR** $q$:

| $p$ | $q$ | $p \downarrow q$ |
| :-: | :-: | :--------------: |
|  0  |  0  |        1         |
|  0  |  1  |        0         |
|  1  |  0  |        0         |
|  1  |  1  |        0         |
