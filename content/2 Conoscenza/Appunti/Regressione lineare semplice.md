---
aliases:
  - Regressione lineare univariabile
share: true
---

La *regressione lineare semplice* o *univariabile* è un [[Regressione lineare|Modello di regressione lineare]] con un solo regressore (cioè una sola variabile indipendente); descrive quindi la correlazione fra due sole variabili.

Tale modello si basa su sei presupposti:
- la relazione fra $x$ e $y$ è lineare;
- $x$ è stata misurata senza errori;
- per ogni valore di $x$ i corrispondenti valori di $y$ nella popolazione sono [[Distribuzione normale|distribuiti normalmente]];
- per ogni valore di $x$ la [[Media aritmetica|Media]] di popolazione giace sulla retta della regressione;
- la varianza della popolazione per i valori di $y$ è costante per ogni valore di $x$;
- le osservazioni sono indipendenti, ossia ogni individuo è rappresentato una sola volta.

L’equazione di una regressione lineare semplice assume la tipica forma di una retta:
$$Y_\text{pop}=\alpha + \beta x$$
In cui:
- $Y_\text{pop}$ è il valore previsto, atteso o medio di $y$ per un dato valore di $x$;
- $\alpha$ è una costante che determina il punto d’intersezione con l’asse verticale; ovvero il valore di $y$ quando $x=0$;
- $\beta$ è il coefficiente angolare, cioè il grado d’inclinazione della retta; indica la risposta di $y$ per ogni variazione unitaria di $x$.

$\alpha$ e $\beta$, detti coefficienti di regressione (della popolazione), sono stimati rispettivamente da $a$ e $b$ sulla base di $n$ osservazioni di un campione $\{(x_1,y_1)(x_2,y_2),\cdots,(x_n,y_n)\}$.
$$b=\frac{\sum(x-\overline{x})(y-\overline{y})}{\sum(x-\overline{x})^2}\quad\text{e}\quad a=\overline{y}-b\overline{x}$$
Da cui la retta di regressione lineare campionaria:
$$Y=a+bx$$

> [!example]- Esempio pratico
> Si vuole studiare la correlazione il peso e una seconda variabile più facilmente misurabile negli ovini in modo da poterne prevedere il peso.
> Sono state raccolte 66 coppie di misurazioni, da altrettanti animali, del peso (LW) e della circonferenza toracica (CG). I valori numerici sono illustrati nella tabella seguente.
> 
> | LW  | CG  | LW  | CG  | LW  | CG  | LW  | CG  | LW  | CG  | LW  | CG  |
> |:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
> | 30  | 76  | 20  | 63  | 28  | 77  | 29  | 73  | 18  | 62  | 19  | 67  |
> | 24  | 71  | 28  | 70  | 25  | 71  | 30  | 74  | 28  | 70  | 27  | 69  |
> | 20  | 63  | 22  | 65  | 27  | 72  | 21  | 64  | 27  | 71  | 31  | 74  |
> | 25  | 69  | 28  | 72  | 28  | 74  | 28  | 74  | 30  | 73  | 23  | 67  |
> | 25  | 67  | 25  | 67  | 25  | 65  | 48  | 89  | 28  | 72  | 22  | 63  |
> | 19  | 62  | 20  | 62  | 20  | 64  | 17  | 60  | 22  | 69  | 35  | 75  |
> | 35  | 77  | 35  | 78  | 35  | 78  | 46  | 86  | 48  | 90  | 44  | 84  |
> | 37  | 84  | 43  | 81  | 32  | 73  | 43  | 84  | 31  | 73  | 31  | 73  |
> | 39  | 78  | 36  | 81  | 33  | 80  | 44  | 82  | 39  | 80  | 45  | 86  |
> | 43  | 88  | 41  | 87  | 36  | 82  | 43  | 80  | 33  | 79  | 35  | 78  |
> | 38  | 78  | 36  | 76  | 35  | 74  | 39  | 81  | 34  | 74  | 39  | 76  |
> 
> Osservando il [[Grafico di dispersione|Diagramma di dispersione]] è evidente una correlazione lineare fra le due variabili.
> 
> La retta di regressione stimata, ottenuta da un software statistico, è $Y=-46.06+1.04x$. Per ogni incremento di un centimetro della circonferenza toracica il peso dell’animale aumenta, in media, di 1.04 chilogrammi.
> 
> ![[Pasted image 20240217083625.png|350]]![[Pasted image 20240217083911.png|350]]