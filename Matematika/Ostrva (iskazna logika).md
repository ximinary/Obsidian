#fax #math #ds1/vežbe


«‎Ostrva» je tip zadataka iz [[Iskazna logika|iskazne logike‎]], koji često dolazi na ispitu iz ds1.

U zadatku je dato ostrvo sa nekim ljudima kojih treba rasporediti u dva plemena da bi važila svaka stavka iz zadatka.

### Plemena
1. **Istinozborci** uvek kažu istinu.
2. **Lažovi** uvek lažu.
3. **Špijuni** kažu istinu ljudima iz svog plemena, i lažu ljudima iz drugog.
4. **Dupli agenti** lažu ljudima iz svog plemena, i kažu istinu ljudima iz drugog.

Osoba $A$ kaže osobi $B$ neko tvrđenje $p$.
U zavisnosti od plemena osoba, $p$ može biti tačno ili netačno.
Razmatramo sve 4 mogućnosti: $A$ i $B$ su u prvom plemenu, $A$ je u prvom $B$ je u drugom plemenu, i td.  U svakoj od mogućnosti gledamo da li je tačno $p$.

### Varijacije ostrva
1. Ostrvo istinozboraca i lažova.

Za svaku osobu $X$, kažemo da je $x=1$ ako je $X$ istinozborac, $x = 0$ ako je lažov.
$A$ kaže $B$-u tvrđenje $p$.
Razmatramo sve mogućnosti pomoću tablice:

|a|b|p| |
| :-: | :-: | :-: | --- |
|0|0|0| $A$ je lažov, $B$ je lažov. $p$ je netačno (jer $A$ laže svima)|
|0|1|0| $A$ je lažov, $B$ je ist. $p$ je netačno (jer $A$ laže svima)|
|1|0|1| $A$ je ist., $B$ je lažov. $p$ je tačno (jer $A$ kaže istinu svima)|
|1|1|1| $A$ je ist., $B$ je ist. $p$ je tačno (jer $A$ kaže istinu svima)|

Iz ove tablice razumemo da na ovom ostrvu uvek važi $a \Leftrightarrow p$ 
($p$ je tačno akko je $A$ ist.)

2.  Ostrvo špijuna i lažova

Za svaku osobu $X$, kažemo da je $x=1$ ako je $X$ špijun, $x = 0$ ako je lažov.
$A$ kaže $B$-u tvrđenje $p$.
Razmatramo sve mogućnosti pomoću tablice:

|a|b|p| |
| :-: | :-: | :-: | --- |
|0|0|0| $A$ je lažov, $B$ je lažov. $p$ je netačno (jer $A$ laže svima)|
|0|1|0| $A$ je lažov, $B$ je špijun. $p$ je netačno (jer $A$ laže svima)|
|1|0|0| $A$ je špijun, $B$ je lažov. $p$ je netačno (jer $A$ laže drugom plemenu)|
|1|1|1| $A$ je špijun, $B$ je špijun. $p$ je tačno (jer $A$ kaže istinu svom plemenu)|
Iz ove tablice razumemo da na ovom ostrvu uvek važi $a \land b \Leftrightarrow p$ 

3. Ostrvo istinozboraca i špijuna

Za svaku osobu $X$, kažemo da je $x=1$ ako je $X$ istinozborac, $x = 0$ ako je špijun.
$A$ kaže $B$-u tvrđenje $p$.
Razmatramo sve mogućnosti pomoću tablice:

|a|b|p|
| :-: | :-: | :-: |
|0|0|1|
|0|1|0|
|1|0|1|
|1|1|1|

Iz ove tablice razumemo da na ovom ostrvu uvek važi $(b \Rightarrow a) \Leftrightarrow p$ 

4. Ostrvo istinozboraca i duplih agenata

Za svaku osobu $X$, kažemo da je $x=1$ ako je $X$ istinozborac, $x = 0$ ako je dupli agent.
$A$ kaže $B$-u tvrđenje $p$.
Razmatramo sve mogućnosti pomoću tablice:

|a|b|p|
| :-: | :-: | :-: |
|0|0|0|
|0|1|1|
|1|0|1|
|1|1|1|

Iz ove tablice razumemo da na ovom ostrvu uvek važi $a \lor b \Leftrightarrow p$ 

5. Ostrvo severnih i južnih špijuna.

Za svaku osobu $X$, kažemo da je $x=1$ ako je $X$ severni špijun, $x = 0$ ako je južni.
$A$ kaže $B$-u tvrđenje $p$.
Razmatramo sve mogućnosti pomoću tablice:

|a|b|p| |
| :-: | :-: | :-: | --- |
|0|0|1| $A$ je južni, $B$ je južni. $p$ je tačno (jer $A$ kaže istinu svom plemenu)|
|0|1|0| $A$ je južni, $B$ je severni. $p$ je netačno (jer $A$ laže drugom plemenu)|
|1|0|0| $A$ je severni, $B$ je južni. $p$ je netačno (jer $A$ laže drugom plemenu)|
|1|1|1| $A$ je severni, $B$ je severni. $p$ je tačno (jer $A$ kaže istinu svom plemenu)|


Iz ove tablice razumemo da na ovom ostrvu uvek važi $(a \Leftrightarrow b) \Leftrightarrow p$ 

6. Ostrvo severnih i južnih duplih agenata.

Za svaku osobu $X$, kažemo da je $x=1$ ako je $X$ severni dupli agent, $x = 0$ ako je južni.
$A$ kaže $B$-u tvrđenje $p$.
Razmatramo sve mogućnosti pomoću tablice:

|a|b|p|
| :-: | :-: | :-: |
|0|0|0|
|0|1|1|
|1|0|1|
|1|1|0|
Iz ove tablice razumemo da na ovom ostrvu uvek važi $(a \underline{\vee} b) \Leftrightarrow p$ 

7. Ostrvo špijuna i duplih agenata.

Za svaku osobu $X$, kažemo da je $x=1$ ako je $X$ špijun, $x = 0$ ako je dupli agent.
$A$ kaže $B$-u tvrđenje $p$.
Razmatramo sve mogućnosti pomoću tablice:

|a|b|p|
| :-: | :-: | :-: |
|0|0|0|
|0|1|1|
|1|0|0|
|1|1|1|
Iz ove tablice razumemo da na ovom ostrvu uvek važi $b \Leftrightarrow p$ 

### Prenos iskaza $p$ u  logički oblik.
Neka je $x = 1$ ako je $X$ iz *prvog* plemena, $x = 0$ ako je *grugog*.

| Iskaz                                           | Logički oblik               |
| ----------------------------------------------- | --------------------------- |
| $A$ je iz *prvog*                               | $a$                         |
| $A$ je iz *drugog*                              | $\neg a$                    |
|||
| $A$ i $B$ su iz *prvog*                         | $a \land b$                 |
| $A$ je iz *prvog* i $B$ je iz *drugog*          | $a \land \neg b$                 |
| $A$ je iz *drugog* i $B$ je iz *prvog*          | $\neg a \land b$       |
| $A$ i $B$ su iz *drugog*                        | $\neg a \land \neg b$       |
|||
| $A$ je iz *prvog* ili $B$ je iz *prvog*         | $a \lor b$                  |
| $A$ je iz *prvog* ili $B$ je iz *drugog*         | $a \lor \neg b$                  |
| $A$ je iz *drugog* ili $B$ je iz *prvog*        | $\neg a \lor b$        |
| $A$ je iz *drugog* ili $B$ je iz *drugog*        | $\neg a \lor \neg b$        |
|||
| ili $A$ ili $B$ je iz *prvog*                   | $a \underline{\vee} b$      |
| ili $A$ ili $B$ je iz *drugog*                  | $a \underline{\vee} b$      |
| $A$ i $B$ su iz različitih plemena              | $a \underline{\vee} b$      |
| $A$ i $B$ su iz istog plemena                   | $a \Leftrightarrow b$       |
|||
| Ako je $A$ iz *prvog*, onda je $B$ iz *prvog*   | $a \Rightarrow b$           |
| Ako je $A$ iz *prvog*, onda je $B$ iz *drugog*  | $a \Rightarrow \neg b$      |
| Ako je $A$ iz *drugog*, onda je $B$ iz *prvog*  | $\neg a \Rightarrow b$      |
| Ako je $A$ iz *drugog*, onda je $B$ iz *drugog* | $\neg a \Rightarrow \neg b$ |


### Primeri
1. 

![[ostrva 1.1.png]]
Rešenje:
![[ostrva 1.2.png]]

2. 
   
![[ostrva 2.1.png]]
Rešenje:
![[ostrva 2.2.png]]