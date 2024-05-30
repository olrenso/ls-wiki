---
aliases: Valore riproduttivo, BV, EBV, Estimated breeding value, Valore riproduttivo stimato,
share: true
---
Il *breeding value* (*BV*), o *valore riproduttivo*, è un valore che esprime l’apporto genetico, per un dato carattere, di un riproduttore verso la propria prole. 
In altre parole indica il possibile miglioramento genetico che si potrebbe ottenere utilizzando il materiale genetico di un riproduttore.

Data la natura complessa del genoma di un individuo non è possibile sapere con esattezza il valore riproduttivo di un carattere, si utilizza per cui l’*estimated breeding value* (*EBV*), tramite cui si può stimare il miglioramento di un carattere per un certo riproduttore.

L’EBV viene misurato sperimentalmente attraverso le seguenti fasi:
1. Fecondazione di diversi individui in ambienti differenti con gameti del riproduttore in esame.
2. Misura dei fenotipi quantitativi d’interesse.
3. Confronto della media della prole del riproduttore $\micro_i$ con la [[Media di popolazione|Media di popolazione]] $\micro$.

Dato che la progenie potrebbe potenzialmente essere prodotta dall’unione del medesimo genotipo il breeding value è definito come il doppio della differenza fra la media della progenie e la media della popolazione:
$$EBV_i = 2(\micro_i - \micro)$$
In altri termini l’indice di performance della prole è un mezzo il breeding value del riproduttore.

Dato un [[Gene|Gene]] con due [[Allele|Alleli]], + e -, si ottiene — introducendo la formula della [[Media di popolazione|Media di popolazione]] e semplificando i vari termini — che l’EBV è pari a:
$$\begin{align*}
EBV_i^{++} &= 2q\alpha\\
EBV_i^{+-} &= (q-p)\alpha \\
EBV_i^{--} &= -2q\alpha\\
\end{align*}$$
Dove $\alpha$ è l’[[Effetto medio di un allele|Effetto medio dell’allele]].