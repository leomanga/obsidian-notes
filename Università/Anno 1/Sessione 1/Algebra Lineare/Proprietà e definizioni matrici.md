---
pagina: 256
---
# Definizione | Matrici simili
Siano $A$ e $B$ due [[Matrice quadrata|matrici quadrate]] di ordine $n$.
$A$ è SIMILE a $B$ $(A\sim B)$ $\iff \exists C \in M_n(\mathbb{K})\mbox{ invertibile }: B = C^{-1}\cdot A\cdot C$
- Matrici rappresentative di uno stesso endomorfismo sono simili
> Da [[Teorema pg 287#Corollario 2]], due matrici sono SIMILI se e solo se ammettono la stessa forma di Jordan a meno di una permutazione dei blocchi in diagonale
> ^d50d72
### Proprietà
- Proprietà riflessiva
	$A\sim A$, $A=C^{-1}\cdot A \cdot C$ ($C$ è l'identità)
- Proprietà simmetria
	$A\sim B\Rightarrow B\sim A$
- Proprietà transitiva
	$A\sim B\land B \sim C \Rightarrow A\sim C$

# Definizione | Matrice diagonalizzabile
$A \in M_n(\mathbb{K})$ è diagonalizzabile se e solo se è [[Proprietà e definizioni matrici#Definizione Matrici simili|simile]] ad una matrice diagonale.
Cambiando le basi se ne può trovare una.

Possiamo anche dire che, da [[Polinomio minimo di f]]
- $\varphi$ è diagonalizzabile $\Rightarrow$ $P_{min}(\varphi)=(t-\lambda_{1})(t-\lambda_{2})\cdot \ldots \cdot (t-\lambda_{m})$ dove $\lambda_{1},\lambda_{2},\ldots,\lambda_{m}$ sono gli autovalori di $\varphi$. ^a469d1