---
aliases:
  - Delta di Dirac
  - delta di Dirac
---
# Tempo continuo
Data $\delta_{\epsilon}(t)=\begin{cases}  \frac{1}{\epsilon}\mbox{ se }0\le t\le \epsilon\\ 0\mbox{ altrimenti}   \end{cases}$


```functionplot
---
title: 
xLabel: 
yLabel: 
bounds: [-0.5,2.5,-0.5,1]
disableZoom: true
grid: true
---
f(x) = x < 0 ? 0 : (x> 2 ? 0 : 1/2)
```

Il segnale impulsivo $\delta(t)$ sarà
$$\delta(t)=\lim_{\epsilon\to 0}\delta_{\epsilon}(t)$$
Dato che $\delta_{\epsilon}$ ha area pari a 1, possiamo notare delle proprietà di $\delta(t)$
1) $\int_{-\infty}^{\infty}\delta(t)=1$
2) Se $f(t)$ è [[Funzioni continue|continua]], $\int_{-\infty}^{\infty}f(t-\tau)\delta(\tau)d\tau = f(t)=\int_{-\infty}^{\infty}f(\tau)\delta(t-\tau)d\tau =f(t)$

Inoltre, dato che per $\epsilon \to 0$ $$\delta(t)=\frac{d}{dt}\mathbb{1}(t)$$
Allora si può vedere l’impulso come derivata del [[Gradino unitario]].

>[!prp] Trasformata di Laplace del segnale impulsivo
>$$\mathcal{L}[\delta(t)\cdot \mathbb{1}(t)]=1$$
>**L’impulso è l’elemento unitario nella trasformata di Laplace**
>[[Trasformata di Laplace]]

# Tempo discreto
$$\delta(k)=\begin{cases}  1\mbox{ se }k=0\\ 0\mbox{ altrimenti}   \end{cases}$$

>[!prp] Trasformata Zeta dell’impulso
>$$\mathcal{Z}[\delta(z)]=1\qquad z\in \mathbb{C}$$
>[[Trasformata Zeta]]