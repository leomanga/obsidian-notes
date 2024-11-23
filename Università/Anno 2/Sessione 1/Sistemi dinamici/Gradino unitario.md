$$
\mathbb{1}(t)=
\begin{cases}
1\mbox{ se } t\ge 0\\
0\mbox{ se } t<0
\end{cases}
$$

```functionplot
---
title: Gradino unitario
xLabel: t
yLabel: 
bounds: [-2,5,-0.5,1.5]
disableZoom: true
grid: true
---
f(x) = x < 0 ? 0 : 1
```

>[!prp] Trasformata di Laplace del gradino unitario
>$$\mathcal{L}[\mathbb{1}(t)]=\frac{1}{s}\qquad s\in \mathbb{C}$$
>[[Trasformata di Laplace]]

^0f456d



