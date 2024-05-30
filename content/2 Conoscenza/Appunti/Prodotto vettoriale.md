---
share: true
---
Il *prodotto vettoriale* è il prodotto fra due [[Vettore|Vettori]] risultante in una terza grandezza vettoriale.
$$\vec{a} \times \vec{b} = \vec{c}$$
Dove:
- Il modulo è dato da: $|c|= |\vec{a}|\cdot|\vec{b}|\cdot\sin{\theta}$
- La direzione è perpendicolare al piano su cui giacciono i vettori $\vec{a}$ e $\vec{b}$. Ossia è *normale* al piano che li attraversa. 
- Il verso è determinato con la [[Regola della mano destra|Regola della mano destra]].

![|200](c4d065862a369a650f66703ba2ef42ad_MD5%201.png)

Si noti che:
- Se $\vec{a} \parallel \vec{b}$ $\;\sin{\theta} = 0$ per cui $|c| = 0$
- Se $\vec{a} \perp \vec{b}$ $\;\sin{\theta} = 1$ per cui $|c| = |\vec{a}|\cdot|\vec{b}|$

A differenza del [[Prodotto scalare|Prodotto scalare]] il prodotto vettoriale non è commutativo:
$$\vec{a} \times \vec{b} \neq \vec{b}\times \vec{a}$$
Ma anziché gode della proprietà *anticommutativa*:
$$\vec{a}\times\vec{b}=-(\vec{b}\times\vec{a})$$

---
###### Prodotto vettoriale fra due vettori bidimensionali
$$\begin{align*}
\vec{a}\times\vec{b} &= (a_x\vec{i}+a_y\vec{j}) \times (b_x\vec{i}+b_y\vec{j}) =\\ &= a_xb_x\vec{i}\times\vec{i}+a_xb_y\vec{i}\times\vec{j} + a_yb_x\vec{j}\times\vec{i}+a_yb_y\vec{j}\times\vec{j}= \\
&= a_xb_x\cdot0+a_xb_y\vec{k}+a_yb_x(-\vec{k})+a_yb_y\cdot0=\\
&= (a_xb_y-a_yb_x)\vec{k}
\end{align*}$$
###### Prodotto vettoriale fra due vettori tridimensionali
$$\begin{align*}
\vec{a} \times \vec{b} &= (a_x\vec{i}+a_y\vec{j}+a_z\vec{k})\times(b_x\vec{i}+b_y\vec{j}+b_z\vec{k}) =\\
& = a_xb_x\vec{i}\times\vec{i} + a_xb_y\vec{i}\times\vec{j}+a_xb_z\vec{i}\times\vec{k}+a_yb_x\vec{j}\times\vec{i}+a_yb_y\vec{j}\times\vec{j}+ \ \\
&\quad\:+\ a_yb_z\vec{j}\times\vec{k}+a_zb_x\vec{k}\times\vec{i}+a_zb_y\vec{k}\times{j}+a_zb_z\vec{k}\times\vec{k}=\\
&= a_xb_x\cdot0 + a_xb_y\vec{k}+a_xb_z(-\vec{j})+a_yb_x(-\vec{k})+a_yb_y\cdot0 + \ \\
&\quad\:+\ a_yb_z\vec{i}+a_zb_x\vec{j}+a_zb_y(-\vec{i})+a_zb_z\cdot0=\\
&=a_xb_y\vec{k}+a_xb_z(-\vec{j})+a_yb_x(-\vec{k}) + a_yb_z\vec{i}+a_zb_x\vec{j}+a_zb_y(-\vec{i}) = \\
&=(a_yb_z -a_zb_y)\vec{i} + (a_zb_x-a_xb_z)\vec{j} + (a_xb_y - a_yb_x)\vec{k}
\end{align*}$$