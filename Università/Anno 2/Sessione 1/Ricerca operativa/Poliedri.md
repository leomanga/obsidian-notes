Se studiamo l’insieme ammissibile di un problema di [[Programmazione lineare|PL]], vediamo che è un insieme convesso, a cui diamo il nome di **poliedro**. A questo insieme possiamo attribuire dei vertici.

>[!def] Poliedro
>Un poliedro è un insieme di punti definito dall’intersezione di un certo numero di semispazi affini e semispazi indotti.
>Possiamo caratterizzare i poliedri attraverso dei vertici.
>>Con semispazio affine si intendono tutte le $x\in \mathbb{R}^{n}$ tali che, dato un $\alpha_{0}\in\mathbb{R}$ e un $\alpha\in \mathbb{R}^{n}$, $$\alpha^{T}x\le \alpha_{0}$$
>> Con semispazio indotto invece $$\alpha^{T}=\alpha_{0}$$

>[!def] Politopo
>Un politopo è un [[Poliedri|poliedro]], ma limitato.
>Un poliedro è un politopo se $\exists M\in \mathbb{R}$ tale che
>$$||x||\le M\quad \forall x\in P$$

^5fae19

>[!def] Vertici del poliedro
>Definito un poliedro $P=\begin{cases}Ax=b\\ x\ge 0\end{cases}$
>$x\in P$ è un vertice o un punto estremo di $P$ se non è possibile esprimere $x$ come combinazione convessa stretta di due punti di $P$.
>Ovvero
>$x\in P$ è un vertice se $\not \exists\ y,z\in P:\ x=\lambda z+(1-\lambda)y$, $\lambda\in(0,1)$

^5d3fe1

>[!thm] Teorema di Minkowski-Weyl
>Qualunque punto di un [[#^5fae19|politopo]] $P$ può essere espresso come combinazione convessa dei suoi [[#^5d3fe1|vertici]].
>Siano $x^{1},x^{2},\ldots, x^{k}$ i vertici di un politopo $P$ allora
>$$\forall x\in P, \exists \lambda_{1},\lambda_{2},\ldots,\lambda_{k}\ge 0;\sum_{i=1}^{k}\lambda_{i}=1$$ tali che $x=\lambda_{1}x^{1}+\lambda_{2}x^{2}+\ldots+\lambda_{k}x^{k}$

>[!thm]
>Dato un problema di programmazione lineare in $\min c^{T}x$, $x\in P$ in cui $P$ è un politopo. Allora esiste sempre un vertice di $P,x^{*} \in P$, soluzione ottima del problema.
>ù
>

>[!def] Soluzione di base
>Dato un poliedro ed una base della matrice $A$, la soluzione $x=\begin{bmatrix}x_{b}\\ x_{f}\end{bmatrix}=\begin{bmatrix}B^{-1}b\\ 0\end{bmatrix}$ ($x_{f}=0$) si dice **soluzione di base** rispetto alla base $B$. $x_{b}$ sono le $x$ relative alle colonne di $A$ usate per la base, mentre $x_f$ sono le $x$ fuori base.
>

>[!def] Soluzione di base ammissibile
>Una soluzione di base si dice ammissibile se $B^{-1}b\ge0\iff x_{b}\ge 0$

^166e60

>[!thm]
>Un punto appartenente ad un poliedro è suo vertice se e solo se è una soluzione di base ammissibile.

>[!def] Soluzione degenere
>Una soluzione di base ammissibile si dice degenere se $x_{b}=B^{-1}b$ ha componenti nulle.

[[Metodo del simplesso]]

