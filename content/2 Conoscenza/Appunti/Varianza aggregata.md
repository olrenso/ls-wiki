---
aliases:
  - Varianza composita
  - Varianza complessiva
  - Varianza combinata
share: true
---

La *varianza aggregata* è uno [[Stimatore|Stimatore]] della [[Varianza|Varianza]] di differenti [[Campione statistico|campioni]] con [[Media aritmetica|Media]] differente se si suppone che la [[Varianza|Varianza]] delle rispettive [[Popolazione statistica|popolazioni]] sia la medesima.

Dato un insieme di [[Varianza campionaria|Varianze campionarie]] $s_i^2$ di $m$ campioni, ognuno con $n_i$ elementi (dove $n_i$ è costante), la varianza aggregata $s_p^2$ è la [[Media aritmetica|Media]] delle varianze:
$$s_p^2 = \frac{\sum_{i=1}^{m} s_i^2}{m}$$

Nel caso in cui l’ampiezza dei campioni non è uniforme la varianza aggregata è calcolata come la media ponderata con pesi i [[Gradi di libertà statistici|Gradi di libertà]] ($n-1$):
$$s_p^2 = \frac{\sum_{i=1}^m(n_i-1)s_i^2}{\sum_{i=1}^m(n_i -1)} = \frac{(n_1-1)s_1^2 + (n_2-1)s_2^2+\cdots+(n_m-1)s_m^2}{n_1 + n_2 + \cdots + n_m - m}$$