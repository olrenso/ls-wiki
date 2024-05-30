---
aliases:
  - Test di verifica d'ipotesi della correlazione lineare
share: true
---

Il *test d’ipotesi della correlazione lineare* è un [[Test di verifica d'ipotesi|Test di verifica d'ipotesi]] basato sul [[Indice di correlazione di Pearson|Coefficiente di correlazione di Pearson]] per verificare la presenza di una correlazione lineare fra due [[Variabile statistica|Variabili statistiche]].

Segue una [[Distribuzione t di Student|Distribuzione t di Student]] e si basa sui seguenti presupposti:
- le variabili sono numeriche;
- almeno una delle variabili segue una [[Distribuzione normale|Distribuzione normale]], in caso contrario si può usare il [[Spearman's rank correlation coefficient|Coefficiente di correlazione per ranghi di Spearman]];
- entrambe le variabili devono approssimare la [[Distribuzione normale|Curva di Gauss]] se si vuole calcolare l’[[Intervallo di fiducia|Intervallo di confidenza]].

La [[Statistica test|Statistica test]] è determinata dall’equazione:
$$\rho\text{-test}=r\sqrt{\frac{n-2}{1-r^2}}\quad{\small\text{con } n-2\text{ GdL}}$$
Dove $r$ è il [[Indice di correlazione di Pearson|Coefficiente di correlazione lineare]] (del campione) e $n$ il numero di individui (o di coppie di osservazioni).

Per calcolare l’[[Intervallo di fiducia|Intervallo di fiducia]] è necessario trasformare la [[Distribuzione campionaria|Distribuzione campionaria]] di $r$ in una [[Distribuzione normale standard|Distribuzione normale standard]]:
$$z=0.5\ln\left(\frac{1+r}{1-r}\right)$$
Da cui si calcolano i valori limite della nuova variabile $z$:
$$\text{CI}_{z\;\gamma\%}=z\pm Z_\gamma\frac{1}{\sqrt{n-3}}$$
In cui $Z_\gamma$ è il [[Punteggio standard|Punteggio Z]] per la corrispondente significatività desiderata ($Z=1.96$ per $\text{CI}_{95\%}$).
Calcolati $z_1$ e $z_2$ (limite inferiore e superiore) si calcolano i limiti dell’intervallo di $r$ attraverso la trasformazione inversa $r=\displaystyle\small\frac{e^{2z}-1}{e^{2z}+1}$:
$$r_1 = \frac{e^{2z_1}-1}{e^{2z_1}+1} \quad r_2=\frac{e^{2z_2}-1}{e^{2z_2}+1}$$

> [!note]- Dimostrazione trasformazione inversa $z\rightarrow r$
> 
>$$\begin{align}
z&=\frac{1}{2}\ln\frac{1+r}{1-r}\\[1.5ex]
2z&=\ln(1+r)-\ln(1-r)\\
e^{2z} &= e^{\ln(1+r)-\ln(1-r)}\\
e^{2z} &= \frac{e^{\ln(1+r)}}{e^{\ln(1-r)}}\\
e^{2z} & = \frac{1+r}{1-r}\\
(1-r)e^{2z} &=1+r\\
e^{2z} -re^{2z}&=1+r\\
r+re^{2z} &= e^{2z}-1\\
r&=\frac{e^{2z}-1}{e^{2z}+1}
\end{align}$$

> [!example]- Esempio pratico
> Si è sviluppata una nuova tecnica per la misurazione dell’attività dell’enzima BAP (bone alkaline phosphatase) e si vuole verificare se questa misura (wBAP) è correlata con un indicatore indipendente della formazione ossea (PICP, collagen Type I carboxy-terminal propeptide).
> Le osservazioni svolte su 46 cavalli sono riportate nella tabella che segue e visualizzate graficamente in un grafico a dispersione con assi logaritmici (al fine di ottenere una distribuzione normale).
> 
> | wBAP (µg/l) | PICP (U/l) | wBAP (µg/l) | PICP (U/l) | wBAP (µg/l) | PICP (U/l) |
> |:-----------:|:----------:|:-----------:|:----------:|:-----------:|:----------:|
> |     20      |    190     |     30      |    400     |     52      |    1005    |
> |     31      |    186     |     36      |    380     |     61      |    1100    |
> |     31      |    190     |     50      |    405     |     61      |    1070    |
> |     22      |    205     |     54      |    370     |     57      |    810     |
> |     18      |    210     |     31      |    490     |     59      |    720     |
> |     16      |    290     |     35      |    470     |     63      |    740     |
> |     18      |    306     |     39      |    470     |     65      |    700     |
> |     55      |    1000    |     36      |    580     |     62      |    750     |
> |     28      |    170     |     36      |    540     |     61      |    700     |
> |     32      |    180     |     40      |    520     |     70      |    570     |
> |     33      |    300     |     36      |    700     |     71      |    1300    |
> |     38      |    303     |     34      |    800     |     88      |    1050    |
> |     34      |    320     |     41      |    800     |     90      |    1100    |
> |     21      |    360     |     48      |    850     |     90      |    1200    |
> |     41      |    340     |     50      |    980     |     110     |    940     |
> |             |            |             |            |     34      |    360     |
> 
> ![[Pasted image 20240217080008.png|400]]
> 
> 1. L’ipotesi nulla afferma che non vi è correlazione fra le due variabili $H_0 : \rho=0$; l’ipotesi alternativa che vi sia una correlazione lineare $H_1:\rho\neq0$.
> 2. Osservando il grafico di dispersione si può intuire una certa correlazione lineare; grafici separati di $\log \text{wBAP}$ e $\log \text{PICP}$ mostrano che le due variabili trasformate seguono una [[Distribuzione normale|Distribuzione normale]]. Si può calcolare il [[Indice di correlazione di Pearson|Coefficiente di correlazione di Pearson]]: $r=0785$.
> 3. La [[Statistica test|Statistica test]] fornisce come valore: $$\rho\text{-test}=0.785\sqrt{\frac{44}{0.3838}}=8.41$$
> 4. Un valore di $8.41$ corrisponde a un [[Valore p|p-value]] $<0.001$.
> 5. Vi è una forte evidenza per poter rifiutare l’ipotesi nulla e confermare una correlazione lineare fra le due variabili.
> 6. L’[[Intervallo di fiducia|Intervallo di fiducia]] è compreso fra $0.64$ e $0.88$: $$\begin{align}z_{1,2} &= 0.5\ln\frac{1.7846}{0.2154}\pm1.96\frac{1}{\sqrt{43}}=0.7583;1.3561\\[2ex]r_1&=\frac{e^{1.5166}-1}{e^{1.5166}+1}=0.64\quad r_2=\frac{e^{2.7122}-1}{e^{2.7122}+1}=0.88\end{align}$$