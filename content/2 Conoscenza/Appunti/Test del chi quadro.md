---
aliases: Test del chi quadrato,
share: true
---
Il *test del* $\chi^2$ (*test del chi quadro*) è un [[Test di verifica d'ipotesi|Test di verifica d'ipotesi]] con cui si confrontano due (o più) [[Proporzione campionaria|proporzioni campionarie]] valutando se i [[Campione statistico|Campioni statistici]] appartengano a due distinte [[Popolazione statistica|popolazioni]].

Segue la [[Distribuzione chi quadrato|Distribuzione chi quadro]].

Affinché il test sia valido devono essere rispettate le seguenti assunzioni:
1. le [[Variabile statistica|Variabili]] studiate sono qualitative;
2. le osservazioni sono espresse in [[Frequenza statistica|Frequenza]] (assoluta);
3. i campioni sono mutualmente esclusivi, ogni individuo è rappresentato una sola volta e possiede un solo risultato;
5. i campioni devono essere casuali e rappresentativi;
6. l’80% delle frequenze (proporzioni) attese deve essere almeno 5.

Il valore della [[Statistica test|Statistica test]] è data dalla formula:
$$\text{test}_{\chi^2} = \sum^n_{i=1}\frac{(\text{O}-\text{E})^2}{\text{E}}\quad{\small\text{con }(\text{r}-1)(\text{c}-1)\text{ GdL}\quad n=r\cdot c}$$

In caso di due soli gruppi con due possibili risultati (tabella 2x2) è:
$$\text{test}_{\chi^2} = \sum_{i=1}^2\frac{(|\text{O}-\text{E}|-0.5)^2}{\text{E}} \quad{\small\text{con } 1 \text{ grado di libertà}}$$

In cui $\text{E}$ e $\text{O}$ sono rispettivamente le frequenze assolute (il numero di osservazioni) attese (*expected*) e osservate (*observed*).

Per il calcolo delle frequenze osservate e attese il test del chi quadro sfrutta una [[Tabella di contingenza|Tabella di contingenza]] $c\times r$ ($c$: colonne; $r$: righe) come quella riportata di seguito.
Ogni colonna riporta uno dei campioni con il numero di osservazioni per ciascun risultato; da queste si calcola il totale delle osservazioni e la [[Proporzione campionaria|Proporzione campionaria]] ([[Frequenza relativa|Frequenza relativa]]).

> [!tldr]+ Tabella risultati osservati
>
> | Risultato osservato     |                       Gruppo 1                        |                       Gruppo 2                        | $\cdots$ |                        Gruppo n                         |                      *Totale*                       |
> | ----------------------- | :---------------------------------------------------: | :---------------------------------------------------: | :------: | :-----------------------------------------------------: | :-------------------------------------------------: |
> | **Categoria 1**         |                          $a$                          |                          $b$                          | $\cdots$ |                          $n_1$                          |                  $a+b+\cdots+n_1$                   |
> | **Categoria 2**         |                          $c$                          |                          $d$                          | $\cdots$ |                          $n_2$                          |                  $c+d+\cdots+n_2$                   |
> | $\qquad\quad\vdots$     |                       $\vdots$                        |                       $\vdots$                        | $\ddots$ |                        $\vdots$                         |                      $\vdots$                       |
> | **Categoria n**         |                          $w$                          |                          $z$                          | $\cdots$ |                          $n_n$                          |                  $w+z+\cdots+n_n$                   |
> |                         |                                                       |                                                       |          |                                                         |                                                     |
> | *Totale*                |                $\sum \text{Gruppo}_1$                 |                $\sum \text{Gruppo}_2$                 | $\cdots$ |                 $\sum \text{Gruppo}_n$                  |             $\sum\sum \text{Gruppo}_i$              |
> | *Frequenza categoria 1* | $\displaystyle\widehat{p}_1=\frac{a}{\sum\text{G}_1}$ | $\displaystyle\widehat{p}_2=\frac{b}{\sum\text{G}_2}$ | $\cdots$ | $\displaystyle\widehat{P}_n=\frac{n_1}{\sum\text{G}_n}$ | $\displaystyle\widehat{p}=\frac{\sum\text{C}_1}{N}$ |

Le categorie sono solitamente raggruppate in «successo» e «fallimento», tuttavia il test del chi quadro non pone limiti al numero di esse.

I risultati attesi sono calcolati supponendo che gli $n$ gruppi appartengano a una sola popolazione: viene calcolata la [[Frequenza statistica|Frequenza]] di ogni categoria sugli $N$ individui e moltiplicata per la numerosità di ciascun gruppo per ottenere il numero di individui attesi per ogni combinazione $\text{gruppo}\times\text{categoria}$.

> [!tldr]+ Tabella risultati attesi
> 
> | Risultato atteso    |                       Gruppo 1                        |                       Gruppo 2                        | $\cdots$ | Gruppo n                                              |
> | ------------------- | :---------------------------------------------------: | :---------------------------------------------------: | -------- | ----------------------------------------------------- |
> | **Categoria 1**     | $\displaystyle\sum\text{G}_1\frac{\sum\text{C}_1}{N}$ | $\displaystyle\sum\text{G}_2\frac{\sum\text{C}_1}{N}$ | $\cdots$ | $\displaystyle\sum\text{G}_n\frac{\sum\text{C}_1}{N}$ |
> | **Categoria 2**     | $\displaystyle\sum\text{G}_1\frac{\sum\text{C}_2}{N}$ | $\displaystyle\sum\text{G}_2\frac{\sum\text{C}_2}{N}$ | $\cdots$ | $\displaystyle\sum\text{G}_n\frac{\sum\text{C}_2}{N}$ |
> | $\qquad\quad\vdots$ |                       $\vdots$                        |                       $\vdots$                        | $\ddots$ | $\vdots$                                              |
> | **Categoria n**     | $\displaystyle\sum\text{G}_1\frac{\sum\text{C}_n}{N}$ | $\displaystyle\sum\text{G}_2\frac{\sum\text{C}_n}{N}$ | $\cdots$ | $\displaystyle\sum\text{G}_n\frac{\sum\text{C}_n}{N}$ |

> [!tldr]- Tabelle semplificate per un test $2\times 2$
> 
> | Risultato osservato  |                  Gruppo 1                  |                  Gruppo 2                  |                 *Totale*                 |
> | -------------------- | :----------------------------------------: | :----------------------------------------: | :--------------------------------------: |
> | **Successo**         |                    $a$                     |                    $b$                     |                  $a+b$                   |
> | **Fallimento**       |                    $c$                     |                    $d$                     |                  $c+d$                   |
> |                      |                                            |                                            |                                          |
> | *Totale*             |                   $a+c$                    |                   $b+d$                    |               $n=a+b+c+d$                |
> | *Frequenza successi* | $\displaystyle\widehat{p}_1=\frac{a}{a+c}$ | $\displaystyle\widehat{p}_2=\frac{b}{b+d}$ | $\displaystyle\widehat{p}=\frac{a+b}{n}$ |
> 
> | Risultato atteso |              Gruppo 1               |              Gruppo 2               |
> | ---------------- | :---------------------------------: | :---------------------------------: |
> | **Successo**     | $\displaystyle(a+c)\frac{(a+b)}{n}$ | $\displaystyle(b+d)\frac{(a+b)}{n}$ |
> | **Fallimento**   | $\displaystyle(a+c)\frac{(c+d)}{n}$ | $\displaystyle(b+d)\frac{(c+d)}{n}$ |

> [!example]- Esempio pratico ($2\times 2$)
> In una popolazione di topi si è osservata un’incidenza del diabete autoimmune di 24% per i maschi e 73% per le femmine.
> Si vuole verificare se il sesso sia determinante nell’insorgere della patologia. Su una popolazione di 100 individui, 50 vengono castrati subito dopo la nascita mentre il restante 50 (gruppo di controllo) subisce un’operazione placebo.
> Al termine del periodo di monitoraggio l’incidenza del diabete è 52% ($\widehat{p}_1$) nel gruppo castrato e 24% ($\widehat{p}_2$) nel gruppo di controllo.
> 
> **Risultati osservati**
> 
> |                   | Topi castrati | Topi controllo | *Totale* |
> | ----------------- | :-: | :-: | -: |
> | **Con diabete**   | 26            | 12             | 38       |
> | **Senza diabete** | 24            | 38             | 62       |
> |                   |               |                |          |
> | *Totale*          | 50            | 50             | 100      |
> 
> **Risultati attesi** [^1]
> 
>|                   |           Topi castrati            |           Topi controllo           |
> | ----------------- | :--------------------------------: | :--------------------------------: |
> | **Con diabete**   | $\displaystyle50\frac{38}{100}=19$ | $\displaystyle50\frac{38}{100}=19$ |
> | **Senza diabete** | $\displaystyle50\frac{62}{100}=31$ | $\displaystyle50\frac{62}{100}=31$ |
> 
> 1. L’ipotesi nulla è che entrambi i gruppi abbiano la medesima frequenza (proporzione) d’incidenza del diabete e la differenza osservata è solo dovuta al caso, $H_0:\widehat{p}_1=\widehat{p}_2$
> 2. La [[Statistica test|Statistica test]] è pari a: $$\begin{align}\text{test}_{\chi^2} &= \frac{(|24-19|-0.5)^2}{19}+\frac{(|12-19|-0.5)^2}{19}=\\&=\frac{(|24-31|-0.5)^2}{31}+\frac{(|38-31|-0.5)^2}{31}=7.17\end{align}$$
> 3. Dalla [[Distribuzione chi quadrato|Distribuzione chi quadro]] $7.17$ (per 1 [[Gradi di libertà statistici|grado di libertà]]) corrisponde a un [[Valore p|Valore p]] di $0.007$.
> 4. L’ipotesi $H_0$ può essere rifiutata con sufficiente livello di significatività: la castrazione è correlata all’insorgenza del diabete. Questo può *suggerire* che il diabete nei topi potrebbe essere associato al livello di testosterone nel sangue.
> 5. L’[[Intervallo di fiducia|Intervallo di fiducia]] della reale differenza fra le proporzioni è: $$\begin{align}\text{CI}_{95\%} &= (\widehat{p}_1-\widehat{p}_2)\pm1.96\sqrt{\frac{\widehat{p}_1(1-\widehat{p}_1)}{n_1}+\frac{\widehat{p}_2(1-\widehat{p}_2)}{n_2}}=\\&= (0.52-0.24)\pm1.96\sqrt{\frac{0.52\cdot0.48}{50}+\frac{0.24\cdots0.76}{50}}=\\&=0.28\pm1.96\cdot0.0929=[0.098;0.462]\end{align}$$
>    Ovvero seppur l’incremento dell’incidenza del diabete osservato è stato del 28%, l’effetto reale potrebbe essere del 10% così come del 46%.

[^1]: Le frequenze identiche fra i due gruppi sono una conseguenza della medesima numerosità dei campioni.

> [!example]- Esempio pratico ($3\times 2$)
> Si vuole confrontare l’efficacia di tre differenti metodi d’inseminazione artificiale nei bovini. 993 vacche sono state assegnate casualmente a uno dei tre metodi e inseminate una sola volta. I risultati sono riportati in tabella.
>
> |                        | Metodo 1 | Metodo 2 | Metodo 3 | *Totale* |
> | ---------------------- | -------- | -------- | -------- | -------- |
> | **Gravida**            | 275      | 192      | 261      | 728      |
> | **Non gravida**        | 78       | 64       | 123      | 265      |
> |                        |          |          |          |          |
> | *Totale*               | 353      | 256      | 384      | 993      |
> | *Frequenza gravidanze* | 0.78     | 0.75     | 0.68     | 0.733    |
> 
> Mentre i risultati attesi sono:
> 
> |                 | Metodo 1              | Metodo 2              | Metodo 3              |
> | --------------- | --------------------- | --------------------- | --------------------- |
> | **Gravida**     | $353\cdot0.733=258.8$ | $256\cdot0.733=187.7$ | $384\cdot0.733=281.5$ |
> | **Non gravida** | $353\cdot0.267=94.2$  | $256\cdot0.267=68.3$  | $384\cdot0.267=102.5$ |
> 
> 1. L’ipotesi nulla è che le [[Proporzione della popolazione|proporzioni di popolazione]] per ciascuno dei tre metodi sia la stessa; l’ipotesi alternativa che siano differente.
> 2. La [[Statistica test|Statistica test]] risulta: $$\begin{align}\text{test}_{\chi^2}&=\frac{(275-258.8)^2}{258.8}+\frac{(78-94.2)^2}{94.2}+\frac{(192-187.7)^2}{187.7}\\&+\frac{(64-68.3)^2}{68.3}+\frac{(261-281.5)^2}{281.5}+\frac{(123-102.5)^2}{102.5}=\\&=9.78\end{align}$$
> 3. Dati $(3-1)\cdot(2-1)=2$ [[Gradi di libertà statistici|Gradi di libertà]], $9.78$ corrisponde a un [[Valore p|Valore p]] compreso fra 0.001 e 0.01 (0.008 per la precisione).
> 4. L’ipotesi nulla $H_0$ viene rifiutata: almeno uno dei tre metodi comporta una differente proporzione di bovine gravide (in positivo o in negativo).
