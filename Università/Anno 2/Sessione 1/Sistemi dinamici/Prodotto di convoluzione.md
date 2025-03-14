Date due funzioni $f(t)$ e $g(t)$, si definisce il **prodotto di convoluzione** la funzione (nel caso in cui si ha un sistema causale) #TODO
$$
h(t)=f(t) * g(t) =\int_{0}^{t}f(t-\tau)g(\tau)d\tau=g(t)*f(t)
$$
In generale la definizione è
$$g(t)*f(t)=f(t)*g(t)=\int_{-\infty}^{\infty}g(\tau)f(t-\tau)d\tau$$

# Tempo discreto

$$h(k)=f(k)*g(k)=\sum_{i=0}^{k}f(k-i)g(i)$$
