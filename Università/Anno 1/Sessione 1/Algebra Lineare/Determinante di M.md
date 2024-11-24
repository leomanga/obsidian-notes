---
pagina: 269
---
# Definizione | Discriminante per matrici 2 x 2
Sia 
$$M=\left(
\begin{split}
a\ b\\
c\ d
\end{split}
\right)$$
Il determinante di $M$ è
$$det(M):=\underbrace{ad}_{elementi\ su\ diagonale\ principale}-\underbrace{bc}_{elementi\ su\ diagonale\ secondaria}$$
N.B. questo vale solo con le matrici $2 \times 2$
Per le matrici $n\times n$ guarda 
# Proprietà
$M$ è invertibile se e solo se il determinante $\not = 0$

# Definizione | Discriminante per matrici n x n
[[Permutazioni e trasposizioni]]
Si definisce il discriminante di una matrice $A$ $n\times n$ come
$$det(A)=\sum_{\sigma\in Sym(n)}Sgn(\sigma)\prod_{i=1}^{n}a_{i\sigma(i)}$$

# Proprietà
1) $det(M)=det(M^{T})$
2) $\sigma\in Sym(n)\quad det(A_{\sigma(1)},A_{\sigma(2)},\ldots,A_{\sigma(n)})=Sgn(\sigma)det(A_{1},A_{2},\ldots,A_{n})$, dove $A_1,A_2,\ldots$ rappresentano le righe della matrice
3) $det(\sum_{i=1}^{m}b_{i}B_{i},A_2,\ldots,A_{n})=\sum_{i=1}^{m}(b_{i}det(B_i,A_{2},\ldots,A_{n}) )$
	$det(\lambda A+\mu B,c)=\lambda det(A,C)+\mu det(B,C)$
	$det(A, \lambda B+\mu C)=\lambda det(A,B)+\mu det(A,C)$
	$det(A_{1},A_{2})=-det(A_{2},A_{1})$
	1)  $det(aA_1,A_2,\ldots,A_n)=a(A_1,A_2,\ldots,A_n)$
	2) $det(0,A_2,\ldots,A_n)=0$
	3) $det(a_{1}A_{1},a_{2}A_{2},\ldots,a_{n}A_{n})=a_{1}\cdot a_{2}\cdot\ldots\cdot a_{n}det(A_{1},\ldots,A_{n})$
#### Proposizione 1
 Il determinante di una matrice $2\times 2$ è una [[Forma bilineare]] antisimmetrica(o alternante)
 (si vede dalla proprietà 3)
#### Proposizione 2
Il determinante di una matrice $n\times n$ è una forma multilineare alternante

4) $A_{i}=A_{j}, i< j\Rightarrow det(A_1,\ldots,A_i,\ldots,A_{i},\ldots,A_n)=0$
5) $det(A_{1},\ldots,A_{n-1}, \sum_{i=1}^{n-1}a_{i}A_{i})=0$
6) $det(A_{1}+\sum_{i=2}^{n}a_{i}A_{i},A_{2},\ldots,A_{n})= det(A_1,A_2,\ldots,A_{n})$
7) $rank(M)<n\Rightarrow det(M)=0$
8) $det(\begin{bmatrix} 1 & 0 & 0 & \ldots & 0 \\ 0 & 1 & 0 & \ldots & 0 \\ 0 & 0 & 1 & \ldots & 0 \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & 0 & \ldots & 1 \\ \end{bmatrix})$ = 1
9) $det(\begin{bmatrix} a_{11} & 0 & 0 & \ldots & 0 \\ 0 & a_{22} & 0 & \ldots & 0 \\ 0 & 0 & a_{33} & \ldots & 0 \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & 0 & \ldots & a_{nn} \\ \end{bmatrix})= \prod_{i=1}^{n}a_ {ii}$
10)  $det(\begin{bmatrix} a_{11} & a_{12} & a_{13} & \ldots & a_{1n} \\ 0 & a_{22} & a_{23} & \ldots & a_{2n} \\ 0 & 0 & a_{33} & \ldots & a_{3n} \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & 0 & \ldots & a_{nn} \\ \end{bmatrix})=$ ad esempio 9 grazie a [[Gauss Jordan]]
Continua da pg 282

# Teorema
Data $M\in M_{n}(\mathbb{k})$
$det(M)\not = 0 \iff rank(M)=n\iff M\mbox{ invertibile}$

# Proposizione 3
Il determinante non dipende dalla base della matrice.