---
capitolo: 17
collegamenti:
---
# Definizione
Siano $f,g:(x_0,x_0+\delta)\to(0,+\infty)$ due funzioni tali che 
$$\lim_{x\to x_0}f(x)=\lim_{x\to x_{0}}g(x)= 0\qquad \mbox{su } (x_0,x_0+\delta)$$
Si dice che $f$ è un o piccolo di $g$ per $x\to x_0^+$, o che $f$ è un infinitesimo di ordine maggiore di $g$ per $x\to x_0$ e si scrive $f=o(g)$ per $x\to x_0$ se
$$\lim_{x\to x_0}\frac{f(x)}{g(x)} = 0\qquad \mbox{su } (x_0,x_0+\delta)$$
- Per le proprietà dei limiti si ha
	- se $f = o(g)$ per $x\to x_0^+$ e $h = o(g)$ per $x\to x_0^+$ allora $f+h = o(g)$ per $x\to x_0^+$;
	- se $f = o(g)$ per $x\to x_0^+$ e $\lambda > 0$  allora $\lambda f = o(g)$ per $x\to x_0^+$;
	- se $f = o(g)$ per $x\to x_0^+$ e $h = o(g)$ per $x\to x_0^+$ allora $fh = o(g^2)$ per $x\to x_0^+$;
- Si scrive $f = o(1)$ per dire che $f$ è infinitesima.