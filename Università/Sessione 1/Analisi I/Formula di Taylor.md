---
capitolo: 17
collegamenti:
  - "[[Derivate]]"
---
# Formula
Sia $n\in\mathbb{N}$, e sia $f:[a,b]\to\mathbb{R}$ una funzione derivabile $n$ volte in $[a,b]$. Allora esiste un $c\in(a,b)$ tale che
$$f(b)-\left[f(a)+f^{'}(a)(b-a)+\ldots+\frac{f^{(n-1)}(a)}{(n+1)!}(b-a)^{n-1}\right] = \frac{f^{(n)}(c)}{n!}(b-a)^{n}       $$
### Polinomio di Taylor di $f$ di ordine $n-1$
Il polinomio, che prende il nome di "polinomio di Taylor di $f$ di ordine $n-1$", ovvero quello fra le quadre, può essere riscritto come 
$$\sum_{k=0}^{n-1}\frac{f^{(k)}(a)}{k!}(b-a)^k$$
- È la generalizzazione del [[Teorema di Lagrange]] con $n$ = 1.
### Resto di Lagrange di ordine $n$
La funzione $\frac{f^{(n)}(c)}{n!}(b-a)^n$ si chiama "resto di [[Teorema di Lagrange|Lagrange]]" di ordine $n$.
### Variabili e punti fissati
In questa formula devo pensare a:
- $a$ come punto fissato.
- $b$ come incognita, che può stare anche a "sinistra" di $a$.
Inoltre è importante sapere che $c$ dipende sia da $a$, $b$ e "n".

#dimostrazione-da-fare 