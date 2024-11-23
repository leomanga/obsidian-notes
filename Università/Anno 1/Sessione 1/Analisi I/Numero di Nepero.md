---
aliases:
  - Numero di Eulero
---
### Numero di Nepero-1
Dimostrazione con il [[Binomio di Newton]].
$$\sum_{k=0}^{+\infty}{\frac{1}{k!}}= e$$
### Derivazione
Si dimostra con [[Formula di Taylor]]
$$\sum_{k=0}^{+\infty}{\frac{a^k}{k!}}= e^a$$

### Carattere di e
Siamo in [[Serie numeriche a termini di segno costante#Studio del carattere di una serie]]

Si sfrutta la [[Dimostrazione per induzione]] per dimostrare che $$k! \ge 2^{k-1}\ \forall k \in \mathbb{N}$$
Quindi
$$\frac{1}{k!} \le \frac{1}{2^{k-1}}\ \forall k \in \mathbb{N}$$
Con il [[Serie numeriche a termini di segno costante#Confronto|teorema del confronto]] segue che
$$
\begin{equation}
\begin{split}
\sum_{k=0}^{+\infty}\frac{1}{k!} = 1+\sum_{k=1}^{+\infty}\frac{1}{k!} \le
1+\sum_{k=1}^{+\infty}\frac{1}{2^{k-1}} &= 1+\sum_{h=0}^{+\infty}\frac{1}{2^{h}}= \\&= 1+\frac{1}{1-\frac{1}{2}} = 3
\end{split}
\end{equation}
$$
In questo modo sappiamo anche che e $\le$ 3 e riusciamo a calcolare velocemente che è > $\frac{8}{3}$
### Irrazionalità di e
Da fare
-[[Criteri di convergenza serie a termini positivi]]
-[[Dimostrazione per assurdo]]

### Numero di Nepero-2
$$e = \lim_{n\to +\infty}(1+ \frac{1}{n})^n$$
#dimostrazione-da-fare 
[[Bernoulli I e II#Bernoulli I]]
### Derivazione 2
$$e^{k}= \lim_{n\to +\infty}(1+\frac{k}{n})^n$$