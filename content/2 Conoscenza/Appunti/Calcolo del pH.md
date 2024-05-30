---
share: true
---
### Acido o base forte
Nel caso di acidi o basi forti la concentrazione degli ioni derivanti dall’acqua è generalmente trascurabile, generalmente fin quando il composto non è fortemente diluito, ovvero quando ha una concentrazione minore di $10^{-6} \text{ M}$.
$$\text{Acido: } \text{ pH} = -\log{\ce{[H3O+]}} \qquad \text{Base: } \text{ pH} = -\log{\ce{[OH-]}}$$
###### Esempio
> Si calcolino il pH e il pOH di una soluzione acquosa $1,00\cdot10^{-4} \text{ M}$ di $\ce{HClO4}$
> 
> ---
> 
> L’acido perclorico è un acido forte con una [[Costante di dissociazione|Costante di dissociazione]] maggiore di uno, quindi in acqua si dissocia completamente.
> $$\ce{HClO4 + H2O -> ClO4- + H3O+}$$
> Il [[pH|pH]] è pari alla concentrazione degli ioni idronio, pari alla concentrazione dell’acido. Gli ioni idronio derivanti dall’acqua sono trascurabili a causa della concentrazione relativamente elevata dell’acido.
> $$\text{pH} = -\log_{10}{\ce{[HClO4]}} = -\log_{10}{1,00\cdot10^{-4}} = 4$$
> Mentre il pOH si può ricavare facilmente dalla relazione $\text{pH} + \text{pOH} = \text{pK}_w$
> $$\text{pOH} = 14 -\text{pH} = 14-4=10$$
> Oppure si ricava prima la concentrazione degli ioni idrossido dal [[Prodotto ionico|Prodotto ionico]] dell’acqua $\ce{[H3O+][OH-]} = 10^{-14}$
> $$\ce{[OH-]} = \frac{10^{-14}}{\ce{[H3O+]}} = \frac{10^{-14} \text{ M}^2}{10^{-4} \text{ M}} = 10^{-10} \text{ M}$$
> E successivamente il pOH:
> $$\text{pOH} = -\log_{10}{\ce{[OH-]}} = -\log_{10}{10^{-10}} = 10$$
> Si può infine calcolare l’errore relativo[^1] alla trascurazione degli ioni idronio derivanti dall’acqua:
> $$E_r = \ce{\frac{[OH-]}{[H3O+]}} \cdot 100 = \frac{10^{-10}}{10^{-4}} \cdot 100 = 10^{-4} \;\%$$
> Ossia un valore di molto inferiore al 5%, per cui assolutamente trascurabile.

[^1]: Nel caso fosse stata una base l’errore si sarebbe ricavato dal rapporto fra la concentrazione degli ioni idronio su quella degli ioni idrossido, ovvero l’inverso.

---
#### Acido o base debole
Quando si calcola il pH di un acido o di una base deboli bisogna tenere in considerazione che la loro dissociazione in acqua è una [[Reazioni chimiche#Reazioni reversibili|Reazione]] all’[[Equilibrio chimico|Equilibrio]].
Le concentrazioni all’equilibrio quindi si trovano analogamente ai [[Problemi sugli equilibri|Problemi sugli equilibri]].

Come nel caso degli acidi e delle basi forti la concentrazione degli ioni derivanti dalla dissociazione dell’acqua è trascurabile per concentrazioni maggiori di $10^6$.

###### Esempio
> Calcolare le concentrazioni delle specie all’equilibrio e il pH di una soluzione $10^{-3} \text{ M}$ di $\ce{CH3COOH}$ sapendo che la [[Costante di dissociazione|Costante di dissociazione]] dell’acido è $K_a = 1,8\cdot10^{-5}$
> 
> ---
> Si inizia prima di tutto scrivendo la reazione all’equilibrio dell’acido:
> $$\ce{CH3COOH + H2O <=> CH3COO- + H3O+}$$
> A questo punto si può creare la tabella riassuntiva delle variazioni di concentrazione.
> 
> |            |     $\ce{CH3COOH}$     | $\ce{CH3COO-}$ | $\ce{H3O+}$ |
> | ---------- |:----------------------:|:--------------:|:-----------:|
> | Iniziale   |  $10^{-3} \text{ M}$   |      $0$       |     $0$     |
> | Variazione |          $-x$          |      $+x$      |    $+x$     |
> | Equilibrio | $10^{-3} -x$ |      $x$       |     $x$     |
> 
> 
> Sapendo la costante di dissociazione dell’acido si possono sostituire i valori riportati in tabella e trovare $x$:
> $$K_a = \ce{\frac{[CH3COO-][H3O+]}{[CH3COOH]}} = 1,8\cdot10^{-5} \longrightarrow1,8\cdot10^{-5} = \frac{x\cdot x}{10^{-3}-x}$$
> Quando la concentrazione dell’acido (o della base) è molto superiore alla parte dissociata $x$ il denominatore può essere semplificato alla sola concentrazione dell’acido.
> Per poter verificare che quest’approssimazione sia fattibile bisogna verificare l’errore relativo che si commetterebbe.
> Si calcola quindi il valore di $x$ approssimando a:
> $$1,8\cdot10^{-5} = \frac{x^2}{10^{-3}} \longrightarrow x = \sqrt{1,8\cdot10^{-8}} = 1,3\cdot 10^{-4}\text{ M}$$
> E avendo $x$ si ricava l’errore:
> $$E_r = \frac{x}{\ce{[CH3COOH]}} \cdot 100= \frac{1,3\cdot10^{-4} \text{ M}}{10^{-3} \text{ M}} \cdot 100 = 13\%$$
> Un errore maggiore del 5% è considerato *non* trascurabile, per cui bisogna risolvere l’equazione di secondo grado, prendendo come accettabile solamente il valore di $x$ maggiore di zero.
> $$x^2+1,8\cdot10^{-5}x-1,8\cdot10^{-8} = 0 \; \Longrightarrow \; x = 1,25\cdot10^{-4} \text{ M}$$
> Avendo $x$ si possono quindi ottenere le concentrazioni delle varie specie all’equilibrio:
> $$\begin{align*}
> &\ce{[CH3COOH]}_{eq} = \ce{[CH3COOH]} - x = 10^{-3} \text{ M} - 1,25\cdot10^{-4} \text{ M} = 8,75 \cdot 10^{-4} \text{ M}\\
> &\ce{[CH3COO-]}_{eq}  = x = 1,25\cdot10^{-4} \text{ M}\\
> &\ce{[H3O+]}_{eq} = x = 1,25\cdot10^{-4} \text{ M}\\
> &\ce{[HO-]} = \frac{10^{-14}}{\ce{[H3O+]}} = \frac{10^{-14} \text{ M}^2}{1,25\cdot10^{-4} \text{ M}} = 8\cdot 10^{-11} \text{ M}
> 
> \end{align*}$$
> Come nel caso degli [[Calcolo del pH#Acido o base forte|Acidi o basi forti]] si è trascurata la concentrazione degli ioni idronio derivanti dall’autodissociazione dell’acqua.
> Anche qui si calcola l’errore relativo per verificare che il risultato sia accettabile.
> $$E_r = \ce{\frac{[OH-]}{[H3O+]}} \cdot 100= \frac{8\cdot10^{-11}\text{ M}}{1,25\cdot 10^{-4}\text{ M}} \cdot 100 = 6,4\cdot10^{-5} \; \%$$
> Si calcola infine il pH:
> $$\text{pH} = -\log{\ce{H3O+}} = -\log{1,25\cdot10^{-4}} = 3,9$$
>