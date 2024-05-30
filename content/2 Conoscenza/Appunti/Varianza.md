---
share: true
---
La *varianza*, $\sigma^2_X$ o $\text{Var}(X)$, di una [[Variabile statistica|Variabile statistica]] o [[Variabile aleatoria|aleatoria]] $X$ è una misura del grado di variabilità dei valori assunti dalla variabile; più precisamente è una misura di quanto i valori si discostano dalla [[Media aritmetica|Media]] o dal [[Valore atteso|Valore atteso]].

Dalla radice quadrata della varianza si ottiene la [[Deviazione standard|Deviazione standard]].
###### Statistica
Statisticamente la varianza è un [[Misura di dispersione|Indice di dispersione]] che esprime la deviazione di delle osservazione dal valore atteso.
Data la [[Distribuzione statistica|Distribuzione statistica]] di una [[Variabile statistica|Variabile]] (più precisamente un [[Parametro statistico|parametro]]) $X$ in una popolazione di $N$ elementi, la varianza è la [[Media aritmetica|Media aritmetica]] del quadrato degli scarti delle osservazioni dalla loro media.
$$\sigma^2_X = \frac{\sum\limits_{i=1}^n(x_i-\micro_X)^2}{N}$$
Dove:
- $x_i$ è il valore dell’osservazione;
- $\micro_X$ è il valore medio, accettato o atteso;
- $N$ è il numero delle osservazioni (la numerosità della popolazione).

Laddove i dati provengano da un [[Campione statistico|Campione statistico]] si impiega la [[Varianza campionaria|Varianza campionaria]] ($S_X^2$) come [[Stimatore|Stimatore]].

###### Probabilità
Dal punto di vista probabilistico è definita come il [[Valore atteso|Valore atteso]] (ossia la media ponderata) del quadrato dello scarto di ogni valore di $X$ rispetto al valore atteso $\mathbb{E}[X]$ :
$$\sigma_X^2=\mathbb{V}ar[X]=\mathbb{E}\Big[(X-\mathbb{E}[X])^2\Big] =\mathbb{E}\Big[(X-\micro_X)^2\Big]$$
Che in base al tipo di variabile (discreta o continua) diventa:
$$\overset{\text{Variabile discreta}}{
\begin{align}
\mathbb{V}ar[X] &= {\textstyle\sum_{i=1}^\infty} (x_i-\mathbb{E}[X])^2P_X(x_i)=\\
&={\textstyle\sum_{i=1}^\infty} (x_i-\micro_X)^2P_X(x_i)
\end{align}
}
\qquad\qquad
\overset{\text{Variabile continua}}{
\begin{align}
\mathbb{V}ar[X] &= \mathbb{E}[X^2]-(\mathbb{E}[X])^2=\\
&=\mathbb{E}[X^2]-\micro_X^2
\end{align}
}$$
In cui:
- $\mathbb{E}[X]$ è il [[Valore atteso|Valore atteso]] o media $\micro_X$;
- $x_i$ è l’$i$-esimo valore assunto da $X$;
- $P_X(x_i)$ è la [[Funzione di probabilità|Funzione di probabilità]] di $X$;
- $\mathbb{E}[X^2]$ è il [[Valore atteso|Valore atteso]] della funzione $g(X)=X^2$.


In caso la [[Variabile aleatoria|Variabile aleatoria]] sia discreta la formula sopra riportata si semplifica:
$$\sigma_X^2= \sum_{i=1}^\infty \Big(x_i^2P_X(x_i) \Big) -\micro_X^2$$

> [!note]- Dimostrazione formula ridotta
> Nota la definizione probabilistica della varianza:
> $$\begin{align}
\sigma_X^2&= \sum_{i=1}^\infty (x_i-\micro_X)^2P_X(x_i)=\sum_{i=1}^\infty (x_i^2 - 2\micro_Xx_i +\micro_X^2)P_X(x_i)=\\[1.5ex]
&=\sum_{i=1}^\infty x_i^2P_X(x_i)-2\micro_X\sum_{i=1}^\infty x_iP_X(x_i) + \micro_X^2\sum_{i=1}^\infty P_X(x_i)
\end{align}$$
> E dato che:
> $$\sum_{i=1}^\infty x_iP_X(x_i) = \micro_X \qquad\text{e}\qquad \sum_{i=1}^\infty P_X(x_i) = 1$$
> Si ottiene:
> $$\begin{align}
\sigma_X^2 &= \sum_{i=1}^\infty x_i^2P_X(x_i) - 2\micro_X\cdot\micro_X + \micro_X^2=\\[1.5ex]
&=\sum_{i=1}^\infty x_i^2P_X(x_i) - \micro_X^2
\end{align}$$
