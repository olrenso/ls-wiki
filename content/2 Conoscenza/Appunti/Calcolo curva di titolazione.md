---
share: true
---

Per calcolare analiticamente la curva di titolazione di una titolazione acido–base si calcola il pH di una serie di punti all’aggiunta di differenti quantità di titolante all’analita.

## Acido forte–Base forte
![](8fa1e4943b5b1a998c2dfbba4c257149_MD5%201.png)

![](9e028ef0967417ed302332785a13da86_MD5%201.png)


## Acido debole–Base forte
![](f4e4197ad7c6acbf89fa0dd926626d00_MD5%201.png)

Titolazione di 25 mL di acido formico $\ce{HCOOH}$ 0,100 M ($K_a = 1,8\cdot 10^{-4}$) con idrossido di sodio $\ce{NaOH}$ 0,100 M.
$$\ce{HCOOH + NaOH -> \underset{Formiato di sodio}{NaHCOO} + H2O}$$

Per costruire la curva di titolazione si calcolerà il pH della soluzione risultante aggiungendo all’analità diverse quantità di idrossido di sodio, quali: 0, 5, 10, 20, 25, 30 e 40 millilitri.

---
$$\ce{25 mL HCOOH + 0 mL NaOH}$$
In soluzione c’è solo l’acido debole, il pH sarà quindi dato dalla concentrazione degli ioni idronio che si dissociano da esso.
$$\ce{HCOOH + H2O <=> HCOO- + H3O+}$$
Dalla costante di dissociazione acida si ottiene la concentrazione degli ioni idronio.
$$K_a=\ce{\frac{[HCOO-][H3O+]}{[HCOOH]}} \;\longrightarrow\; \ce{[H3O+]} = \sqrt{K_a\cdot C_a}$$
E quindi il pH sarà:
$$\text{pH}=-\log_{10}{\sqrt{1,8\cdot10^{-4}\cdot0,100}} = 2,37$$
---
$$\ce{25 mL HCOOH + 5 mL NaOH}$$
Con l’aggiunta di NaOH si ottiene una soluzione tampone, si ha sia l’acido debole che la sua specie coniugata forte derivante dal sale che si ottiene con la reazione acido–base della titolazione.

Si calcola quindi le moli di acido in eccesso e le moli di sale, ossia quelle del titolante.

$$n_{ecc \;\ce{HCOOH}} = \ce{M_{HCOOH} \cdot V_{HCOOH} - M_{NaOH}\cdot V_{NaOH}} = 2\cdot10^{-3}\text{ mol}$$
$$n_\ce{NaHCOO} = \ce{M_{NaOH} \cdot V_{NaOH}} = 5\cdot10^{-4} \text{ mol}$$
Per poi trovare il pH.
$$\text{pH}=-\log_{10}{(K_a)\cdot\frac{n_a}{n_s}} = -\log_{10}{\left(1.8\cdot^{-4}\cdot\frac{2\cdot10^{-3}}{5\cdot10^{-4}}\right)} = 3,14$$
---
Analogamente si procede fino a giungere al punto di equilibrio, dove in soluzione ci sarà solo il formiato di sodio.

Essendo un sale derivante da una specie debole e una forte la base coniugata forte dell’acido, quando il sale si dissocia, si idrolizzerà e innalzerà il pH.

$$\ce{NaHCOO <=>[H2O] Na+ + HCOO-}$$
$$\ce{HCOO- + H2O <=> HCOOH + OH-}$$

Trattandosi di un idrolisi il pH sarà dato da:
$$pH = 14+\log_{10}{\sqrt{Ki\cdot C_s}} = 8,22$$
Dove:
$$Ki = \frac{Kw}{Ka} = \frac{10^{-14}}{1,8\cdot10^{-4}} = 5,5\cdot 10^{-11}$$
$$C_s = \frac{n_\ce{HCOOH}}{\ce{V_{HCOOH} + V_{NaOH}}} = \frac{2,5\cdot10^{-3} \text{ mol}}{0,05 \text{ L}} = 0,05$$
---
Si conclude inoltre calcolando alcuni punti dove l’idrossido di sodio è in eccesso.
Qui il pH è influenzato sia dall’idrolisi del sale che dagli ioni idrossido derivanti dalla dissociazione della base forte.

$$\ce{NaOH ->[H2O] Na+ + OH-}$$
Data un aggiunta di 30 mL di idrossido si avranno 5 mL in eccesso, ovvero $5\cdot10^{-4} \text{ mol}$.

Dato che la quantità di ioni ossidrilici derivanti dall’idrolisi è trascurabile la concentrazione di essi sarà pari a quella derivanti dalla base forte, ovvero:
$$\ce{[NaOH]}_{ecc} = \ce{[OH-]} = \frac{n_{ecc \;\ce{NaOH}}}{\text{V}_\text{soluzione}} = \frac{5\cdot10^{-4}}{(0,025+0,030)\text{ L}} = 9,09 \cdot 10^{-3} \text{ M}$$
$$\text{pH} = 14+\log_{10}{9,09\cdot10^{-3}} = 11,96$$


![](7118dabedd973af1457a3e3f0ef5a2ef_MD5%201.png)