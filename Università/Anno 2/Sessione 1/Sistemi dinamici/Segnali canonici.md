In generale $$r_{k}(t)=\frac{t^{k}}{k!}\cdot \mathbb{1}(t)\quad k=0,1,\ldots$$
Dove $\mathbb{1}(t)$ è il [[Gradino unitario]].
# Rampa lineare
$$r_{1}(t)=t\cdot \mathbb{1}(t)$$

```functionplot
---
title: Rampa lineare
xLabel: 
yLabel: 
bounds: [-2,5,-0.5,5]
disableZoom: true
grid: true
---
f(x)=x<0? 0: x
```
# Rampa parabolica
$$r_{2}(t)=\frac{t^{2}}{2}\cdot \mathbb{1}(t)$$

```functionplot
---
title: Rampa parabolica
xLabel: 
yLabel: 
bounds: [-2,5,-0.5,5]
disableZoom: true
grid: true
---
f(x)=x<0? 0: x^2 
```

>[!prp] Trasformata di Laplace dei segnali canonici
>$$\mathcal{L}[r_{k}(t)]=\frac{1}{s^{k+1}}\qquad s\in \mathbb{C}$$
>[[Trasformata di Laplace]]

