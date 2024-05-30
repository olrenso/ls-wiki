---
aliases: Profondità critica
share: true
---
L’*altezza critica* $k$ è l’altezza di una [[Corrente idraulica|Corrente fluida]] che segna il passaggio da un flusso subcritico a un flusso supercritico, ossia l’altezza dove il [[Numero di Froude|Numero di Froude]] eguaglia l’unità.

Data l’altezza critica come il punto di minor [[Energia rispetto al fondo|Energia rispetto al fondo]] è possibile ricavare il valore di questa annullando la [[Derivata|Derivata]] prima dell’energia in funzione dell’altezza:
$$e(h)' = 0$$

Data una [[Corrente a pelo libero|Corrente a pelo libero]] in [[Regime di moto|Regime di moto]] permanente, quindi [[Portata volumetrica|Portata volumetrica]] costante, e sezione rettangolare l’[[Energia rispetto al fondo|Energia totale specifica]] è pari a:
$$e=h+\frac{v^2}{2g}=h+\frac{Q^2}{2gA^2} = h+\frac{Q^2}{2g(bh)^2}$$
La cui derivata, posta a zero, è:
$$\begin{align*}
h+\frac{Q^2}{2g(bh)^2}\;\frac{d}{dh} = 0\\
h\;\frac{d}{dh} + \frac{Q^2}{2gb^2}\frac{1}{h^2}\;\frac{d}{dh}=0\\
1 + \frac{Q^2}{2gb^2}\cdot\left(-\frac{2}{h^3}\right)=0\\
1-\frac{Q^2}{gb^2h^3}=0
\end{align*}$$

Ovvero l’altezza critica si ricava da:
$$\begin{align*}
1&=\frac{Q^2}{gb^2h^3}\\
k = h&= \sqrt[3]{\frac{Q^2}{gb^2}}
\end{align*}$$



È altresì possibile calcolare l’altezza libera dall’[[Equazione di continuità|Equazione di continuità]].
Date le medesime premesse fatte sopra, la portata $Q$ è data dal prodotto fra la velocità critica $v_c$ e l’area, a sua volta pari al prodotto fra base $b$ e altezza critica $k$:
$$Q = v_c\cdot bk$$
Dato che in condizioni critiche la velocità del fluido corrisponde alla velocità di propagazione delle perturbazioni, e quindi alla [[Celerità di un onda|Celerità delle onde]] ($v_c = \sqrt{gk}$), l’equazione di continuità diventa:
$$Q=\sqrt{gk}\cdot bk$$
Risolvendo per l’altezza critica $k$ si ottiene:
$$k = \sqrt[3]{\frac{Q^2}{gb^2}}$$

Data $v_c=\sqrt{gk}$ e $e_c = k+\frac{{v_c}^2}{2g}$, si ricava che, in condizioni critiche, l’[[Energia rispetto al fondo|Energia rispetto al fondo]] è uguale a:
$$e_c = k+\frac{\left(\sqrt{gk}\right)^2}{2g} = k+\frac{1}{2}k = \frac32k$$