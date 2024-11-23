---
aliases:
  - Vettori proporzionali
  - Vettori non proporzionali
  - linearmente indipendenti
  - linearmente dipendenti
---
# Definizione | dipendenza
Sia $V$ spazio vettoriale e $\mathbb{A} \subseteq V$
$\mathbb{A}$ è linearmente dipendente se e solo se
$$\exists x \in \mathbb{A}\mbox{ tale che }x\in L(\mathbb{A}\setminus\{x\})$$
- <mark style="background: #FFB86CA6;">OGNI INSIEME DI VETTORI CHE CONTIENE IL VETTORE NULLO E' LINEARMENTE DIPENDENTE.</mark>
Esempi pg.93

# Definizione | indipendenza
Sia $V$ spazio vettoriale e $\mathbb{A} \subseteq V$
$\mathbb{A}$ è linearmente indipendente se e solo se
$$\forall x\in \mathbb{A}: x\not \in L(\mathbb{A}\setminus\{x\})$$
Esempi pg.94

# Proposizione 1
Sia $V$ spazio vettoriale e $\mathbb{X} \subseteq V$
($\mathbb{X}$ è linearmente dipendente) $\iff \exists x_1,x_2,\ldots,x_{n}\in \mathbb{X}\quad x_{i}\not = x_{j}\quad e\quad \exists a_1,a_2,\ldots,a_{n}\in \mathbb{K}$ 
tale che $(a_1x_{1}+a_2x_2+\ldots+a_nx_{n}= 0) \land  ((a_{1}\not=0)\lor(a_{2}\not=0)\lor\ldots\lor(a_{n}\not=0))$
Il vettore nullo si può ottenere come [[Combinazione lineare]] di vettori di $\mathbb{X}$ con coefficienti NON tutti nulli.
#dimostrazione-da-fare 

# Caso particolare
Sia $\mathbb{X} = \{x_1,x_2,\ldots,x_n\}$
$$(\mathbb{X}\mbox{ è linearmente dipendente}) \iff \begin{split}\\&(\exists a_1,a_2,\ldots,a_{n}\in \mathbb{K}\mbox{ non tutti nulli} : \\
&a_1x_1+a_2x_2+\ldots+a_nx_{n}= 0)\end{split}$$

# Proposizione 2
Sia $V$ spazio vettoriale e $\mathbb{X} \subseteq V$
$$ \begin{split} 
&X \mbox{ è linearmente} \\ &\mbox{indipendente}\end{split} \iff 
\left(\begin{split}  &\forall x_1,x_2,\ldots,x_{n} \in \mathbb{X}\\
&\forall a_1,a_2,\ldots,a_{n} \in \mathbb{K}\\
&(a_1x_1+a_2x_2+\ldots+a_nx_{n}= 0) \Rightarrow\\
&\qquad a_{1}= a_2=\ldots=a_{n}= 0 
\end{split}\right)$$
# Proposizione 3
$$
\left(\begin{split}
&\mathbb{X} \subseteq V\\
&\mathbb{X} \mbox{ linearmente indipendente}\\
\end{split}\right) \iff 
\left(
\begin{split}
&a_1x_1+a_2x_2+\ldots+a_nx_{n}\\
&=\\
&b_1x_1+b_2x_2+\ldots+b_nx_n\\
&\Rightarrow a_{i}=b_i\qquad\forall i = 1,\ldots,n
\end{split}
\right)$$
#dimostrazione-da-fare PG 96

# Proposizione 4
[[Equivalenza]]
$$\left(\begin{split}
&\mathbb{X} \subseteq V\\
&\mathbb{X} \mbox{ linearmente dipendente}\\
\end{split}\right) \iff 
\left(
\begin{split}
\exists \mathbb{Y} \subset \mathbb{X} \mbox{ tale che } \mathbb{X} \sim \mathbb{Y}
\end{split}
\right)
$$
$$\left(\begin{split}
&\mathbb{X} \subseteq V\\
&\mathbb{X} \mbox{ linearmente indipendente}\\
\end{split}\right) \iff 
\left(
\begin{split}
\forall \mathbb{Y} \subseteq \mathbb{X},\ \ L(\mathbb{Y}) \subset L(\mathbb{X})
\end{split}
\right)
$$
# Esercizio pg 97-98

# Lemma di Steinitz
![[Lemma di Steinitz]]
