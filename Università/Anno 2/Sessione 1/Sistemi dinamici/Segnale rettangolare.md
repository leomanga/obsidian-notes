$$f(t)=\begin{cases}1 \mbox{ se }0\le t\le \Delta\\ 0\mbox{ altrimenti} \end{cases}$$
Con $\Delta > 0$
```functionplot
---
title: 
xLabel: delta = 3
yLabel: 
bounds: [-0.5,3.5,-0.5,1.5]
disableZoom: false
grid: true
---
f(x) = x<0? 0 : ( x>3 ? 0 : 1)
```
Questo segnale può essere riscritto come differenza di [[Gradino unitario|gradini unitari]].
$$f(t)=\mathbb{1}(t)- \mathbb{1}(t-\Delta)$$

>[!prp] Trasformata del segnale rettangolare
>Da [[Trasformata di Laplace#^a6ef22|(1)]] e [[Gradino unitario#^0f456d|(2)]]
>$$\mathcal{L}[f(t)]=\frac{1}{s}-\frac{1}{s}e^{-s\Delta}\qquad s\in \mathbb{C}$$
>