---
share: true
---
La *viscosità dinamica* μ è la [[Viscosità|Viscosità]] di un [[Fluido|Fluido]] in presenza di uno [[Sforzo di taglio|sforzo tangenziale]] dovuto alla differente [[Velocità|Velocità]] degli strati adiacenti del fluido stesso.
$$\micro = \tau \frac{\partial y}{\partial v} = \frac{F}{A}\frac{\partial y}{\partial v}$$

Viene espressa in Poiseuille ($\text{Pl} = \ce{N s m^{-2}}$).

Dato un fluido in flusso alla Couette, ossia un [[Regime laminare|Flusso laminare]] fra due piastre parallele, di cui una fissa e la seconda in movimento con una velocità costante $v$[^1], si osserva una variazione lineare della velocità da $v$ a $0$ procedendo dalla piastra in movimento a quella stazionaria.

Ogni lamina di fluido si muove quindi a una velocità maggiore rispetto a quella inferiore generando una [[Resistenza fluidodinamica|Resistenza fluidodinamica]] che tenderà a rallentare la lamina superiore e trascinare la lamina inferiore.
Le due forze che si generano — uguali e opposte secondo la [[Terza legge di Newton|Terza legge di Newton]] — danno origine a uno [[Sforzo di taglio|Sforzo di taglio]] $\tau$.

Affinchè la velocità $v$ della piastra in movimento resti costante è necessaria una forza $F$ esterna, proporzionale alla velocità $v$ e all’area $A$ della piastra e inversamente proporzionale alla distanza di separazione $y$ rispetto alla piastra fissa ($F \propto \frac{v\cdot A}{y}$), in cui la costante di proporzionalità è rappresentata dalla viscosità dinamica $\micro$:
$$F = \micro \cdot A \frac{v}{y}$$

Dato $\tau = \frac{F}{A}$ si ottiene:
$$\micro = \tau\cdot \frac{v}{y}$$

![|400](94c07f1f737005edac65a6acdba3d7fa_MD5%201.png)

Nel caso in cui il gradiente di velocità non sia lineare la relazione della viscosità dinamica viene generalizzata in:
$$\micro = \tau \frac{\partial y}{\partial v}$$

![|200](b7c2bd6c965769985c93f7ef603f8b65_MD5%201.png)


[^1]: La cui velocità è sufficientemente bassa da non causare un [[Regime turbolento|Flusso turbolento]].