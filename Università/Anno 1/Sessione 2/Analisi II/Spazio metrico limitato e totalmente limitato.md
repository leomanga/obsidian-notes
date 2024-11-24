---
aliases:
  - spazio metrico limitato
  - spazio metrico totalmente limitato
collegamenti:
  - "[[Palla]]"
  - "[[Diametro]]"
---
# Definizione | Spazio metrico limitato
Sia $(X,d)$ uno [[Spazi metrici|spazio metrico]], sia $E\subseteq X$.
Allora $E$ si dice limitato se $$\begin{split}&\exists x\in X,\exists r>0:E\subseteq B_r(x)\\
&\iff\\
&diam(E)<+\infty
\end{split}$$
# Definizione | Spazio metrico totalmente limitato
Sia $(X,d)$ uno [[Spazi metrici|spazio metrico]], sia $E\subseteq X$.
$E$ si dice totalmente limitato se vale
$$\forall \epsilon>0\ \exists n \in \mathbb{N}, \exists \underbrace{x_{1},x_{2},\ldots,x_{n}}_{punti\ di\ X}\in X:E\subseteq\bigcup_{i=1}^{n}B_\epsilon(x_i)$$
# Osservazione
In generale i concetti di [[Spazio metrico limitato e totalmente limitato#Definizione Spazio metrico limitato|spazio metrico limitato]] e [[Spazio metrico limitato e totalmente limitato#Definizione Spazio metrico totalmente limitato|spazio metrico totalmente limitato]] non sono equivalenti.
$$\mbox{totalmente limitato}\Rightarrow\mbox{limitato}$$
In $\mathbb{R}^{n}$ possiamo dire che i due concetti sono equivalenti.
Non sono equivalenti ad esempio in $X=\{\mbox{le successioni} (a_{n})\subseteq \mathbb{R}:\sum_{n=1}^{+\infty}a_{n}^{2}<+\infty\}$
Definisco la distanza, se $a =(a_{n})$ e $b=(b_{n})$,
$d(a,b)=(\sum_{n=1}^{+\infty}|a_{n}-b_{n}|^{2})^{\frac{1}{2}}$

> Moralmente $X=\mathbb{R}^{\mathbb{N}}$

Definisco $E=B_{1}(\bar 0),\qquad \bar 0 = (0,0,\ldots,0)$$B_{1}(\bar0)=\{a=(a_n):d(a,\bar0)<1\}=\{a=(a_n):(\sum_{n=1}^{+\infty}a_{n}^{2})^{\frac{1}{2}}<1\}$Si nota facilmente che $B_{1}(\bar0)$ è limitato, dato che basta prendere una palla centrata in $\bar0$ con raggio $\ge 1$.

#esercizio-analisi 
