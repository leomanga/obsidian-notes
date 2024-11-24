---
pagina: 162
aliases:
  - spazio affine
---
# Definizione

Sia $V$ [[Spazio vettoriale|spazio vettoriale]].
Uno spazio affine di $V$ è il [[Traslazione|traslato]] di uno [[Spazio vettoriale|Spazio lineare]].
$$\mathbb{S} = \tau_p(\mathbb{S}_{0})= \{p+x:x\in\mathbb{S}_0\}$$
Dove $\mathbb{S}_0$ è un [[Sottospazio lineare]].
- $p$ è detto [[Punto di appoggio]].
- $\mathbb{S}_0$ è detta [[Direzione]] o giacitura di $\mathbb{S}$.

[[Dimensione|dim]]($\mathbb{S}$) = [[Dimensione|dim]]($\mathbb{S}_0$) 
![[Spazio affine.excalidraw|{height:40%}]]

- [[Sottospazio lineare]] $\Rightarrow$ [[Sottospazio affine]]

# Caratteristiche
- I [[Sottospazio affine|sottospazi affini]] di [[dim]] 0 sono i [[Vettore|punti]] di $V$.
- I [[Sottospazio affine|sottospazi affini]] di [[dim]] 1 sono le [[Retta|rette]] di $V$.
- I [[Sottospazio affine|sottospazi affini]] di [[dim]] 2 sono i [[Piano|piani]] di $V$.
- [[dim]]($\varnothing$) $:= -1$ per convenzione.

# Proprietà
Sia $V$ [[Spazio vettoriale]]
Siano gli insiemi di vettori $A,B\subseteq V$
1) $A \subseteq B \iff (p+A) \subseteq (p+B)$
2) $A = B \iff (p+A) = (p+B)$
3) $\cup_{i\in I}(p + A_{i})= \cup_{i\in I}(\tau_p(A_{i})) = \tau_p(\cup_{i\in I}A_{i})= p + \cup_{i\in I}A_i$
4) $\cap_{i\in I}(p+A_{i})= p + \cap_{i\in I}A_i$
5) Sia $A$ un [[Sottospazio lineare]] di $V$ e $p\in V$ $p \in p+A$	
6) $p+A = A \iff p\in A$ con $A$ [[Sottospazio lineare|sottospazio lineare]] e $P\in V$.
7) Siano $A$ e $B$ due [[Sottospazio lineare|sottospazi lineari]] di $V$ e $p,q \in V$.
	$p+A \in q+B \iff (A\subseteq B) \land (p\in q+B)$
8) $p+A = q+B \iff (A=B) \land (p\in q+B)$
9) $p+A = q+A \iff p \in q+A$
10) $(p+A)\cap(q+A) \not=0\iff p+A = q+A$
11) $(A \subseteq B)\land((p+A) \cap (q+B)\not=0)\Rightarrow (p+A)\subseteq(q+B)$
12) $A$ [[Sottospazio lineare|sottospazio lineare]]
	$p+A = A \iff 0 \in p+A$
13) $\cap_{i\in I}(P_{i}+ A_{i}) \not= \varnothing \iff \cap_{i\in I}(P_{i}+ A_{i}) = p +\cap_{i\in I}A_i$
