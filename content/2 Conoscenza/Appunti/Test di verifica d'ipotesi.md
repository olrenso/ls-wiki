---
aliases: Hypothesis testing, Test d'ipotesi, Verifica delle ipotesi, Test delle ipotesi,
share: true
---

Un *test di verifica d’ipotesi* è uno strumento statistico inferenziale usato per decidere se i dati a disposizione supportano una particolare ipotesi; ovvero se data una [[Statistica campionaria|Statistica campionaria]] è possibile trarre conclusioni riguardo la [[Popolazione statistica|popolazione]].

Si definisce *ipotesi nulla* $H_0$ l’ipotesi considerata *non falsa*[^1] fino a prova evidente contro la sua veridicità e *ipotesi alternativa* $H_a$ (o $H_1$) l’affermazione accettata in caso cui l’ipotesi nulla sia falsa.

[^1]: Spesso invece di considerare $H_0$ vera si preferisce sostenere che non è possibile rifiutare l’ipotesi nulla: $H_0$ è vera oppure gli strumenti statistici usati non sono sufficientemente potenti da (o i dati a disposizione non sono adatti a) falsificarla.

Un’ipotesi può essere *semplice* se specifica un solo valore (es. $H_0 : X = 18$) o *composta* se prende in considerazione un intervallo; quest’ultima può essere *unilaterale* (es. $H_1 : X > 18$) o *bilaterale* (es. $H_1 : X \neq 18$).
L’ipotesi nulla deve sempre essere un uguaglianza o una disuguaglianza debole; spesso è semplice.

Quando l’ipotesi alternativa è unilaterale si parla di *test a coda singola* (o *test a una coda*), mentre, più comunemente, quando l’ipotesi alternativa è bilaterale il test è detto *a doppia coda*.

La scelta dell’ipotesi è basata su una *regola di decisione*, per esempio se $H_0: X \leq 20$ si può decidere di rifiutarla quando $X > 20.175$.

Nello scegliere l’una o l’altra ipotesi si possono commettere due errori:
- *errore di primo tipo* quando l’ipotesi nulla è vera ma viene rifiutata;
- *errore di secondo tipo* quando l’ipotesi nulla è falsa ma non viene rifiutata.

La [[Probabilità|Probabilità]] dell’errore di primo tipo è detta *livello di significatività* o $\alpha$, mentre la probabilità dell’errore di secondo tipo è indicata da $\beta$. La probabilità $1-\beta$, ovvero la probabilità di rifiutare l’ipotesi nulla quando questa è falsa, è definita *potenza del test*.

| Decisione sull’ipotesi nulla | Ipotesi nulla vera                                             | Ipotesi nulla falsa                                     |
| ---------------------------- | -------------------------------------------------------------- | ------------------------------------------------------- |
| Non rifiuto $H_0$            | Decisione corretta: $p=1-\alpha$                               | Decisione errata:  $p=\beta$                            |
| Rifiuto $H_0$                | Decisione errata: $p=\alpha$<br>(*livello di significatività*) | Decisione corretta: $p=1-\beta$<br>(*potenza del test*) |

Al diminuire della probabilità di errore di primo tipo è sempre associato un incremento della probabilità di errore di secondo tipo, ossia: ogni riduzione di $\alpha$ comporta un aumento di $\beta$, e viceversa.
Nella pratica si tende a scegliere il livello di significatività più basso possibile (spesso $\alpha=0.05$) e, con tale probabilità, viene dichiarata la regola di decisione; solo in secondo luogo viene derivata la probabilità $\beta$.

Sovente invece di determinare a priori il livello di significatività (o [[Intervallo di fiducia|Intervallo di confidenza]]) si impiega il [[Valore p|p-value]] che fornisce il più piccolo livello di significatività a cui l’ipotesi nulla può essere rifiutata.

> [!tldr]+ Metodo generale di un test di verifica d’ipotesi
> 1. Dichiarare l’ipotesi nulla $H_0$ e l’ipotesi alternativa.
> 2. Raccogliere i dati e [[Visualizzazione dei dati|visualizzarli graficamente]] per dedurne una possibile [[Distribuzione statistica|distribuzione]]. Valutare la presenza di [[Outlier|Outlier]].
> 3. Scegliere, anche in base alle considerazioni effettuate nel punto 2, il test più adatto e calcolarne la [[Statistica test|Statistica test]].
> 4. Determinare il [[Valore p|Valore p]] associato al valore della statistica test.
> 5. Decidere se è possibile rifiutare l’ipotesi nulla.
> 6. Se opportuno, calcolare l’[[Intervallo di fiducia|Intervallo di fiducia]].

Alcuni test di verifica d’ipotesi sono qui riportati.
- *Test parametrici*: la variabile in esame deve seguire una determina distribuzione (in genere una [[Distribuzione normale|Distribuzione normale]]).
	- Confronto fra medie
		- z-test, la varianza $\sigma^2$ è nota;
		- [[t-test|t-test]], la varianza $\sigma^2$ è ignota;
		- [[Analisi della varianza|ANOVA]]
	- Confronto fra varianze
		- [[F-test|F-test]]
		- *Test di Levene*
	- Confronto fra proporzioni
		- [[One-sample proportion test|One-sample proportion test]]
		- [[Test del chi quadro|Test del chi quadro]]
- *Test non parametrici* o a distribuzione libera: la variabile oggetto di studio può distribuirsi (o non distribuirsi) secondo una qualsiasi [[Distribuzione di probabilità|Distribuzione di probabilità]].
	- [[Sign test|Sign test]]
	- [[Mann-Whitney U test|Mann-Whitney U test]]
	- [[Wilcoxon signed rank test|Wilcoxon signed rank test]]

| ![[Pasted image 20240213192238.png|Pasted image 20240213192238.png]] | ![[Pasted image 20240213192316.png|Pasted image 20240213192316.png]] |
|:------------------------------------:|:------------------------------------:|
|                                      |                                      |

Vedi anche: [[Prontuario test statistici.canvas|Prontuario test statistici.canvas]]