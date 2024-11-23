Un tipo di coordinate sferiche può essere
$$x= \rho\cos(\varphi)\cos(\theta)\quad y=\rho\cos(\varphi)\cos(\theta)\quad z=\rho\sin(\varphi)$$
Dove
$\rho \in [0,+\infty]$
$\theta\in[0,2\pi]$
$\varphi\in (-\frac{\pi}{2}, \frac{\pi}{2})$

Il $\cos(\theta)$ rappresenta la lunghezza della proiezione sul piano formato da $x$ e $y$.

![[Coordinate sferiche.png]]
# Differentials
>[!proposition] Differential length
$$d\vec{l} = d\rho\cdot\hat \rho+\rho\cdot d\varphi\cdot \hat\varphi+\rho\sin\varphi\cdot d\theta\cdot \hat\theta$$

^ce13bf

>[!proposition] Differential surface areas
$$d\vec{s}_{\rho}=\rho^{2}\sin\varphi d\varphi d\theta\hat\rho$$
$$d\vec{s}_{\phi}=\rho\sin\varphi d\rho d\theta\hat\varphi$$
$$d\vec{s}_{\theta}=\rho d\rho d\varphi \hat\theta$$

>[!proposition] Differential volume
$$dV = \rho^{2}\sin\varphi d\rho d\varphi d\theta$$

# Matrice da coordinate ortogonali a sferiche
$$
\begin{bmatrix}
A_{\rho}  \\ A_{\varphi} \\ A_{\theta} 
\end{bmatrix} =
\begin{bmatrix}
\sin\varphi\cos\theta &\sin\varphi\sin\theta &\cos\varphi \\ 
\cos\varphi\cos\theta &\cos\varphi\sin\theta &-\sin\varphi \\ 
-\sin\theta &\cos\theta &0
\end{bmatrix}
\begin{bmatrix}
A_{x} \\ A_{y} \\ A_{z}
\end{bmatrix}
$$
