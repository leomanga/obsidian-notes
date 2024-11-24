---
capitolo: 14
---
# Funzione continua in un punto
Una funzione reale $f$ definita su un insieme $E\subseteq \mathbb{R}$ si dice continua in un punto $x_{0}\in E$ se vale
$$\lim_{x\to x_{0}}f(x)= f(x_{0})\qquad \mbox{ su E}$$
# Osservazione | Continuità in un punto isolato
Se $x_0$ è un punto isolato di $E$, cioè esiste $t>0$ tale che $\{x\in E:|x-x_{0}|<t\}= \{x_0\}$, allora l'uguaglianza dell'equazione sopra si ridiuce, grazie al [[Limiti finiti di una funzione in un punto#Lemma 2 Localizzazione| lemma di localizzazione]], all'identità
$$\lim_{x\to x_{0}}f(x)= f(x_{0})\qquad \mbox{ su }\{x_0\}$$
# Osservazione | Continuità in un punto non isolato
Se $x_0$ non è un punto isolato di $E$, allora l'equazione sopra è equivalente alla relazione$$\lim_{x\to x_{0}}= f(x_{0})\qquad \mbox{ su }E\setminus\{x_0\}$$
# Osservazione 14.0.5
Dalla [[Limiti finiti di una funzione in un punto#Proprietà|proprietà]]. La continuità di $f$ in $x_0$ è equivalente ad una delle due condizioni:
1) $\forall \epsilon > 0\ \exists\delta = \delta_{0},\epsilon > 0\mbox{ tale che }\forall x \in E, |x-x_0| < \delta\ : |f(x)-f(x_0)| <\epsilon$ 
2) Per ogni successione $x_{n}\subseteq E$ tale che $\lim_{n\to+\infty}x_{n}= x_0$ si ha
$$\lim_{n\to+\infty}f(x_{n})= f(x_0)$$
# Funzione continua in un insieme
Una funzione reale $f$ definita su un insieme $E\subseteq\mathbb{R}$ si dice continua su $E$ se è continua in ogni punto di $E$

# Lemma 1 | Continuità e operazioni algebriche
Se $f$ e $q$ sono funzioni reali definite e continue su $E\subseteq\mathbb{R}$, allora le funzioni $f+g,f-g,fg$ sono definite e continue su $E$. 
Se in più $g(x)\not = 0\quad \forall x\in E$, allora è definita e continua la funzione $f/g$.

# Funzione di Dirichlet discontinua in ogni punto
$f:\mathbb{R}\to\mathbb{R}$
$$f(x):= \begin{cases} 1\ \ \ \mbox{ se } x\in\mathbb{Q}\\
0\ \ \ \mbox{ se } x\in\mathbb{R}\setminus\mathbb{Q}\end{cases}$$

# Funzioni continue su intervalli chiusi e limitati

## Limite destro e sinistro
Se $f:[a,b]\to\mathbb{R}$ e $t\in[a,b)$, scriveremo
$$\lim_{x\to t^+}f(x)$$
per indicare il
$$\lim_{x\to t}f(x)\mbox{ su }\{x\in[a,b]:x>t\}$$
Limite destro.
Per indicare il limite sinistro sarà sufficiente prendere la parte a sinistra dell'insieme $(a,b]$ in modo molto simile.

# Criterio di continuità per le funzioni monotone
Sia $f$ una funzione reale definita su un intervallo $[a,b]$, e sia [[Funzioni monotone|crescente]]. Se $f$ assume tutti i valori compresi fra $f(a)$ e $f(b)$, allora $f$ è continua in $[a,b]$.
#dimostrazione-da-fare 

# Teorema 14.1.6 | Weierstrass
Sia $f$ una funzione reale definita e continua su un intervallo $[a,b]$. Allora l'insieme $f([a,b])$ è limitato ed è dotato di elemento massimo e di elemento minimo.
#dimostrazione-da-fare 

### Ipotesi ottimali
Se eliminiamo l'ipotesi che il dominio di $f$ sia un intervallo chiuso e limitato, il teorema può diventare falso.

### Valori intermedi
Sia $f$ una funzione reale definita e continua sull'intervallo chiuso e limitato $[a,b]$. Allora $f$ assume tutti i valori compresi tra il suo valore minimo e il suo valore massimo.
#dimostrazione-da-fare 

# Esistenza degli zeri
Sia $f:[a,b]\to\mathbb{R}$ una [[Funzioni continue|funzione continua]] tale che 
$$f(a)f(b)<0$$
Esiste $x\in[a,b]$ tale che $f(x) = 0$.
#dimostrazione-da-fare 

# Punto fisso
Sia $f:[0,1]\to[0,1]$ una [[Funzioni continue|funzione continua]]. 
Esiste $x\in[0,1]$ tale che $f(x) = x$.
#dimostrazione-da-fare 