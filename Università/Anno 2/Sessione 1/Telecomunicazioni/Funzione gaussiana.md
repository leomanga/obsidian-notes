La funzione gaussiana viene usata come [[Densità di probabilità]].
$$f_{x}(\mathbb{x})=\frac{1}{\sqrt{2\pi\sigma^{2}}}e^{-\frac{(x-m)^2}{2\sigma^2}}$$
$m$ rappresenta la media, ovvero il punto in cui ha il picco.
$\sigma^{2}$ rappresenta la varianza
$\sigma$ rappresenta la deviazione standard, ovvero quanto la curva della gaussiana sia schiacciata. (Maggiore è $\sigma$, più si schiaccia la curva)
$\frac{1}{\sqrt{2\pi\sigma^{2}}}$ rappresenta il punto di massimo.

```functionplot
---
title: Grafico funzione gaussiana
xLabel: Sigma = 1/radq(2*pi). m = 0
yLabel: 
bounds: [-2,2,0,1.5]
disableZoom: false
grid: true
---
f(x) = (1/sqrt(2*3.14*(1/sqrt(2*3.14))^2))*2.718^(-x^2/(2*(1/sqrt(2*3.14))^2))
```
