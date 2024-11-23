---
pagina: 143
collegamenti:
  - "[[Matrice completa e incompleta]]"
  - "[[Rango]]"
---
# Teorema
Sia $n$ il numero delle incognite del sistema $S$.
$$rank(M_{i})\le rank(M_{c})\le rank(M_i)+1$$
- Se $rank(M_{c})=rank(M_{i})+1\Rightarrow$ Sistema impossibile, $Sol(S) = \varnothing$
-  Se $rank(M_{c})=rank(M_{i}) \Rightarrow$ Sistema risolubile, $Sol(S) \not= \varnothing$
	- $rank(M_{c})=rank(M_{i}) = 1 \Rightarrow$ $S$ determinato e $|Sol(S)| = 1$
	- $rank(M_{c})=rank(M_{i}) = n-r \Rightarrow$ $S$ indeterminato, con $r$ incognite libere

$Sol(S) = Sol(\xi_1,\xi_2,\ldots,\xi_{m})= p +Sol(\xi_{1,0},\xi_{2,0},\ldots,\xi_{m,0})$
- $Sol(S)$ è uno [[Spazio affine]] a $V_n(\mathbb{K})$.
- $\xi_{1,0},\xi_{2,0},\ldots,\xi_{m,0}$ sono le [[equazione lineare  omogenea|equazioni lineari omogenee]] associate a $\xi_1,\ldots$
- $p$ è una particolare soluzione del sistema $S$.

# Caso particolare
Se $S$ è un sistema lineare omogeneo di $m$ equazioni in $n$ incognite, allora $Sol(S)$ è un [[Sottospazio lineare]] di $V_n(\mathbb{K})$ di [[Dimensione]] pari ad $n-rank(M_c)$