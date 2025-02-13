Lo scopo è, data una successione di punti $\{x_{i}\}$ e le coppie di valori $\{(x_{i},f_{i})\}$, quello di trovare una funzione $g$ che verifichi
$$g(x_{i})=f_{i}\quad \forall i=1,\ldots,n$$
Vogliamo poi poter valutare la funzione $g$ in $\bar x\not = x_{i}, i=1,\ldots,0$

Se definiamo $$\xi_{1}=\min \{x_0,x_1,\ldots,x_{n\}\quad}\xi_{2}=\max\{x_{0},x_{1},\ldots,x_{n}\}$$
Parleremo di
- Interpolazione se $\bar x \in [\xi_{1},\xi_{2}]$
- Estrapolazione se $\bar x\not\in [\xi_{1},\xi_{2}]$

In base allo spazio di funzioni scelto per $g$ cambia il tipo di interpolazione
In generale si sceglie una base $\{\phi_j(x),i=0,1,\ldots,n\}$ ed esprimiamo $$g(x)=\sum_{j=0}^{n}a_{j}\phi_{j}(x)$$
Cercheremo quindi $a_0,a_1,\ldots,a_{n}$ tali che
$$g(x_{i})=\sum_{j=0}^{n}a_{j}\phi_{j}(x_i)=f_{i}, \forall i = 0,1,\ldots, n$$
Avremo
[[Interpolazione polinomiale]]


>[!def] Interpolazione trigonometrica
>$$g(x)=a_{0}+a_1\cos(x)+b_1\sin(x)+\ldots$$
