---
aliases: Sistemi irrigui,
share: true
---
Un *sistema irriguo* è quel complesso di opere idrauliche, impianti, [[Sistemazioni idraulico-agrarie|Sistemazioni idraulico-agrarie]] e opportuni metodi e scelte gestionali finalizzato al prelievo, trasporto e distribuzione dell’acqua [[Irrigazione|irrigua]] ai suoli agrari.

I sistemi irrigui, consentendo l’[[Irrigazione|Irrigazione]], garantiscono la disponibilità idrica per soddisfare il [[Fabbisogno irriguo|Fabbisogno irriguo]] e di conseguenza consentono un’adeguata redditività delle attività agricole.

È possibile generalizzare la struttura di un sistema irriguo in cinque componenti, la *fonte idrica* da cui si attinge l’acqua, il *campo* ove l’acqua è consegnata e le opere di *prelievo*, *trasporto* ed *erogazione* che consentono il trasporto — in congiunzione con le opportune infrastrutture e scelte gestionali — dell’acqua dalla fonte all’appezzamento agrario.

```mermaid
stateDiagram-v2
Direction LR
	f : Fonti idriche
	p : Prelievo
	t : Trasporto
	e : Erogazione
	c : Campo
	
	
	state "Infrastrutture, attrezzature e gestione" as n {
	   	Direction LR
		p --> t
		t --> e
	}
	
	f --> p
	e --> c
```

L’infrastruttura costituente la componente attiva di un sistema irriguo sorge dall’insieme di svariate opere idrauliche, associate alle rispettive componenti gestionali, quali:

| Componenti fisiche    | Componenti gestionali                              |
| --------------------- | -------------------------------------------------- |
| [[Derivazione irrigua\|Opere di derivazione]]  | Regolazione delle portate derivate                 |
| [[Rete di adduzione|Rete di adduzione]]     | Gestione della rete                                |
| [[Rete di distribuzione irrigua|Rete di distribuzione irrigua]] | Gestione della rete                                |
| [[Metodo irriguo|Metodo irriguo]]        | Programmazione e gestione degli interventi irrigui |
| [[Rete di drenaggio|Rete di drenaggio]]     | Gestione della rete                                |

L’organizzazione di un sistema irriguo è spesso *collettiva* dove la derivazione da una o più fonti idriche è a disposizione a più utenti finali costituenti un [[Consorzio irriguo|Consorzio irriguo]]. Aziende particolarmente estese o dotate di una propria fonte irrigua possono possedere un sistema irriguo *aziendale*.