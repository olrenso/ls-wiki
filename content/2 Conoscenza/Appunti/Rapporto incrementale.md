---
share: true
---
Il *rapporto incrementale* è il rapporto fra l’incremento subito dalla $y$ e l’incremento fornito sull’asse delle $x$:

$$\frac{f(x+\Delta x) - f(x)}{(x+\Delta x)- x} = \frac{f(x+\Delta x) - f(x)}{\Delta x}$$

Ovvero il coefficiente angolare della [[Funzioni Lineari|Retta]] secante fra il punto $(x,f(x))$ e $(x+\Delta x, f(x+\Delta x))$.

Quando $\Delta x$ tende a $0$ si parla di *rapporto infinitesimale* e il coefficiente angolare assume il valore del coefficente angolare della tangente nel punto $(x,f(x))$, ovvero la [[Derivata|Derivata]] prima:
$$m_{tan} = \lim_{\Delta x \rightarrow0}{\frac{f(x+\Delta x)-f(x)}{\Delta x}} = \frac{d f(x)}{dx} = f'(x)$$