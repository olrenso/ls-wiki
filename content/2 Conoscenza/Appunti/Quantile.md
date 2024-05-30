---
aliases:
  - Quantili
share: true
---

Un *quantile* è una [[Misura di posizione|Misura di posizione]] che suddivide una [[Distribuzione statistica|Distribuzione statistica]] o [[Distribuzione di probabilità|probabilistica]] ordinata[^1] in più intervalli con egual frequenza o probabilità.

[^1]: In modo non decrescente.

Date $n$ osservazioni di un [[Variabile statistica|Carattere statistico]] $x$ si definisce $\alpha$-quantile (quantile d’ordine $\alpha$), dove $\alpha \in[0,1]$, quel valore di $x_\alpha$ per cui la proporzione (o [[Frequenza statistica|Frequenza]] relativa cumulata) di osservazioni inferiori o uguali a $x_\alpha$ è pari a $\alpha$ e la proporzione di osservazioni maggiori o uguali a $x_\alpha$ è $(1-\alpha)$.

![[Pasted image 20240208121706.png|300]]

Per ogni suddivisione in $q$ sottoinsiemi vi sono $(q-1)$ $q$-quantili, uno per ciascun numero intero $k\in(0,q)$.

Sulla base del numero d’intervalli in cui la distribuzione è suddivisa si individuano i seguenti quantili:
- [[Mediana|Mediana]]: $q=2$, $\alpha = \frac{1}{2}$
- [[Quartili|Quartili]]: $q=4$, $\alpha = \frac{1}{4},\frac{2}{4}, \frac{3}{4}$
- *quintile*: $q=5$
- *decile*: $q=10$
- *ventile*: $q=20$
- [[Centile|Centile e percentile]]: $q=100$, $\alpha = \frac{1}{100}, \frac{2}{100}, \dots,\frac{99}{100}$