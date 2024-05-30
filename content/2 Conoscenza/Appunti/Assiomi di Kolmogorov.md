---
aliases:
  - Assiomi della probabilità
  - Assiomi di probabilità
  - Definizione assiomatica della probabilità
share: true
---

Gli *assiomi di Kolmogorov* o *assiomi della probabilità* sono una definizione matematica del concetto di [[Probabilità|Probabilità]].

Sia $S$ uno [[Spazio campionario|Spazio campionario]] di un [[Esperimento aleatorio|Esperimento casuale]], sia $F$ lo spazio degli eventi e sia $P(E)$ la probabilità di un generico [[Evento probabilistico|Evento]] $E$.
Valgono i seguenti tre assiomi.
1. La probabilità di un evento è un numero reale non negativo: $$P(E) \in\mathbb{R},\;P(E)\geq 0 \quad \forall E\in F$$
2. La probabilità che almeno un evento elementare si verifichi è 1: $$P(S) = 1$$
3. Per ogni insieme di $n$ eventi mutualmente esclusivi la probabilità dell’evento unione è uguale alla somma delle probabilità dei singoli eventi: $$P\left(\bigcup_{i = 1}^n E_i\right) = \sum_{i=1}^n P(E_i)$$

Da tali assiomi si possono dedurre varie regole per il calcolo delle probabilità.
1. *Probabilità insieme vuoto*: la probabilità dell’evento impossibile è nulla: $P(\varnothing) =0$
2. *Intervallo di definizione*: la probabilità di un evento $E$ è compresa fra 0 e 1: $0\leq P(E)\leq 1 \quad \forall E \in F$
3. *Monotonicità*: dati due eventi $A$ e $B$ tali che $A$ è un sottoinsieme di $B$ la probabilità $P(A$) è inferiore o uguale a $P(B)$: $\text{se} \; A \subseteq B \;\text{allora}\; P(A) \leq P(B)$
4. *Regola addittiva*: dati due eventi $A$ e $B$, non necessariamente mutualmente esclusivi, la probabilità che si verifichi o $A$ o $B$ (probabilità dell’evento unione $A\cup B$) è pari alla somma delle singole probabilità $P(A)$ e $P(B)$ sottratta della probabilità che si verifichi sia $A$ che $B$ (probabilità dell’evento intersezione $A\cap B$): $P(A\cup B) = P(A)+P(B) - P(A\cap B)$
   Si noti che se $A$ e $B$ sono mutualmente esclusivi ($A\cap B = \varnothing$) si è di fronte al terzo assioma.
5. *Regola moltiplicativa*: dati due eventi $A$ e $B$ statisticamente indipendenti la probabilità che si verifichino entrambi ($A\cap B$) è data dal prodotto delle probabilità dei singoli eventi: $P(A\cap B) = P(A)\cdot P(B)$
   Qualora $B$ sia dipendente da $A$ la probabilità $P(A\cap B)$ è data dal prodotto tra la probabilità di $A$ e la *probabilità condizionale* di $B$ dato il verificarsi di $A$: $P(A\cap B) = P(A) \cdot P(B|A)$
6. *Regola dell’evento complementare*: la probabilità che non si verifichi un dato evento $A$ è $1-P(A)$: $P(A^c) = P(S-A) = 1-P(A)$
7. *Probabilità condizionata*: dati due eventi $A$ e $B$ la probabilità condizionata dell’evento $B$ sapendo che si è verificato $A$ è ricavata come: $P(B|A) = \frac{P(A\cap B)}{P(A)} \quad P(A) >0$