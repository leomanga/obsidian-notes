---
collegamenti:
  - "[[Dipendenza lineare]]"
pagina: 99
---
# Lemma spazi lineari
[[Cardinalità]]
Sia $V$ spazio vettoriale e $\mathbb{X},\mathbb{Y}\subseteq V$
$$
\left(
\begin{split}
&\mathbb{Y} \subseteq L(\mathbb{X})\\
&card(\mathbb{Y}) > card(\mathbb{X})
\end{split}
\right)\Rightarrow
\left(
\begin{split}
\mathbb{Y} \mbox{ è linearmente dipendente}
\end{split}
\right)
$$
### Applicazione 
$V  = V_n(\mathbb{R})$
$\mathbb{X} = \{U_1,U_2,\ldots,U_n\}$
$L(\mathbb{X}) = V_n(\mathbb{R})$

-<mark style="background: #FFB86CA6;"> Ogni insieme di vettori di $V_n(\mathbb{R})$ che contenga almeno $n+1$ vettori è linearmente dipendente.</mark>
#dimostrazione-da-fare 

# Contronominale
Sia $V$ spazio vettoriale e $\mathbb{X},\mathbb{Y}\subseteq V$
$$
\left(
\begin{split}
\mathbb{Y} \mbox{ è linearmente indipendente}
\end{split}
\right)
\Rightarrow
\left(
\begin{split}
&\mathbb{Y} \not\subseteq L(\mathbb{X})\\
&card(\mathbb{Y}) \le card(\mathbb{X})
\end{split}
\right)$$
# Lemma spazi affini
Sia $\mathbb{S}$ uno spazio affine
$$
\left(
\begin{split}
&\mathbb{X} \subseteq \mathbb{S})\\
&card(\mathbb{X}) > \dim(\mathbb{S})+1
\end{split}
\right)\Rightarrow
\left(
\begin{split}
\mathbb{X} \mbox{ è geometricamente dipendente}
\end{split}
\right)
$$