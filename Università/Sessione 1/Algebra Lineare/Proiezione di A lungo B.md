---
pagina: 156
---
# Definizione
Sia $V = A \oplus B$
$\pi_A^{B}: V \to V$
$\pi_A^{B}(x)= x_A$

Proiezione su $A$ lungo $B$

# Proposizione
$V = A \oplus B$
$\forall x,y \in V\qquad \forall \lambda, \mu \in \mathbb{K}$
$\pi_A^{B}(\lambda x + \mu y) = \lambda\pi_A^{B}(x)+ \mu\pi_A^{B}(y)$
#dimostrazione-da-fare 

# Autovalori, autospazio ecc...
PG 268
- $0$ è un [[Autovettori - autovalori - autospazi|autovalore]] di $\pi_{A}^{B}$ ($ker(\pi_{A}^{B})=B$)
	Quindi l'[[Autovettori - autovalori - autospazi|autospazio]] di autovalore $0$ è $B$.
	$mg(0)=dim(B)$
- 1 è autovalore di $\pi_{A}^{B}$($ker(\pi_{A}^{B}-I)=fix(\pi_{A}^{B})=A$)
	Quindi l'autospazio di autovalore 1 è A
	$mg(1)=dim(A)$

- $\pi_{A}^{B}$ è diagonalizzabile, perchè, dato che $V=A(0)\oplus A(1)=A\oplus B$, basta prendere una base di $B$ ed una di $A$, perchè i vettori appartenenti a quegli spazi sono autovettori.
Quindi presa una base $E=(E_1,E_2)$ dove $E_1$ base di $B$ ed $E_2$ base di $A$:
$$\mu_E(\pi_{A}^{B})=\left(
\begin{split}
&0\ 0\ \ldots\ 0\ 0\ 0\ \ldots\ 0\\
&0\ 0\ \ldots\ 0\ 0\ 0\ \ldots\ 0\\ 
&\ldots\\
&0\ 0\ \ldots\ 0\ 1\ 0\ \ldots\ 0\\ 
&0\ 0\ \ldots\ 0\ 0\ 1\ \ldots\ 0\\ 
&\ldots\\
&\underbrace{0\ 0\ \ldots\ 0}_{dim(B)}\underbrace{\ 0\ 0\ \ldots\ 1}_{dim(A)}\\
\end{split}

\right)$$
- $ma(0)=dim(B),ma(1)=dim(A))$