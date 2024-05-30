---
aliases: Campionamento,
share: true
---

Il *campionamento statistico* è il processo di selezione ed estrazione di unità statistiche da una [[Popolazione statistica|Popolazione statistica]] per ottenere un [[Campione statistico|campione]] rappresentativo in cui sia possibile studiarne determinate [[Statistica campionaria|Statistiche campionarie]] e, tramite l’[[Inferenza statistica|Inferenza statistica]], trarre conclusioni ([[Parametro statistico|parametri]]) valide e applicabili all’intera popolazione.

Vi sono differenti metodi di campionamento:
- *campionamento casuale semplice*: ogni elemento della popolazione ha la medesima probabilità di essere scelto e questa non è influenzata dalle scelte precedenti. È il campionamento più naturale e utilizzato;
- *campionamento stratificato*: la popolazione è suddivisa in sottopopolazioni (*strati*) omogenee in cui ogni elemento ha la medesima probabilità di essere estratto, quindi viene applicato il campionamento casuale semplice a ogni strato;
- *campionamento clusterizzato*: la popolazione viene suddivisa in gruppi (*cluster*) eterogenei e uno (o più) di questi è scelto casualmente come campione;
- *campionamento sistematico*: la popolazione è suddivisa in $k$ gruppi con $n$ individui e si sceglie, randomicamente, un gruppo da cui tutti gli individui faranno parte del campione statistico. Dato il *passo di campionamento* $k=\frac{N}{n}$ si sceglie ogni $k$-esimo elemento, a eccezione del primo che è scelto fra 1 e $k$.

> [!example]- Esempio campionamento sistematico
> Data una popolazione $N=3000$ e un campione $n=100$, il passo di campionamento è $k=\frac{N}{n}=\frac{3000}{100}=30$.
> Si estrae casualmente la prima unità del campione fra 1 e $k$ (30): 15.
> Le successive unità saranno $15+k, 15+2k, 15+3k, \cdots, 15+(n-1)k$ ottenendo un campione di $n=100$.