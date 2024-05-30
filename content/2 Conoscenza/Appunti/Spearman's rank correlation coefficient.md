---
aliases:
  - Coefficiente di correlazione per ranghi di Spearman
share: true
---

Il *coefficiente di correlazione per ranghi di Spearman* è una misura statistica non parametrica di correlazione, non necessariamente lineare, fra due [[Variabile statistica|Variabili]].
È un’alternativa non parametrica al [[Indice di correlazione di Pearson|Coefficiente di correlazione di Pearson]] per il [[Test di verifica d'ipotesi|Test di verifica d'ipotesi]] della correlazione fra due variabili.

Assume valori compresi fra $-1$ e $+1$, i cui i limiti indicano una correlazione perfetta.

Date $n$ coppie delle variabili $x$ e $y$ ${(x_1,y_1),(x_2,y_2),\cdots,(x_n,y_n)}$ si sostituiscono i valori di $x_i$ e $y_i$ con i rispettivi ranghi dopo aver ordinato i valori in ordine crescente. Si calcola quindi il coefficiente di correlazione:
$$r_s=1-\frac{6\sum d^2}{n^3-n}$$
Dove $d$ è la differenza di rango fra la coppia di valori di un’osservazione e $n$ il numero di osservazioni.