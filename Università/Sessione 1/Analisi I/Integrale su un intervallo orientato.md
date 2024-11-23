---
capitolo: 19
collegamenti:
  - "[[Integrale superiore e inferiore. Funzioni integrabili secondo Rienmann]]"
---
# Definizione: Integrale definito di $f$ tra $a$ e $b$
Dati due numeri reali $a,b$. Indicheremo con
$$\int_a^bf(x)dx$$
l'integrale seguente, che prenderà nome di integrale definito di $f$ tra $a$ e $b$:
$$\int_a^bf(x)dx:=
\begin{cases} \int_{[a,b]}f(x)dx\qquad &\mbox{se }a<b,\\-\int_{[b,a]}f(x)dx&\mbox{se } a>b,\\
0&\mbox{se }a=b,
\end{cases}$$
- $f$ deve essere [[Integrale superiore e inferiore. Funzioni integrabili secondo Rienmann|integrabile secondo Riemann]] in $[a,b]$ nel primo caso, e in $[b,a]$ nel secondo.

# Teorema 19.1.12 | Proprietà additiva
Se $a,b,c$ sono tre numeri reali qualunque, e $f$ è una funzione [[Integrale superiore e inferiore. Funzioni integrabili secondo Rienmann|integrabile secondo Riemann]]  nell'intervallo che ha come primo estremo il più piccolo dei tre numeri $a,b,c$, e come secondo estremo il più grande dei tre numeri $a,b,c$. Allora vale l'uguaglianza:
$$\int_a^bf(x)dx+\int_b^cf(x)dx=\int_a^cf(x)dx$$
# Teorema 19.1.13 | Teorema della media
Se $a,b$ sono due numeri reali qualunque, e $f$ è una funzione [[Integrale superiore e inferiore. Funzioni integrabili secondo Rienmann|integrabile secondo Rienmann]] nell'intervallo che ha come primo estremo il più piccolo dei due numeri $a,b$ e come secondo estremo il più grande. Se in tale intervallo si ha
$$c_{1}\le f(x)\le c_2$$
allora
$$c_1\le\frac{1}{b-a}\int_{a}^{b}f(x)dx\le c_2$$
- $b \not = a$, non serve che sia maggiore come su [[Integrale di una funzione costante a tratti#Corollario 19.0.9 Teorema della media]]
