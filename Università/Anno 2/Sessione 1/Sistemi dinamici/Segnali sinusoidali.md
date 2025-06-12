---
collegamenti:
  - "[[Funzioni complesse#Formule di Eulero]]"
---
# Tempo continuo
In generale
$$
f(t)=\cos(\omega t)=\frac{e^{j\omega t}+e^{-j\omega t}}{2}
$$

^d3c773

$$
f(t)=\sin(\omega t)=\frac{e^{j\omega t}-e^{-j\omega t}}{2j}
$$

^c31b97

Dove $\omega$ è la pulsazione.

>[!prp] Trasformata di Laplace del coseno
>$$\mathcal{L}[\cos(\omega t)\cdot\mathbb{1}(t)]=\frac{s}{s^{2}+\omega^{2}}\qquad s\in \mathbb{C}$$
>[[Trasformata di Laplace]]

>[!prp] Trasformata di Laplace del seno
>$$\mathcal{L}[\sin(\omega t)\cdot\mathbb{1}(t)]=\frac{\omega}{s^{2}+\omega^{2}}\qquad s\in \mathbb{C}$$
>[[Trasformata di Laplace]]

# Tempo discreto
$$f(k)=\cos(\omega k)\mathbb{1}(k)=\frac{1}{2}(e^{j\omega})^{k}+\frac{1}{2}(e^{-j\omega})^{k}$$
$$f(k)=\sin(\omega k)\mathbb{1}(k)=\frac{1}{2j}(e^{j\omega})^k-\frac{1}{2j}(e^{-j\omega})^k$$
>[!prp] Trasformata Zeta del coseno
>$$\mathcal{Z}[\cos(\omega z)]=\frac{z(z-\cos(\omega))}{z^{2}+2\cos(\omega)z+1}\qquad z\in \mathbb{C}$$
>[[Trasformata Zeta]]

>[!prp] Trasformata Zeta del seno
>$$\mathcal{Z}[\sin(\omega z)]=\frac{z\sin(\omega)}{z^{2}+2\cos(\omega)z+1}\qquad z\in \mathbb{C}$$
>[[Trasformata Zeta]]