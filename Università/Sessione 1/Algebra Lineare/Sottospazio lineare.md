---
aliases:
  - Sottospazio vettoriale
  - sottospazio vettoriale
  - sottospazio lineare
  - sottospazi vettoriali
  - sottospazi lineari
---
 # Definizione
Sia $V$ uno [[Spazio vettoriale|spazio vettoriale]] su $\mathbb{K}$.
Sia $\mathbb{X} \subseteq V$ un insieme di vettori non vuoto.
$\mathbb{X}$ è un **SOTTOSPAZIO LINEARE DI V** o **SOTTOSPAZIO VETTORIALE** se:

- [^1] | $v_{1}+ v_{2}\in \mathbb{X}, \ \ \ \forall v_{1}, v_{2}\in \mathbb{X}$
- [^2] | $\lambda \cdot v \in \mathbb{X}, \ \ \ \forall \lambda \in \mathbb{K}, \forall v \in \mathbb{X}$

Le proprietà [^1] e [^2] si possono riscrivere
$$av_{1}+ bv_{2}\in \mathbb{X}\ \ \ \forall a,b \in \mathbb{K}, \forall v_{1}, v_{2}\in \mathbb{X}$$
##### Dalle proprietà di chiusura:
- $0 \in \mathbb{X}$ ($\lambda = 0$)
- $\forall v \in \mathbb{X}$     $-v \in \mathbb{K}\ \ \ (\lambda = -1$) 
$\Rightarrow (\mathbb{X}, +, \cdot)$ è uno spazio vettoriale su $\mathbb{K}$ a sua volta ($+\ e\ \cdot$ sono di V)
$\iff \mathbb{X}$ è un sottospazio lineare di V.

##### Sottospazi lineari impropri
Sia V uno spazio vettoriale su $\mathbb{K}$, allora V e {0} sono sottospazi lineari di V, e vengono detti **sottospazi lineari impropri**
## Proposizione 1
Sia $\xi$ una [[equazione lineare omogenea]] in $n$ variabili.
1) Se $\xi$ ammette almeno un coefficiente non nullo, allora l'insieme delle soluzioni di $\xi$ è un sottospazio lineare di $V_n(\mathbb{K})$ [[Isomorfismo|isomorfo]] a $V_{n-1}(\mathbb{K})$
2) Se $\xi$ è l'equazione nulla, allora l'insieme delle soluzioni di $\xi$ è un sottospazio lineare di $V_n(\mathbb{K})$ 
#dimostrazione-da-fare 

## Proposizione 2
Sia $V$ uno spazio vettoriale e sia $\{x_i\}_{i\in I}$ un insieme di sottospazi lineari di V.
$$\Rightarrow \bigcap_{i\in I}x_{i}\ \ \  è\ un\ sottospazio\ lineare.$$
#dimostrazione-da-fare 
###### **NON È VERO CHE L'UNIONE DI SOTTOSPAZI LINEARI È UN SOTTOSPAZIO LINEARE**

## Corollario 1
Le soluzioni di un [[sistema di equazioni lineari omogenee]] in n incognite è un sottospazio lineare di $V_n(\mathbb{K})$.

## Esempi
PAG 59 APPUNTI PER DISEGNI
1) $\xi_{1}:=ax+by+cz = 0$
	La soluzione è un sottospazio lineare che indica un piano passante per l'origine. 
	$Sol(\xi_1)$ isomorfa a $V_2(\mathbb{R})$
2) $$ \xi_{2}:=\begin{cases}a_1x+b_1y+c_1z = 0\\ a_2x+b_2y+c_2z = 0\end{cases}$$
	Rappresenta l'intersezione fra due piani, e coincide con una retta passante per l'origine.

# Proposizione 3
Sia
$\xi:= a_1x_{1}+ \ldots+a_nx_{n}= a$
$\xi_{0}:= a_1x_{1}+ \ldots+a_nx_{n}= 0$ [^3]

$P = (p_1,\ldots,p_n)$ è soluzione di $\xi$
##### Allora
$$P + Sol(\xi_{0}):= \{P + y : y\in Sol(\xi_{0}) \} = Sol(\xi)$$
										Dove $Sol(\xi)$ è l'insieme delle soluzioni di $\xi$.
$P + Sol(\xi_{0})$ viene detto <mark style="background: #FFB86CA6;">SPAZIO AFFINE</mark>.
#dimostrazione-da-fare 

# Più piccolo sottospazio lineare di V contenente $\mathbb{X}$
$L(\mathbb{X})$ è il più piccolo sottospazio lineare di $V$ che contiene $\mathbb{X}$.
- Viene chiamato <mark style="background: #FFB86CA6;">sottospazio lineare generato dall'insieme</mark> $\mathbb{X}$, 
- E $\mathbb{X}$ è detto <mark style="background: #FFB86CA6;">insieme di generatori</mark> di $L(\mathbb{X})$.
###### Proprietà
1) $L(\mathbb{X})$ è un sottospazio lineare.
2) $\mathbb{X} \subseteq L(\mathbb{X})$
3) Per ogni $y$ sottospazio lineare di $V$	$$\mathbb{X} \subseteq y \Rightarrow L(\mathbb{X}) \subseteq y$$
4) $L(0) = \{0\} = L(\varnothing)$
5) $L(V) = V$
# Proposizione 4
Sia $V$ spazio vettoriale e $\mathbb{X} \subseteq V$
Indichiamo con $\mathcal{L}_{\mathbb{X}} = \{y:(y\ sottospazio\ lineare\ di\ V) \land (\mathbb{X} \subseteq y)    \}$
$$\Rightarrow L(\mathbb{X}) = \bigcap_{y\in \mathcal{L}_{\mathbb{X}}}y$$
#dimostrazione-da-fare 

Esempi pag 65 appunti.
# Proposizione 5
Sia $V$ spazio vettoriale su $\mathbb{K}$ e $\mathbb{X} \subseteq V$
Allora
$$L(\mathbb{X}) = \{\sum_{i=1}^{n}a_ix_i:x_{i}\in \mathbb{X},a_1,a_2,\ldots,a_{n} \in \mathbb{K}, n \in \mathbb{N}\}$$
Rappresenta tutte le possibili combinazioni lineari che si possono scrivere con i vettori di $\mathbb{X}$.

Per convenzione 
$$\sum_{i=1}^{n}a_ix_i:x_{i} = 0$$
# Proprietà
Sia $V$ uno spazio vettoriale su $\mathbb{K}$ e $\mathbb{X},\mathbb{Y}$, insiemi di vettori di $V$.

1) $\mathbb{X} = L(\mathbb{X}) \iff \mathbb{X}$ è un sottospazio lineare.
2) $L(\{0\}) = L(\varnothing) = \{0\}$
3) $L(L(\mathbb{X})) = L(\mathbb{X})$
4) $\mathbb{X} \subseteq \mathbb{Y} \Rightarrow L(\mathbb{X}) \subseteq L(\mathbb{Y})$ (Non vale l'implicazione inversa)
5) $\mathbb{X} \subseteq L(\mathbb{Y}) \iff \mathbb{X} \subseteq L(\mathbb{Y})$
6) $v \in L(\mathbb{X})\iff L(v) \subseteq L(\mathbb{X})$
7) $L(\mathbb{X}) = L(\mathbb{Y}) \iff (\mathbb{X} \subseteq L(\mathbb{Y})) \land (\mathbb{Y} \subseteq L(\mathbb{X}))$
8) $(x \in L(\mathbb{Y})) \land (x\not=0) \Rightarrow L(\mathbb{X}) = L(\mathbb{Y})$ 
9) $L(\mathbb{X} \cap \mathbb{Y} ) \subseteq L(\mathbb{X}) \cap L(\mathbb{Y})$
10) $L(\mathbb{X}) \cup L(\mathbb{Y}) \subseteq L(\mathbb{X} \cup \mathbb{Y})$
11) $L(L(\mathbb{X}) \cup L(\mathbb{Y})) = L(\mathbb{X} \cup \mathbb{Y})\qquad \forall \mathbb{X},\mathbb{Y}\subseteq V$
# Proposizione 6
Siano A e B due sottospazi lineari di V.
$A \cup B$ è un [[Sottospazio lineare#Definizione|sottospazio lineare]] se e solo se $(A \subseteq B) \lor (B \subseteq A)$

# Teorema
Dati $A$ e $B$ 2 sottospazi lineari di $V$.
Allora $A+B = L(A \cup B)$

# Proposizione 7
Sia $E_n(\mathbb{K})$ (vale anche per $EO_n(\mathbb{K})$) lo spazio vettoriale delle equazioni lineari in $n$ variabili a coefficienti in $\mathbb{K}$.
$$\xi \in L(\xi_1,\xi_2,\ldots,\xi_{m})\Rightarrow Sol(\xi_1,\xi_2,\ldots,\xi_{m}) \leftarrow\mbox{ (Insieme soluzioni equazioni lineari) }\subseteq Sol(\xi)$$

$E_n(\mathbb{K}) \cong V_{n+1}(\mathbb{K})$
(Si usa quando si parla di sistemi)
Ogni soluzione del sistema con $\xi_{1}$ e $\xi_2$ è anche soluzione di $\xi = \xi_{1}+ \xi_{2}$

# Corollario 2
Lavoriamo in $E_n(\mathbb{K})$.
$\xi_{1}^{'}, \xi_{2}^{'},\ldots,\xi_{s}^{'} \in L(\xi_1,\xi_2,\ldots,\xi_{m}) \Rightarrow$
 $$ Sol(\xi_{1}, \xi_{2},\ldots,\xi_{m}) \subseteq \begin{cases}Sol(\xi_1^{'})\\ Sol(\xi_{2}^{'})= Sol(\xi_{1}^{'})\cap\dots \cap Sol(\xi_{s}^{'})\\
\ldots\\
Sol(\xi_{s}^{'})\end{cases}$$
Cioè
$$Sol(\xi_{1}, \xi_{2},\ldots,\xi_{m}) \subseteq Sol(\xi_1^{'},\xi_2^{'},\ldots,\xi_s^{'})$$

# Corollario 3
Lavoriamo in $E_n(\mathbb{K})$
$L(\xi_1,\xi_2,\ldots,\xi_{m}) = L(\xi_1^{'},\xi_2^{'},\ldots,\xi_{s}^{'}) \Rightarrow$
$$Sol(\xi_1,\xi_2,\ldots,\xi_{m}) = Sol(\xi_1^{'},\xi_2^{'},\ldots,\xi_{s}^{'})$$
- Sostituendo delle equazioni lineari con delle combinazioni lineari, lo spazio delle soluzioni non cambia.

[^1]: Proprietà di chiusura rispetto alla somma
[^2]: Proprietà di chiusura rispetto alla moltiplicazione
[^3]: Equazione omogenea associata ad $\xi$
