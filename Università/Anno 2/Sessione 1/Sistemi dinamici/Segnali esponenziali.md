# Tempo continuo
In generale 
$$
f(t)=e^{\alpha t}\cdot \mathbb{1}(t),\quad \alpha\in \mathbb{R}
$$

^4cdd45

## Caso $\alpha>0$

```functionplot
---
title: Segnale esponenziale, caso alpha>0
xLabel: alpha = 2
yLabel: 
bounds: [-1,2,-0.5,5]
disableZoom: true
grid: true
---
f(x) = x<0?0:2.71828^(2*x)
```
## Caso $\alpha<0$

```functionplot
---
title: Segnale esponenziale, caso alpha<0
xLabel: alpha = -2
yLabel: 
bounds: [-1,2,-0.5,5]
disableZoom: true
grid: true
---
f(x) = x<0?0:2.71828^(-2*x)
```

>[!prp] Trasformata di Laplace dei segnali esponenziali
>$$\mathcal{L}[e^{\alpha t}(t)\cdot \mathbb{1}(t)]=\frac{1}{s-\alpha}\qquad s\in \mathbb{C}$$
>[[Trasformata di Laplace]]

# Tempo discreto
$$f(k)=\rho^{k}\cdot \mathbb{1}(k)$$
