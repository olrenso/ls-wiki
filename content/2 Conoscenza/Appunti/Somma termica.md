---
aliases: GDD, Growing degree days,
share: true
---
La *somma termica* è una tecnica di stima della lunghezza del ciclo colturale e degli stadi fenologici di una coltura basata sui *gradi utili giornalieri* o GDD (*Growing degree days*), ossia sulla [[Temperatura dell'aria|Temperatura media dell’aria]] e sulle temperature cardinali e critiche della coltura.

Ogni giorno in cui la temperatura media ($T_\text{media} = \frac{\sum_{i=0}^n i}{n} \approx \frac{T_\text{min} + T_\text{max}}{2}$) è compresa fra le temperature cardinali la pianta accumula un certo numero di gradi utili, sinonimo di un incremento di [[Biomassa vegetale|Biomassa vegetale]] dovuto a un [[Tasso di crescita colturale|Tasso di crescita]] maggiore di zero.

I gradi utili giornalieri sono calcolati come segue:
- Se la temperatura media è inferiore o maggiore delle temperature critiche minima o massima $\text{GDD} = 0$
- Se la temperatura è maggiore della cardinale minima $\text{GDD} = T_\text{media} - T_\text{min}$
- Se la temperatura media è pari alla cardinale ottimale $\text{GDD} = T_\text{ott} - T_{min}$
- Se la temperatura è maggiore della cardinale ottimale $\text{GDD} = \frac{(T_\text{ott}-T_\text{min})\cdot(T_\text{max}-T_\text{media})}{T_\text{max}-T_\text{ott}}$

Graficamente la funzione dei gradi utili si compone di tre segementi lineari che semplificano e approssimano la curva del [[Tasso di crescita colturale|CGR]] della coltura in esame.

![|300](413b52839e9afd9eae687e34cb565a2b_MD5%201.png)

La somma dei gradi utili lungo il ciclo — seppur essendo un modello approssimativo rispetto alla relazione fra temperatura e [[Tasso di crescita colturale|CGR]] e non inclusivo di variabili quali la disponibilità d’acqua, di nutrienti e della temperatura del suolo (durante la germinazione e l’emergenza), presenza di stress, … — consente di stimare con una certa precisione il ciclo colturale di determinate colture come mais e pisello.