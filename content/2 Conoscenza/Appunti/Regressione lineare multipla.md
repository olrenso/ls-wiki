---
aliases: []
share: true
---

La *regressione lineare multipla* è un [[Regressione lineare|Modello di regressione lineare]] in cui la variabile risultato (v. dipendente) è correlata a due o più variabili predittrici (v. indipendenti).

Date $k$ variabili indipendenti la retta di regressione della popolazione è data dall’equazione:
$$Y_\text{pop} = \alpha + \beta_1x_1 + \beta_2x_2+\cdots+\beta_kx_k$$
Dove:
- $x_i$ è il valore dell’i-esima variabile indipendente rilevata per ogni individuo;
- $\alpha$ è il valore medio di $y$ quando tutte le variabili predittrici hanno valore $0$;
- $\beta_i$ è il coefficiente parziale di regressione per ciascuna i-esima variabile.

Ciascun coefficiente parziale di regressione $\beta_i$ esprime la risposta di $y$ alla variazione unitaria della relativa variabile indipendente $x_i$ quando tutte le altre variabili sono mantenute costanti.

Lo [[Stimatore|Stimatore]] della regressione lineare multipla di popolazione è pari a:
$$Y=a+b_1x_1+b_2x_2+\cdots+b_kx_k$$
Dove $Y$ è la stima della media di $y$, $a$ è la stima di $\alpha$ e $b$ è la stima di $\beta$.