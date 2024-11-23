---
pagina: 218
collegamenti:
  - "[[Vettori ortogonali]]"
  - "[[Equivalenza]]"
---
# Teorema
In uno [[Spazio euclideo]] di [[Dimensione]] finita o numerabile, esiste sempre una [[Base ortogonale e ortonormale|base ortogonale]] e quindi anche una ortonormale.

# Procedimento
In uno [[Spazio euclideo]] di [[Dimensione]] finita o numerabile permette di costruire un insieme $\mathbb{Y}=\{y_1,y_2,\ldots,y_n\}$ di [[Vettore|vettori]], a partire da un insieme $\mathbb{X}=\{x_1,x_2,\ldots,x_n\}$ [[Dipendenza lineare|linearmente indipendente]], con queste proprietà
1) $0 \not \in \mathbb{Y}$
2) $\mathbb{Y}$ è [[Insieme ortogonale]]
3) $\forall k\quad (x_i)_{i=1}^{k}\sim(y_i)_{i=1}^{k}\qquad\Rightarrow \mathbb{X}\sim\mathbb{Y}$ 
4) Se per qualche $n$ l'insieme $\{x_1,x_2,\ldots,x_n\}$ è già ortogonale, allora $y_1=x_1,y_2=x_2,\ldots$
- Dalla 1 e 2 , da "[[Insieme ortogonale#Proposizione]]" possiamo anche affermare che $\mathbb{Y}$ è [[Dipendenza lineare|linearmente indipendente]].
- Per tutti i passi guardare appunti e lucidi 9.11,9.12,9.13

Per trovare tutte le $y_n$ sarà necessario fare questo calcolo per ognuna:
$$\begin{split}
y_n&=x_n-\sum_{i=1}^{n-1}\frac{<x_n,y_i>}{<y_i,y_i>}y_i=\\
&=x_n-\sum_{i=1}^{n-1}\pi_{y_i}^{\perp}x_n
\end{split}$$
- $\pi_{y_i}^{\perp}$ è la [[Proiezione ortogonale]].

