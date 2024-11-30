---
collegamenti:
  - "[[Segnali esponenziali]]"
  - "[[Segnali canonici]]"
---
# Tempo continuo
In generale $$f_{k}(t)=\frac{t^{k}}{k!}\cdot e^{\alpha t}\cdot \mathbb{1}(t)$$

```functionplot
---
title: Segnale a rampa esponenziale
xLabel: k=1, alpha = -1
yLabel: 
bounds: [-0.5,8,-0.5,1]
disableZoom: true
grid: true
---
f(x) = x<0? 0 : x * 2.71828^(-1 * x)
```

>[!prp] Trasformata di Laplace della rampa esponenziale
>$$\mathcal{L}[f_{k}(t)]=\frac{1}{(s-\alpha)^{k+1}}\qquad s\in \mathbb{C}$$
>[[Trasformata di Laplace]]

# Tempo discreto
$$f_{n}(k)=\rho^{k}\binom{k}{n}\mathbb{1}(k)$$
>[!prp] Trasformata Zeta della rampa esponenziale
>$$\mathcal{Z}[f_{n}(k)]=\frac{\rho^{n}\cdot z}{(z-\rho)^{n+1}}\qquad z\in \mathbb{C}$$
>[[Trasformata Zeta]]