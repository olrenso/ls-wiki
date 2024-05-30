---
aliases: Trasformazioni termodinamiche
share: true
---
Una *trasformazione termodinamica* è un processo fisico che comporta il passaggio fra due stati termodinamici in equilibrio mediante apporti o sottrazioni di energia, sotto forma di [[Calore|Calore]] o [[Lavoro|Lavoro]], all’interno di un [[Sistema termodinamico|Sistema termodinamico]].

Si utilizza abitualmente la convenzione in cui il calore trasferito è positivo quando entra nel sistema mentre negativo quando esce. Viceversa il lavoro è positivo quando è svolto dal sistema e negativo quando è compiuto dall’ambiente sul sistema stesso.

Il percorso fra i due stati in equilibrio di una trasformazione termodinamica può compiere infiniti possibili percorsi, da cui dipende la quantità di *lavoro termodinamico* svolto:
$$W = \int_i^f dW = \int_i^f p\;dV$$

Passando ciclicamente fra due stati termodinamici all’equilibrio svolgendo due differenti percorsi consente di compiere o svolgere [[Lavoro|Lavoro]], ottenendo una [[Macchina termica|Macchina termica]].

![|400](46f79365337dca6d5260cdda235a9a01_MD5%201.png)


Una trasformazione termodinamica può essere:
- *Isoterma*, $T$ costante, variano solo pressione e volume.
- *Isobara*, $P$ costante, variano solo temperatura e volume.
- *Isocora*, $V$ costante, variano solo pressione e temperatura.
- *Adiabatica*, $Q=0$, non avvengono scambi di calore.

Può essere inoltre considerata *reversibile* se avviene lentamente, quasi staticamente, e all’equilibrio termodinamico, ossia quando le variabili di stato del sistema sono uniformi, non ci sono reazioni chimiche e non ci sono forze disequilibrate; oppure *irreversibile* quando intervengono forze dissipative e non è possibile invertire la sua direzione — a causa dell’aumento di [[Entropia|Entropia]] —, se non svolgendo lavoro e aumentando l’entropia dell’ambiente.

Il lavoro svolto da un sistema termodinamico durante una trasformazione termodinamica è pari all’area sottesa dalla curva rappresentante la trasformazione in un grafico pressione–volume.
Di conseguenza per le reazioni reversibili si ottiene:

|       Isobara        | Isocora |                 Isoterma                 |
|:--------------------:|:-------:|:----------------------------------------:|
| $$W = p_A(V_B-V_A)$$ | $$W=0$$ | $$W=nRT\ln\left(\frac{V_B}{V_A}\right)$$ |

![](70192a5c5f076f40e6d478a02b28f6ab_MD5%201.png)

---
###### Dimostrazione isobara
Nota la definizione di lavoro come il prodotto scalare fra la forza e lo spostamento $W=Fd$, si può esprimere la forza esercitata come la pressione costante $p$ esercitata dal sistema su una superficie $S$:
$$W = Fd = pSd$$
Dove $Sd$ non è altro che la superficie per lo spostamento compiuto, ossia la variazione di volume fra lo stato iniziale $A$ e lo stato finale $B$:
$$W = p(V_B-V_A)$$

###### Dimostrazione isoterma
Dato che sia la pressione che il volume non sono costanti bisogna considerare variazioni infinitesimali in cui entrambe le variabili possono essere considerate costanti.
Su scala infinitesimale il lavoro sarà quindi pari a:
$$dW = F\cdot dx = pS\cdot dx = p\cdot dV$$
La pressione può perciò essere espressa, dalla [[Legge dei gas perfetti|Legge dei gas perfetti]], come $p=nRT \frac{1}{V}$, ottenendo che il lavoro, fra lo stato $A$ e lo stato $B$, è pari a:
$$\begin{align*}
dW &= nRT\frac{1}{V} \; dV \\
\int_{V_A}^{V_B} dW &= \int_{V_A}^{V_B} nRT\frac{1}{V}\;dV\\[2ex]
W &= nRT[\ln(V_B)-\ln(V_A)] =\\[1.5ex]
&=nRT\ln\left(\frac{V_B}{V_A}\right)
\end{align*}$$

Nel caso di un [[Gas ideali|Gas ideale]], dato il [[Primo principio della termodinamica|Primo principio della termodinamica]] $\Delta U = Q-W$ e $U = \frac{3}{2}nRT$, e dato che la temperatura è costante, il lavoro $W$ è pari al calore $Q$ assorbito dal sistema:
$$\begin{align*}
\Delta U &= \frac{3}{2}nRT_f - \frac{3}{2}nRT_i \quad\leftarrow\;\; T_f = T_i\\[2ex]
\Delta U &= 0 = Q-W \quad\Longrightarrow\quad Q= W
\end{align*}$$