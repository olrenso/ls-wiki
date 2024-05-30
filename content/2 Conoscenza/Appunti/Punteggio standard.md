---
aliases:
  - Valore standardizzato
  - Punto Z
  - Punteggio Z
  - Normalizzazione
  - Variabile aleatoria normale standard
  - Standardizzazione
share: true
---
Il *punteggio standard* o *punteggio Z* è la distanza dalla [[Media aritmetica|Media]] di un valore $x$ appartenente a una [[Variabile aleatoria|Variabile stocastica]] $X\sim\mathcal{N}(\micro_X,\sigma_X^2)$ espresso in [[Deviazione standard|deviazioni standard]].

Il procedimento per il calcolo del valore Z è detto *standardizzazione*. Esso consiste nel ricondurre una [[Variabile aleatoria|Variabile casuale]] $X$, distribuita secondo una [[Distribuzione normale|Distribuzione normale]] con una certa [[Media aritmetica|Media]] $\micro_X$ e una certa [[Deviazione standard|Deviazione standard]] $\sigma_X$ a una variabile casuale $Z$ distribuita secondo una [[Distribuzione normale standard|Distribuzione normale standard]] ($\micro_Z=0,\sigma_Z=1$)[^2]. 

[^2]: $Z\sim\mathcal{N}(0,1)$

$$Z =\frac{X-\micro_X}{\sigma_X}$$

> [!note]- Dimostrazione di $Z=\frac{X-\micro_X}{\sigma_X}$
>Sia $X$ una variabile stocastica con un dato [[Valore atteso|Valore atteso]] $\mathbb{E}[X]=\micro_X$ e una data [[Varianza|Varianza]] $\sigma_X^2$.
> Si vuole trasformare linearmente $X$ in una nuova variabile $Z$ tale che $\micro_Z = 0$ e $\sigma_Z^2 = \sigma_Z = 1$:
> $$Z = a+bX \qquad \small z(x)$$
> Date le seguenti equazioni per il calcolo della media e della varianza di una variabile trasformata linearmente:[^1]
> $$\micro_Z = a+b\micro_X \qquad\text{e}\qquad \sigma_Z^2 = b^2\sigma_X^2$$
> E dato che  $\micro_Z = 0$ e $\sigma_Z = 1$:
> $$\begin{cases}
\micro_Z = a+b\micro_X = 0\\
\sigma_Z = b\sigma_X = 1\\
\end{cases}$$
> Da cui, risolvendo il sistema, si ottiene che le costanti $a$ e $b$ sono pari a:
> $$
\begin{cases}
a = -b\micro_X = -\frac{\micro_X}{\sigma_X}\\
b = \frac{1}{\sigma_X}\\
\end{cases}$$
> 
> Sostituendo quindi $a$ e $b$ alla funzione $z(x)$ si ottiene:
> $$Z = -\frac{\micro_X}{\sigma_X} + \frac{1}{\sigma_X}X = \frac{X-\micro_X}{\sigma_X}$$
> 
> [^1]:  Data $z(x)=a+bx$, dove $x$ è un possibile valore di $X$, si possono ricavare le due formule riportate applicando la definizione di [[Valore atteso|Valore atteso]] e di [[Varianza|Varianza]] probabilistica: $\micro_Z = \mathbb{E}[z(x)]$ e  $\sigma_Z^2 = \mathbb{E}[(z(x)-\micro_Z)^2]$.

Quando si lavora con un [[Campione statistico|Campione statistico]] la formula diventa:
$$Z = \frac{X-\overline{x}}{S}$$
Dove $X$ è il valore della variabile, $\overline{x}$ la [[Media aritmetica|Media]] campionaria e $S$ la [[Deviazione standard|Deviazione standard]] campionaria.

![[Pasted image 20240210080158.png|350]]

Trasformando linearmente una variabile $X$ nella relativa variabile $Z$ standard è possibile calcolare, mediante la [[Funzione di ripartizione|Funzione di ripartizione]] tabulata ($F(z)=P(Z\leq z)$[^3]), una data probabilità nella [[Distribuzione normale|Distribuzione normale]] originaria.

[^3]: Oppure, in base alla fonte, $F(z) = P(Z\geq z)$.

Sia $X\sim\mathcal{N}(\micro_X,\sigma_X)$, sia $Z\sim\mathcal{N}(0,1)$, data $F(z)$ la funzione di ripartizione di $Z$ e dati due valori $a$ e $b$ tali che $a<b$, la probabilità che $X$ sia compresa fra $a$ e $b$ è:
$$\begin{align}
p(a<X<b) &= P(\frac{a-\micro_X}{\sigma_X}<Z<\frac{b-\micro_X}{\sigma_X})=\\
&= F(\frac{b-\micro_X}{\sigma_X})-F(\frac{a-\micro_X}{\sigma_X})
\end{align}$$


> [!example]- Esempi di calcoli delle probabilità di una variabile $X\sim\mathcal{N}(\micro_X,\sigma_X^2)$
> Sia $X$ una [[Variabile aleatoria|Variabile aleatoria]] che segue una [[Distribuzione normale|Distribuzione normale]] con $\micro_X=5$ e $\sigma_X^2=4$ ($\sigma_X = 2$) e sia $Z\sim\mathcal{N}(0,1)$ con funzione di ripartizione $F(z)$.
> 
> Dati i seguenti valori di $X$: $\displaystyle x_1 = 7; x_2 = 5; x_3 = 1$
> I relativi punteggi Z sono: $\displaystyle z_1= \frac{7-5}{2}=1.5 \quad z_2= \frac{5-5}{4}=0 \quad z_3=\frac{1-5}{2}=-2$
> 
> Dati i valori tabulati si può affermare che la probabilità che $Z\leq z_1$ è $F(1.5)=0.9332$ (riga 1.5; colonna 0) e, per definizione, che la probabilità che $X\leq x_1$ è $0.9332$.
> Analogamente la probabilità $p(Z\leq z_2)=p(X\leq x_2) = F(0) = 0.5$ (riga 0; colonna 0).
> 
> Per $z_1$, che ha valore negativo ma nella tabella sono riportati solo valori positivi, dato che la curva è simmetrica, vale: $F(-z)=1-P(Z\leq -(-z))=1-P(Z\leq z)$
> 
> Quindi: $p(Z\leq z_3) = p(X\leq x_3)= 1-p(Z\leq -z_3) = 1-p(Z\leq 2) = 1- F(2) = 1-0.9772 = 0.0228$
> 
> Inoltre, per ottenere la probabilità che il valore di $X$ sia nell’intervallo $[x_2,x_1]$:
> $p(x_2\leq X \leq x_1) = p(z_2 \leq Z \leq z_1) = p(0 \leq Z \leq 1.5)$
> Vale: $p(0 \leq Z \leq 1.5) = p(Z\leq1.5)-p(Z\leq0) = F(1.5) - F(0) = 0.9332 - 0.5 = 0.4332$
> 
> Da cui la probabilità che *non* sia nell’intervallo $[x_2,x_1]$: $p'=1-0.4332 = 0.5668$
> 
> Infine può essere utile trovare il valore limite di $X$ data una probabilità cumulata $p$. Per esempio: per sapere entro che valore di $X$ si ha il 90% di probabilità $F(z) = 0.9 \rightarrow z=1.29$
> E di conseguenza: $z=\frac{x-5}{2}=1.29 \rightarrow x = 1.29\cdot 2 + 5 = 7.58$

> [!tldr]- Valori tabellari della funzione di ripartizione
> La tabella riporta i valori della funzione $F(z) = P(Z\leq z)$
> ![[Pasted image 20240209192545.png|Pasted image 20240209192545.png]]