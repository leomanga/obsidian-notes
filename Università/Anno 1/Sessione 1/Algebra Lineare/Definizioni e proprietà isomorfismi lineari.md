---
pagina: 248
collegamenti:
  - "[[Proprietà funzioni lineari]]"
  - "[[Isomorfismo]]"
---
# Definizioni
Sia $\mathcal{L}(V)$ spazio degli isomorfismi lineari.
- Se $f\circ f = f$ allora si dice <mark style="background: #FFB86CA6;">IDEMPOTENTE</mark>([[Proiezione ortogonale]], [[Proiezione di A lungo B]]) ^79a5a5
- Se $f\circ f=\mbox{identità}$ allora si dice <mark style="background: #FFB86CA6;">INVOLUTORIA</mark>([[Riflessione]]) ^fcae3c
- Se $\exists n \in \mathbb{N}: f\circ f\circ \ldots(n volte) \circ f = \mbox { identità}$ e $f^{n-1}\not = \mbox{ identità}$ allora si dice che $f$ è <mark style="background: #FFB86CA6;">PERIODICA DI ORDINE </mark>$n$. ^20361d
- Se $\exists n \in \mathbb{N}:f^n=0(\mbox{funzione nulla})$ e $f^{n-1}\not = 0$ si dice che $f$ è <mark style="background: #FFB86CA6;">NILPOTENTE DI ORDINE</mark> $n$. ^c6ba6b

# Proprietà
- Siano $f,g \in \mathcal{L}(V)\quad f\circ g \not = g\circ f$ (non vale la proprietà commutativa per la composizione)

# Teorema 1
Se $\varphi \in \mathcal{L}(V)$ commuta con qualsiasi funzione di $\mathcal{L}(V)$ se e solo se $\varphi$ è una [[Omotetia di ragione a]].
Cioè $\varphi \circ \psi = \psi \circ \varphi\quad \forall \psi \in \mathcal{L}(V)\iff\varphi = a I, a\in \mathbb{K}$

# Teorema 2
Per ogni matrice appartenente a $M_n(\mathbb{K})$ esiste sempre una [[Trasformazione lineare#Proposizione 4 matrice rappresentativa di $ varphi$ rispetto alle basi E ed F|matrice rappresentativa]] di un isomorfismo lineare.
Inoltre $dim(\mathcal{L}(V_n))=\dim(M_n(\mathbb{K})) = n^2$.
$$\mathcal{L(V_{n})}\cong M_n(\mathbb{K})$$
