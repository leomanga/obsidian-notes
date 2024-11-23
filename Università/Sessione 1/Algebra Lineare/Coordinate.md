---
pagina: 124
---
# Definizione
Sia $V$ [[Spazio vettoriale|spazio vettoriale]] di [[Dimensione|dim]]($V$) = $n$.
Sia $\mathbb{E} = (E_1,E_2,\ldots,E_n)$ [[Base|base]] ordinata di $V$.
$$\forall x \in V,\qquad x = x_1E_1+x_2E_{2}+\ldots +x_nE_n$$
$x_1,x_2,\ldots,x_n$ sono <mark style="background: #FFB86CA6;">univocamente determinati</mark>.

- Questa viene chiamata [[Rappresentazione completa]] di $x$ rispetto alla [[Base]] $\mathbb{E}$.

- I coefficienti $x_1,x_2,\ldots,x_n$ della [[Rappresentazione completa]] di $x$ rispetto alla [[Base]] $\mathbb{E}$  si chiamano [[Coordinate]] di $\mathbb{X}$ rispetto ad $\mathbb{E}$. 
- Si indicano con
$$(x)_{\mathbb{E}} := (x_1,x_2,\ldots,x_{n}),\qquad \forall x \in V$$
# Rappresentazione ridotta o essenziale
Se $x \not= 0$ e $x_{i1},x_{i2},\ldots,x_{in}$ sono non nulli, allora
$$x = x_{i1}E_{i1}+x_{i2}E_{i2}+\ldots+x_{in}E_{in}$$
# Cambio di coordinate
Sia $V$ uno [[Spazio vettoriale]] su $\mathbb{K}$ e [[Dimensione|dim]]($V$) = $n$.
$$
\left(
\begin{split}
&\mathbb{E} = (E_1,E_2,\ldots,E_n)\\
&\mathbb{F} = (F_1,F_2,\ldots,F_n)
\end{split}
\right) \mbox{ basi ordinate di } V_n(\mathbb{R})
$$
$$\begin{split}
&F_{1}= (E_1a_{11}+E_2a_{21}+\ldots+E_na_{n1})\qquad (F_1)_{\mathbb{E}} = (a_{11},a_{21},\ldots)\\
&F_{2}= (E_1a_{12}+E_2a_{22}+\ldots+E_na_{n2})\qquad \ldots\\
&\ldots \qquad \ldots\\
&F_{n}= (E_1a_{1n}+E_2a_{2n}+\ldots+E_na_{nn}) \qquad \ldots\\
\end{split}$$
Abbreviato:
$$F_{k}= \sum_{i=1}^{n}E_ia_{ik}\qquad \forall k=1,\ldots,n$$
Si può in questo modo creare una [[Matrice che fa passare da una base ad un altra]]
![[Matrice che fa passare da E ad F.excalidraw]]

Grazie a questa matrice possiamo trovare le $(x)_\mathbb{E} = M(x)_\mathbb{F}$

# Calcolare $(x)_\mathbb{F}$, conoscendo $(x)_\mathbb{E}$
Per fare ciò dobbiamo invertire la matrice $M$, risolvendo il sistema nelle incognite $y_1,y_2,\ldots,y_n$
