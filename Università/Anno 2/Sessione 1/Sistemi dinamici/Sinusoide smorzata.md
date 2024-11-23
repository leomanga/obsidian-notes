$$f(t)= e^{-2 t}\cos(2\pi t)\cdot \mathbb{1}(t)$$

```functionplot
---
title: Sinusoide smorzata
xLabel: 
yLabel: 
bounds: [-0.5,2.5,-1.1,1.1]
disableZoom: true
grid: true
---
y = x<0 ? 0 :2.718^(-2*x)*cos(2*3.14*x)
```
>[!prp] Trasformata di Laplace della sinusoide smorzata
>$$\mathcal{L}[f(t)]=\frac{s+2}{(s+2)^{2}+(2\pi)^{2}}\qquad s\in \mathbb{C}$$

