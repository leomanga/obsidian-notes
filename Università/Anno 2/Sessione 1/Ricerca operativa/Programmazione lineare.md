---
aliases:
  - PL
---
Il problema di programmazione lineare consiste nel determinare un punto $x^{*}$ appartenente ad un insieme $X$ tale da rendere minima una funzione $f$ lineare. In generale viene indicato così:

$$
\begin{split}\min f(x)\\ x\in X\subset \mathbb{R}^{n}\end{split}
$$

^0dd399

dove $X=\{x:h(x)=0,g(x)\ge 0\}$, $g$ e $h$ vettori di funzioni lineari di $x\in \mathbb{R}^{n}$. 
Dato che le funzioni lineari sono sia concave che convesse, possiamo usare [[Ottimizzazione vincolata#^a41736]], quindi avremo che $X$ è un [[Insieme convesso]], quindi un minimo locale è anche un minimo globale.

Possiamo scrivere un generico problema di programmazione lineare come
$$\begin{split}\min c^{T}x\\Ax=b\\x\ge 0\end{split}$$
dove $A$ è una matrice $m\times n$, $c\in \mathbb{R}^{n}$, $b\in \mathbb{R}^{m}$ e $x\in \mathbb{R}^{n}$.
Supporremo inoltre che $m<n$ e che la $A$ abbia [[Rango]] pieno, ossia $m$.
Cercheremo di applicare le [[Condizioni di Karush-Kuhn-Tucker]].

Avremo che devono esistere due vettori $u^{*}, s^{*}$ (il primo si riferisce ai vincoli attivi, il secondo alla non negatività), tali che
$$\begin{split}
\nabla_{x}L(x^{*},u^{*},s^{*})=c^{T}-u^{*T}A-s^{*T}=0\\
Ax^{*}=b\\
x^{*}\ge 0\\
s^{*}\ge 0\\
s_{j}^{*}x_{j}^{*}=0\quad \forall j=1,\ldots,n
\end{split}$$
Possiamo riscrivere le condizioni semplificando così
$$\begin{split}
Ax^{*}=b\\
x^{*}\ge 0\\
c^{T}-u^{*T}A\ge 0\\
(c^{T}-u^{*T}A)x^{*}=0
\end{split}$$

^533680

>[!thm]
>Dato un problema di PL [[#^0dd399]], se $x^{*}$ è un punto di minimo, allora esistono vettori $u^{*}$ e $s^{*}$ tali da soddisfare ![[#^533680]]

>[!thm]
>Se $x^{*}$ e $u^{*}$ soddisfano [[#^533680]], allora $c^{T}x^{*}=b^{T}u^{*}$

[[Problema duale]]
 


