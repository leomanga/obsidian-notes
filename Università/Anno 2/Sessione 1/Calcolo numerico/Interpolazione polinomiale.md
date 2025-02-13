>La forma sarà:
>$$g(x)=\sum_{k=0}^{n}a_{k}x^{k}$$
>

>[!thm]
>Esiste un unico polinomio di grado massimo $n$ che assume valori $f_{i}\ \forall i$ in corrispondenza di $(n+1)$ punti distinti $x_{i}$ 

La soluzione ottimale si ha con tutte funzioni linearmente indipendenti fra di loro, che assumono la forma
$$\ell_{i}^{(n)}(x)=\frac{\prod_{j=0,j\not=i}^{n}(x-x_{j})}{\prod_{j=0,j\not=i}^{n}(x_{i}-x_{j})}$$
e prendono il nome di **funzioni fondamentali di Lagrange**.

La forma del polinomio interpolante sarà
$$\mathcal{L}_{n}(x,f)=f_{0}\ell_0^{(n)}(x)+f_{1}\ell_1^{(n)}(x)+\ldots+f_{n}\ell_n^{(n)}(x)$$
Questo polinomio presenta difficoltà quando iniziano ad esserci tante coppie di punti, dato che le funzioni fondamentali dipendono da tutti i punti.

Usiamo il polinomio interpolante di Newton
$$N_{n}(x,f)=f_{0}+\sum_{k=1}^{n}C_{k}w_{k}(x)$$
dove $w_{k}=(x-x_{0})(x-x_{1})\ldots(x-x_{k})$ e $$C_{k}=\frac{f_{k}-\mathcal{L}_{k-1}(x_{k},f)}{w_{k}(x_k)}$$
Si può studiare l’errore di interpolazione

Abbiamo che
$$e(x)=w_{n+1}(x)R(x)$$
dove $R(x)=\frac{f^{n+1}(\epsilon)}{(n+1)!}\le \frac{M}{(n+1)!}$
se $\forall x\in [a,b]$ si ha $f^{(n+1)(x)}\le M$
Questo se $f\in C^{n+1}[a,b]$, sennò se $f\not \in $