---
pagina: 247
collegamenti:
  - "[[Trasformazione lineare]]"
---
# Proprietà
Sia $V$ [[Spazio vettoriale|spazio vettoriale]] con $dim(V)=n$.
Sia $\mathbb{E} = (E_1,E_2,\ldots,E_n)$ [[Base]] di $V$.
$\mathcal{L}(V)=\{f:V\to V\mbox{ è funzione lineare}\}$
Allora
- $f_1+f_{2}: V\to V$ è funzione lineare
		$(f_{1}+f_{2})(x)=f_1(x)+f_2(x),\quad\forall x \in V$
- $\forall \lambda \in \mathbb{K},\quad \forall f \in \mathcal{L}(V)$
		$\lambda f: V\to V$ è funzione lineare
		$(\lambda f)(x)=\lambda f(x)\quad \forall x \in V$
- Funzione nulla $\in \mathcal{L}$
- $\forall f\in \mathcal{L}(V)$
		$(-f):V\to V$ è funzione lineare
		$(-f)(x)=-f(x)\quad \forall x \in V$

Dati questi punti possiamo dire che $\mathcal{V}$ è uno [[Spazio vettoriale]].

# Composizione
Siano $f,g \in \mathcal{L}(V)$. Posso considerare la loro composizione
$$\begin{split}
&f \circ g:V\to V\\
&(f\circ g)(x)=f(g(x)),\quad \forall x\in V
\end{split}
$$
