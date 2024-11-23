---
pagina: 201
collegamenti:
  - "[[Vettori ortogonali]]"
  - "[[Disuguaglianza triangolare]]"
aliases:
  - minima distanza
---
# Definizione
Sia $V$ [[Spazio vettoriale]] su $\mathbb{R}$ dotato di [[Prodotto scalare]] e $A \not = 0$
![[Proiezione ortogonale.excalidraw]]
Dato $x\in V$, il vettore $x_A$ è la proiezione ortogonale di $x$ su $L(A)$ se e solo se 
$\widehat{(x-x_A,A)}={\frac{\pi}{2}}$, ovvero $<x-x_A,A>= 0$, ovvero $(x-x_{A})\perp A$

- La proiezione ortogonale di $x$ su $A$ si indica con $$\pi_A^{\perp}(x) = \frac{<x,A>}{<A,A>}A$$
- Non è né una funzione iniettiva né una funzione suriettiva.

# Proiezione in uno spazio $S$
pg 216
$$\pi_{S}^{\perp}=\sum_{i=1}^{m}\pi_{A_{i}}^{\perp}\in S$$
dove $S = L(A_1,A_2,\ldots,A_m)$, e $(A_1,A_2,\ldots,A_m)$ è una [[Base ortogonale e ortonormale|base ortogonale]].
- Rappresenta il punto di $S$ avente minima distanza da $X$**