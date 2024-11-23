---
capitolo: 19
collegamenti:
  - "[[Funzioni costanti a tratti]]"
  - "[[Misura di un intervallo]]"
---
# Definizione
Sia $f:[a,b]\to\mathbb{R}$ una funzione [[Funzioni costanti a tratti|costante a tratti]]. 
Se $a_1,a_2,\ldots,a_{n-1}$ sono i punti di discontinuità di $f$ interni ad $[a,b]$, e se indichiamo con $T_1,T_2,\ldots,T_n$ gli intervalli $[a,a_1],[a_1,a_2],\ldots,[a_{n-1},b]$, e con $c_i$ l'unico valore che $f$ assume in $T_i$ per ogni $i = 1,\ldots,n$, allora diremo integrale di $f$ esteso a $[a,b]$ il numero reale 
$$\sum_{i=1}^{n}c_{i}mis(T_i)$$
e lo indicheremo con il simbolo
$$\int_{[a,b]}f(x)dx$$
### Interpretazione geometrica
Se $c_i>0$ allora $c_imis(T_i)$ è l'area del rettangolo
$$\{(x,y)\in\mathbb{R}^{2}:x\in T_{i}, y\in[0,c_i]\}$$
e quindi la funzione $f$ assume solo valori positivi, l'integrale è la regione del piano che si ottiene facendo l'unione dei rettangoli per $i=1,\ldots,n$.
Rappresenta la differenza dei rettangoli per $c_i>0$ e $c_i<0$.

# Osservazione 19.0.6
Nel caso particolare in cui $f$ è costante, $f(x)=c$ per ogni $x\in[a,b]$, si ha
$$\int_{[a,b]}f(x)dx=c(b-a)$$
# Proposizione 19.0.7 | Integrale come limite
Sia $f:[a,b]\to\mathbb{R}$ una [[Funzioni costanti a tratti|funzione costante a tratti]]. Allora
$$\int_{[a,b]}f(x)dx=\lim_{s\to 0^+}s\sum_{i\in\mathbb{N}:a\le is < b}f(is)$$
#dimostrazione-da-fare 
Oppure
$$\int_{[a,b]}f(x)dx=\lim_{s\to +\infty}2^{-n}\sum_{i\in\mathbb{N}:a\le i2^{-n} < b}f(i2^{-n})$$
# Corollario 19.0.8 | Monotonia dell'integrale
Siano $f,g:[a,b]\to\mathbb{R}$ due [[Funzioni costanti a tratti]]. Se
$$f(x)\le g(x)\qquad \forall x \in[a,b]$$
allora
$$\int_{[a,b]}f(x)dx\le\int_{[a,b]}g(x)dx$$
#dimostrazione-da-fare 

# Corollario 19.0.9 | Teorema della media
Se $f:[a,b]\to\mathbb{R}$ è una [[Funzioni costanti a tratti|funzione costante a tratti]], e se si ha, per $c_1,c_2\in\mathbb{R}$,
$$c_1\le f(x)\le c_2\qquad \forall x\in[a,b]$$
allora
$$c_1mis([a,b])\le\int_{[a,b]}f(x)dx\le c_2 mis([a,b])$$
- In poche parole l'integrale della funzione è maggiore di tutta l'area del rettangolo con altezza $c_1$ e base $mis([a,b])$, e maggiore dell'altezza $c_2$ e base $mis([a,b])$.
#dimostrazione-da-fare 
# Corollario 19.0.10 | Proprietà distributiva
Se $f,g:[a,b]\to\mathbb{R}$ sono due [[Funzioni costanti a tratti]], e se $\lambda,\mu\in\mathbb{R}$, allora
$$\int_{[a,b]}(\lambda f(x) + \mu g(x))dx = \lambda \int_{[a,b]}f(x) dx + \mu \int_{[a,b]}g(x)dx$$
#dimostrazione-da-fare 

# Corollario 19.0.11 | Proprietà additiva
Se $f,g:[a,b]\to\mathbb{R}$ sono due [[Funzioni costanti a tratti]], e se $c\in(a,b)$, allora
$$\int_{[a,b]}f(x)dx = \int_{[a,c]}f(x) dx + \int_{[c,b]}f(x) dx$$
#dimostrazione-da-fare 

