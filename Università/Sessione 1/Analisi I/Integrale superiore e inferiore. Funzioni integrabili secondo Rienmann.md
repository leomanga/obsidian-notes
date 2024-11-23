---
capitolo: 19
collegamenti:
  - "[[Estremo superiore e inferiore]]"
  - "[[Funzioni costanti a tratti]]"
aliases:
  - integrabile secondo Rienmann
---
Sia $f:[a,b]\to\mathbb{R}$ una funzione limitata.
# Definizione | Integrale superiore
Si dice integrale superiore di $f$ esteso all'intervallo $[a,b]$, e si indica con
$$\int_{[a,b]}^{*} f(x) dx,$$
il numero reale 
$$\inf\{\int_{[a,b]}k(x) dx: k \mbox{ costante a tratti}, k(x)\ge f(x)\ \forall x \in [a,b]\}$$
# Definizione | Integrale inferiore 
Si dice integrale superiore di $f$ esteso all'intervallo $[a,b]$, e si indica con
$$\int_{{*}[a,b]} f(x) dx,$$
il numero reale 
$$\sup\{\int_{[a,b]}h(x) dx: h \mbox{ costante a tratti}, h(x)\le f(x)\ \forall x \in [a,b]\}$$
# Rapporto fra i due integrali
Si vede immediatamente che 
$$\int_{*[a,b]} f(x)dx \le \int_{[a,b]}^{*}f(x)dx$$

### Osservazione 
Può valere la disuguaglianza stretta, ad esempio con [[Problema dei riordinamenti#Teorema Dirichlet]] ( Guarda appunti per capire meglio)

# Definizione 19.1.3 | Funzione integrabile secondo Riemann
Una funzione $f:[a,b]\to\mathbb{R}$ limitata si dice integrabile secondo Riemann in $[a,b]$ se
$$\int_{*[a,b]} f(x)dx = \int_{[a,b]}^{*}f(x)dx$$
In questo caso il valore comune dell'integrale superiore e dell'integrale inferiore di $f$ verrà indicato con il simbolo
$$\int_{[a,b]}f(x) dx$$
# Teorema 19.1.4 | Integrabilità delle funzioni continue 
Se $f:[a,b]\to\mathbb{R}$ è [[Funzioni continue|funzione continua]] in $[a,b]$, allora è integrabile in $[a,b]$.
- Da [[Funzioni continue#Teorema 14.1.6 Weierstrass]], $f$ è anche limitata.
#dimostrazione-da-fare 

# Teorema 19.1.7 | Integrabilità delle funzioni monotone
Sia $f:[a,b]\to\mathbb{R}$ una funzione monotona. Allora $f$ è integrabile secondo Rienmann.
#dimostrazione-da-fare 

# Teorema 19.1.10 | Integrale come limite
[[Integrale di una funzione costante a tratti#Proposizione 19.0.7 Integrale come limite]]
Sia $f:[a,b]\to\mathbb{R}$ limitata.
Supponiamo che $f$ sia integrabile in $[a,b]$. Allora
$$\int_{[a,b]}f(x)dx=\lim_{s\to 0^+}s\sum_{i\in\mathbb{N}:a\le is < b}f(is)$$
#dimostrazione-da-fare 
Oppure
$$\int_{[a,b]}f(x)dx=\lim_{s\to +\infty}2^{-n}\sum_{i\in\mathbb{N}:a\le i2^{-n} < b}f(i2^{-n})$$
- In questo modo possiamo ricavare le proprietà valide per le funzioni costanti a tratti([[Integrale di una funzione costante a tratti]])