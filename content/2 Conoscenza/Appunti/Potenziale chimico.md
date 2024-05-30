---
share: true
---
Il *potenziale chimico* $\micro$ di una specie chimica è l’[[Energia|Energia]] che può essere assorbita o rilasciata quando si verifica la variazione del numero di particelle di tale specie.

La differenza di potenziale chimico è alla base di tutte le reazioni chimiche, fisiche e dei movimenti dei soluti[^1] spontanei.
Una specie chimica tenderà sempre a passare da una situazione di alto potenziale chimico, ossia con un’elevata [[Energia libera di Gibbs|Energia libera di Gibbs]], a un potenziale chimico minore, rilasciando energia.

[^1]: Anche contro gradiente di concentrazione.

Il potenziale chimico $n$ di una sostanza $i$ è definito come la derivata parziale dell’[[Energia libera di Gibbs|energia libera molare di Gibbs]] a temperatura, pressione e moli delle altre particelle costanti:
$$\micro_i = \left(\frac{\partial G}{\partial n_i}\right)_{T,P,n_j\neq i} = \left(\frac{\partial U}{\partial n_i}\right)_{S,V,n_j\neq i}$$
È ovvero la variazione di [[Energia libera di Gibbs|Energia libera di Gibbs]] all’aumentare o al diminuire del numero di molecole della sostanza considerata.

Il potenziale chimico può essere riferito a un potenziale di riferimento in condizioni standard $\micro^*$ come la somma delle diverse forme di [[Energia|Energia]] che concorrono a determinarne l’energia libera di Gibbs.
Nel caso di un soluto all’interno di una soluzione diventa[^2]:
$$\micro_j = \micro_j^* + RT\ln a_j + z_j EF +m_j gh + PV_j$$
Dove:
- $\micro_j^*$ è il potenziale di riferimento della sostanza in [[Condizioni standard|Condizioni standard]].
- $RT\ln a_j$ è una misura degli effetti della concentrazione della sostanza $j$, in cui $a$ è l’[[Attività chimica|Attività]] di quest’ultima. Da questa si può ricavare la [[Pressione osmotica|Pressione osmotica]].
- $z_jEF$ è l’energia derivante dalle [[Legge di Coulomb|Interazioni elettrostatiche]], $z_j$ è la carica del soluto $j$, $F$ la costante di Faraday e $E$ il [[Potenziale elettrico|Potenziale elettrico]].
- $m_jgh$ è l’[[Energia potenziale gravitazionale|Energia potenziale gravitazionale]].
- $PV_j$ è la [[Pressione idrostatica|Pressione idrostatica]].

Da questa relazione si può ricavare il potenziale chimico dell’acqua o [[Potenziale idrico|Potenziale idrico]].

[^2]: https://rseco.org/content/362-chemical-potential.html