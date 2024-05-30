---
share: true
---
Schema risolutivo:
1. Creazione di una tabella con moli (o concentrazioni) iniziali, all’equilibrio e la variazione fra queste due fasi
2. Sostituzione delle moli (o concentrazioni) ricavate dalla tabella nella formula della costante di equilibrio
3. Risoluzione dell’equazione di secondo grado a trovare la variazione di moli (o concentrazione)

![](ac454ee528e793422198f4670e70eef4_MD5%201.png)

Un aspetto importante è quello di prevedere, prima di iniziare a fare i calcoli, la direzione della reazione.

---

## Esercizio 1

> **Esercizio 1**
> In un reattore di 3L viene aggiunta una certa quantità di $\ce{N2O4_{(g)}}$ dove avviene la seguente reazione:
> $$\ce{N2O4_{(g)} <=> 2NO2_{(g)}}$$
> All’equilibrio esercita una pressione $P_{eq} = 6 \text{ atm}$, con una $T=55^\circ C$ e con una costante di equilibrio pari a $K_p = 0,66$.
> Calcolare:
> a) Il grado di dissociazione $\alpha$
> b) La quantità iniziale di $\ce{N2O4}$

---


Si crea prima di tutto una tabella riassuntiva dello stato iniziale e dell’equilibrio del sistema:

|                | $\ce{N2O4}$ | $\ce{NO2}$ |
| -------------- |:-----------:|:----------:|
| Stato iniziale |    $n_0$    |     0      |
| Variazione     |   $-n_d$    |  $+2n_d$   |
| Equilibrio     | $n_0 - n_d$ |   $2n_d$   |

Dove $n_d$ è la quantità dissociata e $n_0$ la quantità totale, il cui rapporto da il [[Grado di dissociazione|Grado di dissociazione]]:
$$\alpha = \frac{n_d}{n_0}$$

Sappiamo inoltre che la [[Costante di equilibrio|Costante di equilibrio]] è uguale a:
$$K_p = \frac{(p_\ce{NO2})^2}{p_\ce{N2O4}} = 0,66$$

Dal grado di dissociazione si può ricavare la frazione molare dei componenti del sistema:
$$\chi_\ce{NO2} = \frac{2n_d}{n_0-n_d+2n_d} \qquad \qquad \chi_\ce{N2O4} = \frac{n_0-n_d}{n_0-n_d+2n_d}$$
Che si possono semplificare come segue:
$$\begin{align*}
&\chi_\ce{NO2} = \frac{2\alpha \cdot n_0}{n_0(1 + \alpha)} = \frac{2\alpha}{1+\alpha}\\[1em]
&\chi_\ce{N2O4} = \frac{n_0(1-\alpha)}{n_0(1+\alpha)} = \frac{1-\alpha}{1+\alpha}
\end{align*}$$


Avendo le frazioni molari e la pressione totale all’equilibrio possiamo ricavare le pressioni parziali.
Dalla [[Legge di Dalton|Legge di Dalton]] le pressioni parziali sono uguali al prodotto della pressione totale per la frazione molare ($p_i = \chi_i \cdot P$):

$$p_\ce{NO2} = \chi_\ce{NO2} \cdot P_{eq} = \frac{2\alpha}{1+\alpha} \cdot 6 \text{ atm} \qquad p_\ce{N2O4} = \chi_\ce{N2O4} \cdot P_{eq} = \frac{1-\alpha}{1+\alpha} \cdot 6 \text{ atm}$$
Sostituendo le pressioni parziali alla formula della costante d’equilibrio $K_p$ si può ricavare il grado di dissociazione $\alpha$.
$$\begin{align*}
&K_p = \left(\frac{2\alpha\cdot6}{1+\alpha}\right)^2 \cdot \frac{1 + \alpha}{6\cdot(1- \alpha)} = 0,66\\[1em]
&\frac{144\alpha^2}{(1+\alpha)^2} \cdot \frac{1 + \alpha}{6\cdot(1- \alpha)} = 0,66\\[1em]
&\frac{24\alpha^2}{1+\alpha} \cdot \frac{1}{1-\alpha} = 0,66\\[1em]
&24\alpha^2=0,66\cdot(1+\alpha)(1-\alpha)\\[1em]
&24\alpha^2=0,66-0,66\alpha^2\\[1em]
&24,66\alpha^2=0,66\\[1em]
&\alpha=\sqrt{\frac{0,66}{24,66}} = 0,163
\end{align*}$$

Si possono ricavare le moli di sostanta all’equilibrio applicando l’[[Legge dei gas perfetti|Equazione di stato dei gas perfetti]] $PV=nRT$.

$$n_\text{tot}=\frac{PV}{RT} = \frac{6\text{ atm} \cdot 3\text{ L}}{0,08206 \ce{\frac{atm\cdot L}{mol\cdot K}}\cdot (55+273,15)\text{ K}} = 0,668 \text{ mol}$$
E sapendo il grado di dissociazione risalire alle moli di tetraossido di diazoto inizialmente presenti:
$$\begin{align*}
&n_\text{tot} = n_\ce{N2O4} + n_\ce{NO2} = n_0-n_d+2n_d = n_0+n_d = n_0+n_0\cdot\alpha = n_0\cdot(1+\alpha)\\[1.5em]
&0,668\text{ mol} = n_0 \cdot (1+0,163)\\[1em]
&n_0 = \frac{0,668\text{ mol}}{1,163} = 0,574 \text{ mol} 
\end{align*}$$
E infine si possono ricavare i grammi di $\ce{N2O4}$:
$$\text{m} = n \cdot MM = 0,574 \text{ mol} \cdot 92\ce{\frac{g}{mol}} = 53\text{ g}$$


---

## Esercizio 2

> **Esercizio 2**
> Data la reazione $$\ce{CO_{(g)} + H2O_{(g)} \rightleftarrows CO2_{(g)} + H2_{(g)}}$$
> Sapendo cha la costante di equilibrio $K_c$ è di $0,58$ a $1000 \; ^\circ \text{C}$, introducendo una mole di ciascun reagente in un pallone di $50,0 \text{ L}$ come varia l’equilibrio?

---
Avendo le moli e il volume della miscela gassosa si può ricavare la concentrazione dei reagenti come segue:
$$\ce{[CO] = [H2O]} = \frac{1 \text{ mol}}{50 \text{ L}} = 0,02 \text{ M}$$
Nota la concentrazione si costruisce la tabella:


|                    | $\ce{CO}$ | $\ce{H2O}$ | $\ce{CO2}$ | $\ce{H2}$ |
| ------------------ |:---------:|:----------:|:----------:|:---------:|
| **Stato iniziale** |   0,02    |    0,02    |     0      |     0     |
| **Variazione**     |    -x     |     -x     |     +x     |    +x     |
| **Equilibrio**     | 0,02 - x  |  0,02 - x  |     +x     |    +x     |

Sostituendo le concentrazioni all’equilibrio alla formula per la costante di equilibrio si ottiene la seguente equazione di secondo grado:
$$K_c = \ce{\frac{[CO2][H2]}{[CO][H2O]}} \rightarrow 0,58=\frac{(x)(x)}{(0,02-x)(0,02-x)}$$
$$\frac{x^2}{(0,02-x)^2} = 0,58 \longrightarrow \sqrt{\frac{x^2}{(0,02-x)^2}} = \sqrt{0,58}$$
Ovvero:
$$ \frac{x}{0,02-x}= \pm 0,76$$
Da cui si ricava $x_1= -0,063$, non accettabile fisicamente e $x_2=0,0086$, il valore accettato e che consente di calcolare le seguenti concentrazioni all’equilibrio:
$$\begin{align*}
&\ce{[CO]} = \ce{[H2O]} = 0,02 \text{ M} -x = 0,02\text{ M} - 0,0086\text{ M} = 0,0114 \text{ M}\\
&\ce{[CO2]} = \ce{[H2]} = x = 0,0086 \text{ M}
\end{align*}$$