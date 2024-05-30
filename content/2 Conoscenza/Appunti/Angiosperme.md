---
share: true
---
> - Sottoregno: [[Tracheofite|Tracheobionta]]
> 	- Superdivisione: [[Spermatopyhta|Spermatopyhta]]
> 		- Divisione: *Magnoliophyta*

La divisione delle *Angiosperme* è il raggruppamento di piante attualmente esistenti più numeroso, comprendendo circa 275’000 specie con un vasto spettro di caratteristiche.

##### Tassonomia
Comprendono due gruppi principali monofiletici che comprendono il 97% delle Angiosperme.
1. [[Monocotiledoni|Monocotiledoni]]
2. [[Dicotiledoni|Eudicotiledoni]]

Il restante 3% presenta caratteri arcaici che non hanno avuto successo evolutivo e sono rappresentate dai seguenti due gruppi:
- *Angiosperme basali*
- *Magnoliide*

![](549a84d22939294331b40bb3873a1a8d_MD5%201.png)

## Caratteristiche e morfologia
Le angiosperme presentano alcune caratteristiche uniche che le differenziano da 
qualunque altro gruppo di organismi vegetali:
- Ovuli protetti in carpelli.
- Semi racchiusi in frutti.
- Microgametofito ([[Polline|Polline]]) costituito da 3 nuclei.
- Macrogametofito (*Sacco embrionale*) formato da sette cellule e otto nuclei.
- Doppia fecondazione con formazione dell’embrione 2n e dell’endosperma 3n.
- [[Legno eteroxilo|Legno eteroxilo]] composto da trachee, tracheidi, fibre e parenchima.
- [[Floema|Libro]] costituito da tubi cribosi.
- Presenza di diversi metaboliti secondari.


![|400](390e671aca3af80c4be11f81ba94a1cc_MD5%201.png)


#### Riproduzione
- Fiori
- Ovuli protetti dall'ovario che forma il frutto
- Doppia fecondazione con formazione di endosperma
- Riduzione estrema dei gametofiti

```mermaid
stateDiagram-v2
 Direction LR
 sf : <i>Sporofita</i><br>Pianta
 spm : Tetrade
 spf : Tetrade
 gm : <i>Gamete maschile</i><br>Nuclei spermatici
 gf : <i>Gamete femminile</i><br>Oosfera
 ssm : <i>Spore maschili</i><br>Microspore
 ssf : <i>Spore femminili</i><br>Macrospore
 zig : Zigote
 state "Fase Diploide" as 2n {
   	Direction LR
	zig --> sf : Mitosi
}

gm --> zig : Gamia
gf --> zig : Gamia

state spm{
	ssm
}
state spf{
	ssf
}

sf --> ssm : Meiosi
sf --> ssf : Meiosi
```

```mermaid
stateDiagram-v2
 Direction LR
 gmm : <i>Gametofito maschile</i><br>Cellula generativa
 gmf : <i>Gametofito femminile</i><br>Megaspora funzionale
 gtm : Polline
 gtf : Ovario
 gm : <i>Gameti maschili</i><br>Nuclei spermatici
 gf : <i>Gameti femminili</i><br>Oosfera
 spm : <i>Spora maschile</i><br>Microspora maschile
 spf : <i>Spora femminile</i><br>Macrospora femminile
 state "Fase Aploide" as n {
   	Direction LR
	spm --> gmm : Mitosi
	spf --> gmf : Mitosi

	gmm --> gm : Mitosi
	gmf --> gf : Mitosi
}

	state gtf {
		gf
	}
	
	state gtm {
		gm
	}
```