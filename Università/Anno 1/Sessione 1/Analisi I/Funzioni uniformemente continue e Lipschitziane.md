# Definizione 15.0.1 | Funzione uniformemente continua
Una funzione $f:E\subseteq\mathbb{R}\to\mathbb{R}$ si dice uniformemente continua in $E$ se 
$$\forall \epsilon > 0\ \exists \delta_\epsilon > 0:\ \forall x^{'}\in E\ \ \forall x^{''} \in E\ \ |x^{'}-x^{''}| <\delta_\epsilon \Rightarrow |f(x^{'})-f(x^{''})|<\epsilon$$
- Da notare che $\delta$ non dipende dalle $x$, cosa non vera con le [[Funzioni continue]].
- Il concetto di uniforme continuità non viene dato in un punto ma in tutto un insieme.

Esercizi 15.0.2,0.3

# Teorema 15.0.4 | Continua su un compatto è uniformemente continua
[[Chiusura di un insieme#Definizione 11.1.4 Insieme compatto]]
Sia $f:[a,b]\to\mathbb{R}$ una [[Funzioni continue|funzione continua]]. Allora $f$ è uniformemente continua in $[a,b]$.

#dimostrazione-da-fare [[Dimostrazione per assurdo]]

# Definizione 15.0.6 | Funzione Lipschitziana
Una funzione $f:E\subseteq \mathbb{R}\to\mathbb{R}$ si dice Lipshitziana in $E$ se esiste una costante $c\ge 0$ tale che 
$$\forall x^{'}\in E\ \ \ \forall x^{''}\in E\quad |f(x^{'})-f(x^{''})| \le c|x^{'}-x^{''}|$$

Esercizio 15.0.7-8