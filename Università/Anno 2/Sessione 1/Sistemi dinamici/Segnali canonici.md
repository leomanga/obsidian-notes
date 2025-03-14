# Tempo continuo
In generale $$r_{k}(t)=\frac{t^{k}}{k!}\cdot \mathbb{1}(t)\quad k=0,1,\ldots$$
Dove $\mathbb{1}(t)$ è il [[Gradino unitario]].
## Rampa lineare
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
## Rampa parabolica
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

## Segnali utili per telecomunicazioni

### Rettangolo
$$rect(t)=\Pi(t)=\begin{cases}1 \quad -\frac{1}{2}\le t\le \frac{1}{2}\\0 \quad \mbox{altrimenti} \end{cases}$$
### Triangolo
$$tr(t)=\Lambda(t)=\begin{cases}t+1 \quad -1\le t\le 0\\-t+1\quad 0\le t\le 1  \\0\quad |t|>1\end{cases}$$
$$\Lambda(t)=\Pi(t)*\Pi(t)$$ * [[Prodotto di convoluzione]]
### Segno
$$sgn(t)=\begin{cases}1\quad t>0\\ 0\quad t=0 \\ -1\quad t<0\end{cases}=u(t)-u(-t)$$
Definendo $x_{n} = \begin{cases}e^{\frac{-t}{n}} \quad t> 0 \\ 0 \quad t=0\\ -e^{\frac{t}{n}}\quad t<0\end{cases}$
$$sgn(t)=\lim_{n\to \infty} x_{n}(t)$$

### Sinc
$$sinc(t)=\begin{cases}\frac{\sin(\pi t)}{}\end{cases}$$
# Tempo discreto
$$r_{n}(k)=\binom{k}{n}\mathbb{1}(k)$$