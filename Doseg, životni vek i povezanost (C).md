#fax #cs/prog/c [deo [[Programski jezik C|jezika C]]]
$\:$

### Doseg identifikatora 
— određuje deo programa u kojem je identifikator vidljiv.

Globalni:
- doseg **datoteke** — ime važi od tačke uvođenja do kraja datoteke (globalne promenljive);

Lokalni:
- doseg **bloka** — ime važi od tačke uvođenja do kraja bloka (lokalne promenljive);
- doseg **funkcije** — ime važi u celoj funkciji (lokalne promenljive koje se koriste uz ```goto``` naredbu)
- doseg **prototipa funkcije** — ime važi u okviru prototipa funkcije.
$\:$

Konflikt identifikatora — smatraju se kao različite promenljive.
```c
int main() {
	int a = 3, i;
	for (i = 0; i < 4; i++) {
		int a = 5;
		printf("%d ", a);
	}
	printf("%d\n", a);
	return 0;
}
// ispis: 5 5 5 5 3
```

### Životni vek objekata. ```static``` i ```auto```

### Povezanost identifikatora. ```ststic``` i ```extern```