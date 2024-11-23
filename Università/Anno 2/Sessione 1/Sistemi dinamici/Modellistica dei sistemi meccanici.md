# Masse in transizione
$$M\ddot{z}(t)=f(t)$$
![[Masse.excalidraw]]
# Elementi elastici
(molle)
$$f(t)=k(z_{2}(t)-z_{1}(t))$$
$k$ coefficiente elastico
![[Elementi elastici.excalidraw]]
# Elementi dissipativi
(smorzatori)
$$f(t)=\beta(\dot{z}_{1}(t)-\dot{z}_{1}(t))$$
![[Elementi dissipativi.excalidraw]]

# Massa-molla-smorzatore

>[!I/O]
>$$M\ddot{y}(t)+\beta\dot{y}(t)+ky(t)=u(t)$$
>$y(t)= z(t)\qquad u(t)=f(t)$

>[!I/S/O]
>$$\begin{cases}
>\dot{x}(t)=\begin{bmatrix}0 &1\\ \frac{-k}{M} & \frac{-\beta}{M}\end{bmatrix}x(t)+\begin{bmatrix}0\\ \frac{1}{M} \end{bmatrix}u(t)\\
>y(t) = \begin{bmatrix}1&0\end{bmatrix}x(t) + \begin{bmatrix}0\end{bmatrix}u(t)
>\end{cases}$$
>$x_{1}(t) = z(t)\qquad x_{2}(t)=\dot{z}(t)\qquad u(t)=f(t)$

# Masse in rotazione
$$J\ddot{\theta}(t)=C(t)$$
$J$ [[Moto di rotazione#^a5ff25|momento di inerzia]], $C(t)$ coppia([[Moto di rotazione]])

![[Masse in rotazione.excalidraw]]
# Elementi elastici di rotazione
$$C(t)=k(\theta_{2}(t)-\theta_{1}(t))$$
![[Elementi elastici di rotazione.excalidraw]]
# Elementi dissipativi di rotazione
$$C(t)=\beta(\dot{\theta}_{2}(t)-\dot{\theta}_{1}(t))$$

$\theta_1$ è la rotazione di un fluido esterno, $\theta_{2}$ è la rotazione dell’elemento interno. (Immagina un tubo che ruota nell’olio)
![[Elementi dissipativi di rotazione.excalidraw]]