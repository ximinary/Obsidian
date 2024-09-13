#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$

$\begin{array}{}\\\\\downarrow\\\\\\\uparrow\end{array}\ \begin{array}{|l|}\hline\text{Segment koda}\\\hline\text{Segment podataka}\\\hline\text{Hip}\\\\\\\text{Stek}\\\hline\end{array}\quad\quad\Bigg\downarrow\text{adrese}$

### Segment koda (.text)
— mašinski kod programa zaštićen od pisanja
### Segment podataka (.data i .BSS)
— globalne, statičke lokalne promenljive, konstantni podaci: konstantni niske.
### Hip segment
— [[Dinamička alokacija memorije (C)|dinamička alokacija memorije]]
### Stek segment
— prostor za funkcije
Prilikom jednog poziva funkcije kreira se stek okvir, koji sadrži:
- argumente funkcije (za to se koriste i registri)
- lokalne promenljive
- međurezultate izračunavanja
- adresa povratka (skok na kraju fje) — moguće i preko registra
- adresa stek okvira funkcije-pozivaoca.
- pri pozivanju neke funkcije koja ne može da se vrati rezultat preko registra, mesto za upisivanje rezultata u trenutnoj funkciji. 

![[stek.png]] #todo