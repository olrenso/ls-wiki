---
share: true
---
Il *prodotto scalare* è un prodotto fra due [[Vettore|Grandezze vettoriali]] che risulta in una grandezza scalare:

$$\vec{a} \cdot \vec{b} = c$$

Dove $c$ è pari a:
$$c = |\vec{a}|\cdot|\vec{b}|\cdot \cos{\theta}$$
Ossia il modulo di $\vec{a}$ per la [[Proiezione vettoriale|Proiezione vettoriale]] di $\vec{b}$ su $\vec{a}$.

![|150](302a244b6c54b7f410febb2921622918_MD5%201.png)

Il prodotto scalare gode della proprietà commutativa $\vec{a} \cdot \vec{b} = \vec{b} \cdot \vec{a}$. La proiezione vettoriale di $\vec{b}$ su $\vec{a}$ o di $\vec{a}$ su $\vec{b}$ conducono al medesimo risultato di $c$.

#### Casi particolari
Se $\vec{a} \parallel \vec{b}\;$ $\;\cos{\theta}=1$, per cui $c=|\vec{a}|\cdot|\vec{b}|$
Se $\vec{a}\perp \vec{b}\;$ $\;\cos{\theta}=0$, di conseguenza $c=0$

---
- $\vec{i}\cdot\vec{j} = |\vec{i}|\cdot|\vec{j}|\cdot\cos{90}=1\cdot1\cdot0 = 0$
- $\vec{j}\cdot\vec{j} = |\vec{j}|\cdot|\vec{j}|\cdot\cos{0}=1\cdot1\cdot1 = 1$
- $\vec{i}\cdot\vec{i} = |\vec{i}|\cdot|\vec{i}|\cdot\cos{0}=1\cdot1\cdot1 = 1$

###### Prodotto scalare di due vettori bidimensionali
$$\begin{align*}
\vec{a} \cdot \vec{b} &= (a_x\vec{i}+a_y\vec{j})\cdot(b_x\vec{i}+b_y\vec{j}) = a_xb_x\vec{i}\cdot\vec{i} + a_xb_y\vec{i}\cdot\vec{j} + a_yb_x\vec{j}\cdot\vec{i}+a_yb_y\vec{j}\cdot\vec{j}=\\
&=a_xb_x\cdot 1+a_xb_y\cdot0+a_yb_x\cdot0+a_yb_y\cdot 1=\\
&=a_xb_x+a_yb_y
\end{align*}$$

###### Prodotto scalare di due vettori tridimensionali
$$\begin{align*}
\vec{a}\cdot\vec{b} &= (a_x\vec{i}+a_y\vec{j}+a_z\vec{k})\cdot(b_x\vec{i}+b_y\vec{j}+b_z\vec{k}) =\\
&= a_xb_x\vec{i}\cdot\vec{i} + a_xb_y\vec{i}\cdot\vec{j}+a_xb_z\vec{i}\cdot\vec{k}+a_yb_x\vec{j}\cdot\vec{i}+a_yb_y\vec{j}\cdot\vec{j}+ \ \\
&\quad\:+\ a_yb_z\vec{j}\cdot\vec{k}+a_zb_x\vec{k}\cdot\vec{i}+a_zb_y\vec{k}\cdot{j}+a_zb_z\vec{k}\cdot\vec{k}=\\
&= a_xb_x\cdot 1 + a_xb_y\cdot0+a_xb_z\cdot0+a_yb_x\cdot0+a_yb_y\cdot1+ \ \\
&\quad\:+\ a_yb_z\cdot0+a_zb_x\cdot0+a_zb_y\cdot0+a_zb_z\cdot1=\\
&=a_xb_x+a_yb_y+a_zb_z
\end{align*}$$