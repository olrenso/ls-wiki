---
share: true
---

La *varianza campionaria* $S_X^2$ è la [[Varianza|Varianza]] di una [[Popolazione statistica|Popolazione statistica]] basata sui dati di un [[Campione statistico|Campione statistico]].

Vi sono due [[Stimatore|stimatori]]:

$$S_n^2 = \frac{\sum\limits_{i=1}^n(x_i-\overline{x})^2}{n} \qquad\qquad S_{n-1}^2 = \frac{\sum\limits_{i=1}^n(x_i-\overline{x})^2}{n-1}$$

Dove $x_i$ è il valore dell’$i$-esima osservazione, $\overline{x}$ è il [[Media aritmetica|valore medio]] delle osservazioni e $n$ il numero delle osservazioni.

In quanto la varianza $S_n^2$ tende generalmente a sottostimare la varianza della popolazione, sottraendo un’unità al numero di individui del [[Campione statistico|campione]] ($n-1$) si ottiene un valore meno distorto ($S_{n-1}^2$) della varianza della [[Popolazione statistica|popolazione]].
Ciò è dovuto dal fatto che la [[Media aritmetica|Media]] campionaria $\overline{x}$  — usata come stima della media di popolazione — è calcolata dalle medesime osservazioni con cui si sta calcolando la varianza: i [[Gradi di libertà statistici|Gradi di libertà]] della varianza si riducono di conseguenza a $n-1$.