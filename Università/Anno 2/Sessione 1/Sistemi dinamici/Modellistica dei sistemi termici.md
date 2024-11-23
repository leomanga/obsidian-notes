# Forno
$$\frac{d Q}{dt}(t)=C\cdot \frac{dT}{dt}(t)$$
dove $C$ è la [[Calore#^2c368a|capacità termica]].

>[!I/O]
>$$C\cdot \dot{y}(t)=u_{1}(t)-k(y(t)-u_{2}(t))$$
>$y(t)=T(t)$ ([[Temperatura]])
>$u_{1}(t)=p(t)$ ([[Potenza]])
>$u_{2}(t)=T_{e}(t)$ (Temperatura esterna)
>$k$ è il coefficiente di conduttività termica

>[!I/S/O]
> $$\begin{cases}
> \dot{x}(t)=\begin{bmatrix}-\frac{k}{C}\end{bmatrix}x(t)+\begin{bmatrix}\frac{1}{C} & \frac{k}{C}\end{bmatrix}u(t)\\
> y(t)=[1]x(t)+\begin{bmatrix}0&0\end{bmatrix}u(t)
> \end{cases}$$
>$x(t)=T(t)$ ([[Temperatura]])
 $u_{1}(t)=p(t)$ ([[Potenza]])
>$u_{2}(t)=T_{e}(t)$ (Temperatura esterna)
> 

