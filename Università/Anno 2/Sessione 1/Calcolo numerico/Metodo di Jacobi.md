Dato il sistema lineare $Ax=b,\quad A\in \mathbb{R}^{n\times n}, b\in \mathbb{R}^{n}$
Cerchiamo una successione $\{x^{(k)}\}$ che converge alla soluzione $x^{*}$.

Assegnato $x^{(0)}\in \mathbb{R}^{n}$
$$x_{i}^{(k+1)}=\frac{1}{a_{ii}}[b_{i}-\sum_{j=1,j\not=i}^{n}a_{ij}x_{j}^{(k)}]\quad a_{ii}\not = 0$$

Formulazione matriciale
$$A = L+D+U$$
$$A=\begin{bmatrix}0 &0&\ldots&0\\a_{21}& 0&\ddots&\vdots\\\vdots&\ddots&\ddots&\vdots\\a_{n1}&a_{n2}&\ldots&0\end{bmatrix}\quad D=\begin{bmatrix}a_{11}&0 &\ldots&0\\0&a_{22}&\ddots&\vdots\\\vdots&\ddots&\ddots&\vdots\\0&\ldots&\ldots&a_{nn}\end{bmatrix}\quad U=\begin{bmatrix}0 &a_{12}&\ldots&a_{1n}\\0& 0&\ddots&a_{2n}\\\vdots&\ddots&\ddots&\vdots\\0&0&\ldots&0\end{bmatrix}$$


$$Dx^{(k+1)}=-(L+U)x^{(k)}+b$$
>[!thm]
>Il metodo di Jacobi converge se $A$ è [[Matrice diagonale dominante|diagonale dominante]] in senso forte oppure se $A^{T}$ è diagonale dominante in senso forte
>