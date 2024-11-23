---
capitolo: 19
collegamenti:
  - "[[Integrale su un intervallo orientato]]"
---
# Teorema 19.2.1 | Teorema fondamentale del calcolo integrale I
Sia $f: [a,b]\to\mathbb{R}$ una [[Funzioni continue|funzione continua]], e sia $c\in[a,b]$ un punto fissato. Se si considera la funzione
$$F(x)=\int_c^{x}f(t)dt\qquad\forall x\in[a,b]$$
allora
- $F$ è derivabile in ogni punto di $[a,b]$
- per ogni $x\in[a,b]$ si ha$$F^{'}(x)=f(x)$$
#dimostrazione-da-fare 

# Definizione 19.2.3 | Primitiva
Sia $I\subseteq \mathbb{R}$ un intervallo. Sia $f:I\to\mathbb{R}$ una funzione.
Diremo primitiva di $f$ ogni funzione $g:I\to\mathbb{R}$ [[Derivate#Definizione Derivata di una funzione in un punto|derivabile]] in ogni punto di $I$ e tale che $g^{'}(x)=f(x)$ per ogni $x\in I$.

# Teorema 19.2.4 | Teorema fondamentale del calcolo integrale II
Sia $I\subseteq \mathbb{R}$ un intervallo. Sia $f:I\to\mathbb{R}$ una [[Funzioni continue|funzione continua]]. Allora esistono infinite primitive di $f$, che possono ottenersi da una di esse aggiungendo una qualunque costante reale. Fra le primitive di $f$ vi sono le funzioni integrali
$$F(x)=\int_c^{x}f(t)dt\qquad\forall x\in I$$
dove $c$ è un punto fissato di $I$.

# Proposizione 19.2.5 | Calcolo di integrali definiti
Se $f:I\to\mathbb{R}$ è una funzione continua e se $a,b\in I$ e $g$ è una qualunque primitiva di $f$ allora si ha
$$$\int_a^bf(x)dx=g(b)-g(a)$$
#dimostrazione-da-fare 
