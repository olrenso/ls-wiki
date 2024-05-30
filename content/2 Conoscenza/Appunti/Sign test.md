---
share: true
---

Il *sign test* è un [[Test di verifica d'ipotesi|Test di verifica d'ipotesi]] non parametrico analogo al [[One-sample t-test|t-test a campione singolo]] o al [[Paired t-test|Paired t-test]] ma senza il presupposto di [[Distribuzione normale|normalità]] dei dati.
Attraverso il sign test viene verificata l’ipotesi che due [[Campione statistico|campioni]] (o campione e la [[Popolazione statistica|popolazione]]) abbiano la medesima [[Mediana|Mediana]].

Se la mediana del campione è uguale a quella della popolazione (o del secondo gruppo di confronto) allora ci si aspetta di trovare il 50% delle osservazioni inferiori e il 50% superiori alla mediana.
In altri termini si verifica l’ipotesi, tramite una [[Distribuzione binomiale|Distribuzione binomiale]] (approssimata a una [[Distribuzione normale|Curva di Gauss]]), che metà dei dati siano sopra il valore mediano.

Nel caso il campione abbia una numerosità maggiore di 20 vale la seguente equazione:
$$\text{s-test} = \frac{|p-0.5|-\frac{1}{2n}}{\sqrt{\displaystyle\small\frac{0.5^2}{n}}}$$
Dove:
- $p=\frac{k}{n}$ è la frequenza osservata di dati sopra o sotto la mediana di riferimento, $n$ è il numero di osservazioni differenti dalla mediana e $k$ il numero di osservazioni sopra o sotto la mediana (tipicamente viene scelto il valore di $k$ minore).
- $n$ è l’ampiezza del campione;

Si noti che è la medesima equazione del [[One-sample proportion test|Test di una proporzione a campione singolo]].

Nel caso il campione abbia meno di 20 individui la statistica test è $k$ (dove $k$ è il numero minore di osservazioni sopra o sotto la media). Per derivare il [[Valore p|Valore p]] corrispondente si adoperano l’apposita tabella.

> [!tldr]- Valori P per $n\leq20$ e $k\leq9$
> ![[Pasted image 20240220171936.png|Pasted image 20240220171936.png]]

> [!example]- Esempio pratico
> Si vuole verificare che la durata mediana di una consultazione veterinaria sia 12 minuti.
> Sono stati registrate le durate di 43 visite: 22 erano inferiori a 12 minuti, 6 pari a 12 minuti e 15 superiori a 12 minuti.
> 
> ![[Pasted image 20240220170353.png|350]]
> 
> 1. L’ipotesi nulla è che la mediana delle osservazioni non differisce significativamente dalla vera mediana delle consultazioni veterinarie (12 minuti).
> 2. Dati $k=15$ e $n=37$ (le osservazioni differenti dalla mediana), la [[Statistica test|Statistica test]] è pari a: $$\text{s-test} = \frac{|\frac{15}{37}-0.5|-\frac{1}{2\cdot37}}{\sqrt{0.25\frac{1}{37}}} = 0.986$$
> 3. Il [[Valore p|Valore p]] corrispondente è $0.32$.
> 4. Non vi è evidenza statisticamente significativa per poter rifiutare $H_0$.