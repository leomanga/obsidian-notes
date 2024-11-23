---
collegamenti:
  - "[[Derivate]]"
capitolo: 17
---
# Definizione 
Sia $I \subseteq \mathbb{R}$ un intervallo
Sia $f:I \to \mathbb{R}$ una funzione, e sia $x_0$ un punto <mark style="background: #FFB86CA6;">interno</mark> ad $I$.
Supponiamo che $f$ sia derivabile in $x_0$.
Allora $x_0$ è un punto critico di $f$ se
$$f^{'}(x_{0)} = 0$$
- Dal [[Derivate#Corollario 17.2.4 Punti di minimo e massimo interni|Corollario 17.2.4]], possiamo dire che se $x_0$ è un punto di massimo o minimo, allora è anche un punto critico.
- Esistono anche punti critici che non sono né massimi né minimi, ad esempio $x=0$ è critico per $f(x)=x^3$, ma non è né di massimo né di minimo.
```functionplot
---
title: f(x) = x^3
xLabel: 
yLabel: 
bounds: [-10,10,-10,10]
disableZoom: false
grid: true
---
f(x) = x^3

```
# Definizione 17.4.2 | Minimi e massimi locali
Sia $f:I\subseteq\mathbb{R} \to \mathbb{R}$ una funzione e $x_{0} \in I$.
- $x_0$ si dice <mark style="background: #FFB86CA6;">minimo locale</mark> per $f$ se esiste $\rho>0$ tale che
$$f(x_{0}) \le f(x)\qquad\forall x\in I \cap(x_0-\rho,x_0+\rho)$$
- $x_0$ si dice <mark style="background: #FFB86CA6;">minimo locale stretto</mark> per $f$ se esiste $\rho>0$ tale che
$$f(x_0)<f(x)\qquad \forall x \in I\cap(x_0-\rho,x_0+\rho)\setminus\{x_0\}$$
- Stessa cosa per il <mark style="background: #FFB86CA6;">massimo e massimo locale stretto</mark> ma con segno opposto.
#chiedere_a_prof il meno $x_0$ non dovrebbe essere sopra?

# Teorema 17.4.3
Sia $f:I\subseteq\mathbb{R}\to\mathbb{R}$ una funzione derivabile due volte in $I$, con derivata seconda continua in $I$. 
Sia $x_0$ un punto interno ad $I$ che sia critico per $f$. Se
$$f^{''}(x_0)>0$$
allora $x_0$ è un punto di minimo locale stretto per $f$.
- Stessa cosa con verso opposto per il massimo locale stretto.
#dimostrazione-da-fare  Si usa la [[Formula di Taylor]]
# Teorema 17.4.5
Sia $f:I\subseteq \mathbb{R}\to\mathbb{R}$ una funzione derivabile $n>2$ volte, con $f^{(n)}$ continua in $I$, e sia $x_0$ un punto interno ad $I$. Supponiamo
$$f^{'}(x_{0})= f^{''}(x_{0)}= \ldots = f^{(n-1)}(x_{0})= 0$$
e 
$$f^{(n)}(x_0)\not=0$$
- Se $n$ è pari
	- Se $f^{(n)} > 0$ il punto $x_0$ è un minimo locale stretto di $f$;
	- Se $f^{(n)} < 0$ il punto $x_0$ è un massimo locale stretto di $f$;
- Se $n$ è dispari, il punto $x_0$ non è né un minimo locale né un massimo locale di $f$.
#dimostrazione-da-fare [[Formula di Taylor]]