---
aliases:
  - Speranza matematica
share: true
---

Il *valore atteso* $\mathbb{E}$, anche detto *media* µ o *speranza matematica*, è il risultato più probabile di un fenomeno o [[Esperimento aleatorio|Esperimento aleatorio]].
Più precisamente il valore atteso di una [[Variabile aleatoria|Variabile stocastica]] $X$ è la media dei possibili risultati di essa, ciascuno pesato per la propria [[Probabilità|Probabilità]].

###### Variabile aleatoria discreta
Data una [[Variabile aleatoria|Variabile aleatoria]] $X$ discreta il valore atteso $\mathbb{E}[X]$ è dato dalla media ponderata dei risultati rispetto alla loro [[Probabilità|Probabilità]] (ottenuta dalla [[Funzione di probabilità|Funzione di probabilità]] $P_X(x)$):
$$\mathbb{E}[X]= \micro_X=\sum_{i=1}^\infty x_iP_X(X=x_i) $$

In presenza di una qualunque funzione $g(X)$ della variabile $X$ con funzione di probabilità $P_X(x)$ il valore atteso $\mathbb{E}[g(X)]$ viene definito come:
$$\mathbb{E}[g(X)] = \sum_{i=1}^\infty g(x_i)P_X(x_i)$$

###### Variabile aleatoria continua
Data una [[Variabile aleatoria|Variabile aleatoria]] $X$ continua e data $f(x)$ la sua [[Funzione di densità di probabilità|Funzione di densità di probabilità]]:
$$\mathbb{E}[X] = \micro_X = \int_{-\infty}^{+\infty} x f(x)\;dx$$
E analogamente a quanto detto per una variabile aleatoria discreta:
$$\mathbb{E}[g(X)] = \int_{-\infty}^{+\infty}g(x)f(x)\;dx$$