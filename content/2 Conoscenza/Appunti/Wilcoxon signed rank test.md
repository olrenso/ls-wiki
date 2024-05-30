---
share: true
---

Il *wilcoxon signed rank test* è un [[Test di verifica d'ipotesi|Test di verifica d'ipotesi]] non parametrico analogo al [[Paired t-test|Paired t-test]].

Per ogni individuo viene calcolata la differenza fra le osservazioni e, in base al valore assoluto della differenza, classificati in ordine crescente.
Si calcola quindi la [[Statistica test|Statistica test]]:

$$\text{test}_{n>25} = \frac{T -n\frac{n+1}{4}}{\sqrt{\displaystyle\small n(n+1)\frac{2n+1}{24}}}\qquad\qquad\text{test}_{n\leq25}=T$$

In cui $T$ è la somma di tutte le differenze positive ($T_+$) o di tutte le differenze negative ($T_-$) — solitamente la minore fra le due.
La statistica test per campioni di ampiezza $n>25$ segue la [[Distribuzione normale standard|Distribuzione normale standard]].

> [!example]- Esempio pratico
> Una nuova dieta per ratti da laboratorio viene esaminata per valutare il tasso di crescita ponderale.
> Per ogni individuo a cui è somministrata la nuova dieta è associato un secondo individuo, dello stesso sesso e proveniente dalla medesima cucciolata, a cui è somministrata una seconda dieta di controllo.
> Dopo 60 giorni le coppie sono state pesate e i dati ottenuti sono riportati nella tabella seguente.
> 
> | Coppia individui | Peso dieta test (g) | Peso dieta controllo (g) | Differenza (controllo - test) (g) | Rango della diff |
> | :--------------: | :-----------------: | :----------------------: | :-------------------------------: | :--------------: |
> |        1         |         243         |           265            |                22                 |        15        |
> |        2         |         161         |           165            |                 4                 |       5.5        |
> |        3         |         318         |           361            |                43                 |        16        |
> |        4         |         270         |           270            |                 0                 |        -         |
> |        5         |         214         |           235            |                21                 |        14        |
> |        6         |         97          |            83            |                -14                |        11        |
> |        7         |         189         |           170            |                -19                |        13        |
> |        8         |         151         |           158            |                 7                 |       9.5        |
> |        9         |         143         |           143            |                 0                 |        -         |
> |        10        |         117         |           121            |                 4                 |       5.5        |
> |        11        |         177         |           174            |                -3                 |       3.5        |
> |        12        |         204         |           211            |                 7                 |       9.5        |
> |        13        |         190         |           192            |                 2                 |       1.5        |
> |        14        |         134         |           131            |                -3                 |       3.5        |
> |        15        |         154         |           160            |                 6                 |        8         |
> |        16        |         273         |           291            |                18                 |        12        |
> |        17        |         126         |           131            |                 5                 |        7         |
> |        18        |         188         |           190            |                 2                 |       1.5        |
> 
> 1. L’ipotesi nulla dichiara che non vi è differenza fra l’accresimento ponderale nelle due diete $H_0: P_c=P_t$.
> 2. Una visualizzazione grafica dei dati (o un test formale) rivela che i dati non seguano una [[Distribuzione normale|Distribuzione normale]] e quindi non può essere applicato il [[Paired t-test|Paired t-test]].
> 3. Viene calcolata la differenza fra i pesi di ciascuna coppia e ordinata in ordine crescente. Valori identici ricevono un rango intermedio, per esempio vi sono due differenza pari a $4$, comprese fra il rango $4$ e il rango $7$. Invece di assegnare $5$ e $6$ si assegna $(5+6)/2=5.5$ a entrambe. Si calcola quindi la somma dei ranghi delle differenze negative (in quanto in questo caso $T_-<T_+$): $T_-=11+13+3.5+3.5 = 31$
> 4. In quando $n<25$ il valore della [[Statistica test|Statistica test]] è pari a $T_-$. Il [[Valore p|Valore p]], ricavato dai valori critic tabulati per il wilcoxon signed rank test, è compreso fra 0.05 e 0.10 (precisamente è pari a 0.06).
> 5. Dato che P>0.05 non si può rifiutare l’ipotesi nulla e si può mettere in dubbio la capacità della nuova dieta di aumentare l’incremento ponderale.


> [!tldr]- Valori critici tabulati per $n\leq25$
![[Pasted image 20240219090558.png|Pasted image 20240219090558.png]]