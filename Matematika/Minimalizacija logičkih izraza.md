#fax #math #cs/ar [deo [[Iskazna logika|iskazne logike]] i [[Računarstvo|računarstva]]]
$\:$

Transformirati [[Normalne forme|savršeni DNF]] u [[Normalne forme|DNF]] sa najmanje veznika.

### Metod algebarskih transformacija
1. grupisanje: $x\,K+\overline x\,K=K$ 
   Primer: $x\,\overline y \,z +x\,\overline y\,\overline  z=x\,\overline y$
   $\:$
2. udvojenje: $K=K+K$
   Primer: $\overline x\,\overline y\,\overline z + \boxed{\overline x\,\overline y\,z}+\overline x\, y\, z=(\overline x\,\overline y\,\overline z + \boxed{\overline x\,\overline y\,z})+(\boxed{\overline x\,\overline y\,z}+\overline x\, y\, z)=$
   $= \overline x\,\overline y + \overline x\, z$ 
   
### Metod Karnoovih mapa
![[KarnooveMape.png]]
[[KarnooveMapePrimer.png|Primeri]]

### Metod Kvin-Meklaskog
![[KvinMek.png]]
[[KvinMekPrimer1.png|Primeri]]
[[KvinMekPrimer2.png|Primer sa korišćenjem Petrikovog metoda]]

---

[[MinimNebitneVrednosti.png|Minimalizacija u prisustvu nebitnih vrednosti sa primerima]]