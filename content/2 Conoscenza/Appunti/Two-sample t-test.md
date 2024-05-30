---
aliases:
  - t-test a campione doppio
  - t-test a due campioni
  - unpaied t-test
  - t-test non accoppiato
  - t-test disaccoppiato
share: true
---

Il *t-test a campione doppio* (*two-sample t-test*) o *t-test non accoppiato* (*unpaired t-test*) è un [[t-test|Test t]] impiegato per confrontare una [[Statistica test|Statistica]] di due [[Campione statistico|campioni]] indipendenti di una stessa [[Popolazione statistica|Popolazione statistica]].

È uno dei [[Test di verifica d'ipotesi|Test di verifica d'ipotesi]] più usati e perciò abusati; affinché non venga usato in modo scorretto è opportuno valutare attentamente le assunzioni su cui si basa:
1. i due campioni devono essere indipendenti (oltre che rappresentativi), ovvero un dato elemento può appartenere a un solo campione;
2. la [[Variabile statistica|Variabile]] d’interesse deve essere approssimabile con una [[Distribuzione normale|Distribuzione normale]], in ognuno dei due campioni;
3. la variabilità ([[Varianza|Varianza]]) osservata nei dati dei due campioni deve essere approssimativamente uguale (*omoschedastica*). In caso contrario si deve usare il *t-test modificato*.

$$\text{t-test}_2 = \frac{\overline{x}_1 -\overline{x}_2}{\displaystyle\sqrt{s^2\left(\frac{1}{n_1}+\frac{1}{n_2}\right)}}\quad{\small\text{con } n_1+n_2-2\text{ gradi di libertà}}$$

In cui:
- $\overline{x}_1$ e $\overline{x}_2$ sono, rispettivamente, la [[Media aritmetica|Media]] campionaria del primo e del secondo campione;
- $n_1$ e $n_2$ sono le osservazioni del primo e del secondo campione;
- $s^2$ è la [[Varianza aggregata|Varianza aggregata]]: $\displaystyle\small s^2 = \frac{(n_1-1){s_1}^2+(n_2-1){s_2}^2}{n_1+n_2-2}$

L’[[Intervallo di fiducia|Intervallo di confidenza]] è $\displaystyle(\overline{x}_1-\overline{x}_2) \pm t_{0.05}\text{SE}(\overline{x}_1-\overline{x}_2) = \displaystyle(\overline{x}_1-\overline{x}_2) \pm t_{0.05}\sqrt{s^2\left(\frac{1}{n_1}+\frac{1}{n_2}\right)}$

Il t-test modificato (il quale non segue la [[Distribuzione t di Student|Distribuzione t]]) per il confronto di due campioni il cui scarto quadratico medio è differente assume la forma di:
$$\text{t-test}_{2'}  = \frac{\overline{x}_1 -\overline{x}_2}{\displaystyle\sqrt{\left(\frac{s_1^2}{n_1}+\frac{s_2^2}{n_2}\right)}}$$

> [!example]- Esempio pratico
> Si vuole studiare l’effetto sul peso corporeo al momento dell’accoppiamento di un piano nutrizionale ad elevato apporto calorico su una popolazione di pecore.
> La popolazione è stata suddivisa in due gruppi, uno di controllo e uno sottoposto al piano nutrizionale per tre settimane prima dell’accoppiamento.
> Da ciascun gruppo è stato estratto un campione e misurato il peso; i risultati sono riportati in tabella.
> 
> |      | Controllo |      |     |      | Ingrassato |      |
> |:----:|:---------:|:----:| --- |:----:|:----------:|:----:|
> | 62.5 |   63.9    | 69.2 |     | 70.7 |    67.8    | 69.8 |
> | 66.8 |   65.7    | 62.6 |     | 71.8 |    66.8    | 68.1 |
> | 69.5 |   67.2    | 61.1 |     | 64.9 |     67     |  66  |
> | 64.1 |   65.2    | 61.8 |     | 68.2 |    67.1    | 69.4 |
> | 65.3 |   63.5    | 69.6 |     | 69.4 |    67.6    | 69.8 |
> | 65.6 |   65.3    | 71.1 |     | 64.4 |    66.1    | 67.9 |
> | 66.4 |   65.1    |  67  |     | 66.9 |    62.7    | 66.2 |
> | 66.1 |   64.8    | 67.5 |     | 69.4 |    64.6    | 64.2 |
> | 68.6 |   67.4    | 68.2 |     |      |            |      |
> | 62.5 |    66     | 63.6 |     |      |            |      |
> 
> $$\overline{x}_c=65.77\quad\overline{x}_i=67.37 \quad s_p^2=2.51$$
> 
> 1. L’ipotesi nulla afferma che non vi è differenza fra la media dei due gruppi $H_0: \overline{x}_c = \overline{x}_i$. L’ipotesi alternativa dichiara che vi è una significativa differenza.
> 2. Si osservano graficamente i dati (p. e. con un [[Box-plot|Diagramma a scatola e baffi]]) per assicurarsi che seguano una [[Distribuzione normale|Distribuzione normale]] e che la [[Varianza|Varianza]] fra i due campioni sia simile.
> 3. Viene calcolata la [[Statistica test|Statistica test]] come: $$\text{t-test}_2=\frac{67.37-65.77}{\sqrt{\displaystyle2.51\left(\frac{1}{24}+\frac{1}{30}\right)}} = 2.43\quad{\small\text{con }24+30-2\text{ GdL}}$$
> 4. Il [[Valore p|Valore p]] corrispondente è 0.018 ($0.01 < P <0.02$).
> 5. L’ipotesi nulla difficilmente è vera e viene rifiutata a favore dell’ipotesi alternativa.
> 6. L’[[Intervallo di fiducia|Intervallo di fiducia]] della reale differenza fra le medie è $[0.28;2.91]$:$$\text{CI}_{95\%}=\underset{\overline{x}_i-\overline{x}_c}{(67.37-65.77)}\pm \underset{t_{0.05}}{2.007}\cdot\underset{\text{SE}(\overline{x}_i-\overline{x}_c)}{0.655} = 1.59\pm1.31$$