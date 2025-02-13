>La forma sarà:
>$$g(x)=\sum_{k=0}^{n}a_{k}x^{k}$$
>
>[!thm]
>Esiste un unico polinomio di grado massimo $n$ che assume valori $f_{i}\ \forall i$ in corrispondenza di $(n+1)$ punti distinti $x_{i}$ 

La soluzione ottimale si ha con tutte funzioni linearmente indipendenti fra di loro, che assumono la forma
$$\ell_{i}^{(n)}(x)=\frac{\prod_{j=0,j\not=i}^{n}(x-x_{j})}{\prod_{j=0,j\not=i}^{n}(x_{i}-x_{j})}$$
e prendono il nome di **funzioni fondamentali di Lagrange**.

La forma del polinomio interpolante sarà
$$\mathcal{L}_{n}(x,f)=f_{0}\ell_0$$