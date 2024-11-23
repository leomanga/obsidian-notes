---
pagina: 401
---
# Definizione
Sia $V\times V\to \mathbb{K}$ [[Forma bilineare]]
$dim(V)=n$

$$M=\mu_{\mathbb{E}}(<.,.>) = \begin{bmatrix}
<v_1, v_1> & <v_1, v_2> & \cdots & <v_1, v_n> \\
<v_2, v_1> & <v_2, v_2> & \cdots & <v_2, v_n> \\
\vdots & \vdots & \ddots & \vdots \\
<v_n, v_1> & <v_n, v_2> & \cdots & <v_n, v_n>
\end{bmatrix}
$$
$$$<x,y>=(x)^{T}_{\mathbb{E}}\cdot M\cdot(y)_{\mathbb{E}}=(x_1,\ldots,x_{n})\cdot M\cdot\begin{pmatrix}x1\\x2\\\ldots\\x_n\end{pmatrix}$$
# Cambio di base
$\phi:V\times V\to\mathbb{R}$
$M^{'}=\mu_{F}(\phi)$
$M=\mu_{E}(\phi)$
Sia $C$ la matrice che porta $E$ in $F$.
$\phi(x,y)=(x)_{E}^{T}\cdot M\cdot(y)_{E}=(x)_{F}^{T}\cdot\underbrace{C^{T}\cdot M\cdot C}_{M^{I}}\cdot(y)_F\Rightarrow M^{'}=C^{T}\cdot M\cdot C$
Se $C$ è ortogonale, allora $M e M^{'}$ sarebbero simili.
# Corollario
Se $\phi$ è una [[Forma bilineare#Definizione forma bilineare simmetrica|forma bilineare simmetrica]] allora $\mu_{E}(\phi )$ è una matrice simmetrica.
Dal [[Teorema spettrale]] si può dire allora che $M$ è ortogonalmente diagonalizzabile
$$\exists C:C^{-1}=C^{T}:C^{T}\cdot M\cdot C\mbox{ è diagonale}$$