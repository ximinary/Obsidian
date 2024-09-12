#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$

### Od izvornog do izvršivog programa
- PRETPROCESIRANJE — jednostavne [[Makroi i uslovno prevođenje (C)|zamene]] u tekstu programa. Objedinjava kod iz različitih datoteka (```#include```) u **jedinici prevođenja**.
  ```
  gcc -E 1.c
  ```
  ^14a8a4
- KOMPILACIJA
  Jedinica prevođenja $\to$ **objektni modul** (ne može da se izvrši)
	- Predni sloj: 
		- <u>leksička analiza</u> (izdvajanje leksema)
		- <u>sintaksička analiza</u> (kreiranje sintaksičkog stabla)
		- <u>semantička analiza</u> (transformacija stabla)
		- <u>generisanje međukoda</u> ("asemblerski kod")
	- Srednji sloj:
		- <u>optimizacija međukoda</u>
	- Zadnji sloj:
		- <u>generisanje ciljnog (mašinskog) koda</u>
		- <u>optimizacija ciljnog koda</u>
	```
  gcc -c 1.c     //rezultat u 1.o
  ```
 
- POVEZIVANJE — kreiranje jedinstvene izvršive datoteke od jednog ili više objektnih modula (koje su dobiti kompilacijom ili već postoje) — poveziva adrese funkcija i nekih promenljivih.
  ```
  gcc program -o 1.o 2.c -m    //-m za <math.h>
  ```

[[Od izvornog do izvršivog.png|Primer]]
### Organizacija koda u više datoteka i ```make```

