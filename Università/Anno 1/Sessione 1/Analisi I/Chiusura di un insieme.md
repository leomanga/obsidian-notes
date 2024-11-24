---
capitolo: 11
---
Utile per lo studio dei limiti, derivate ecc...
Studiamo
$$f:E\subseteq\mathbb{R} \to \mathbb{R}$$
# Chiusura di E
Sia $E\subseteq\mathbb{R}$. Chiamiamo chiusura di $E\ (in\ \mathbb{R})$  l'insieme che indicheremo con $\bar E$, definito da
$$\bar E := \{x\in\mathbb{R}: \forall \epsilon \in \mathbb{R},\epsilon > 0\ \exists y\in E:|y-x|<\epsilon\}$$
### Osservazioni
In generale $E \subseteq \bar E$, ma può verificarsi che $E = \bar E$.
Se
$$E \subseteq F \Rightarrow \bar E \subseteq \bar F$$
$$\bar {\bar E} = \bar E $$
# Insieme chiuso
Un insieme $E$ si dice chiuso(in $\mathbb{R}$) quando $E = \bar E$.

# Esempi
$E = \mathbb{R} \Rightarrow \bar E = E = \mathbb{R}$
$E = [0,1] \Rightarrow \bar E = E = [0,1]$
$E = \mathbb{Q} \cap [0,1] \Rightarrow \bar E = [0,1]$ (Dimostrazioni appunti 2 pg 7)

# Teorema 11.0.6
Sia $E$ un insieme di numeri reali. Perché $x \in \bar E$ occorre e basta che esista una successione $e_n$ di elementi di $E$ tale che
$$\lim_{n\to+\infty}e_{n}= x$$
#dimostrazione-da-fare 

# Insieme limitato
Un sottoinsieme $E$ dei numeri reali si dice limitato (in $\mathbb{R}$) se esistono due numeri reali $\alpha,\beta$ con $\alpha \le \beta$ tali che 
$$E \subseteq [\alpha,\beta].$$
$$\exists \alpha,\beta \in \mathbb{R}\qquad\alpha\le e\le\beta\qquad \forall e \in E$$
# Definizione 11.1.3 | Insieme relativamente compatto
Un sottoinsieme $E$ dei numero reali si dice relativamente compatto(in $\mathbb{R}$) se, data una successione di punti di $E$, essa ammette una [[Successioni e limiti infiniti#Teorema 7.0.12 - 7.0.13 Sottosuccessioni estratte|sottosuccessione]] convergente ad un numero reale.
### Esempi
$(0,1)$ è relativamente compatto, $(-\infty,0)$ non è relativamente compatto.
# Definizione 11.1.4 | Insieme compatto
Un sottoinsieme $E$ dei numeri reali si dice compatto se, data una successione di punti di $E$, essa ammette una [[Successioni e limiti infiniti#Teorema 7.0.12 - 7.0.13 Sottosuccessioni estratte|sottosuccessione]] convergente a un punto di $E$.
### Esempi
L'intervallo $(0,1)$ non è compatto.

### Osservazione 1
E' immediato osservare che 
$$E\ compatto\Rightarrow E\ chiuso$$
$$E\ compatto\Rightarrow E\ limitato$$
# Riformulazione Bolzano-Weierstrass
[[Teorema di Bolzano-Weierstrass]]
Il teorema di Bolzano-Weierstrass si può riscrivere:
- Un sottoinsieme limitato dei numeri reali è relativamente [[Chiusura di un insieme#Definizione 11.1.3 Insieme relativamente compatto|compatto]]
- Siano $\alpha,\beta$ due numeri reali, con $\alpha \le \beta$. Allora l'intervallo $[\alpha,\beta]$ è compatto.
- E\ chiuso\ e\ limitato\iff E\ compatto$

# Punto di accumulazione per un insieme
Siano
$$E\subseteq \mathbb{R},\qquad x\in \mathbb{R}$$
Il punto $x$ si dice di accumulazione per $E$ se
$$
x \in  \overline{E\setminus \{x\}}
$$
Si può anche scrivere:
$$\forall \epsilon > 0:(x-\epsilon,x+\epsilon) \cap E \not = \{x\}$$
In poche parole, $x$ è di accumulazione per $E$ se e solo se esiste una successione di punti di $E$ diversi da $x$ convergente a $x$.
### Esempi
$\mathbb{N}$ non ha punti di accumulazione.
L'insieme dei punti di accumulazione di $E = (0,1)$ è $[0,1]$.

# Punto isolato di un insieme
Siano
$$E\subseteq \mathbb{R},\qquad x\in \mathbb{E}$$
$x$ è un punto isolato di $E$ se
$$\exists \epsilon > 0:(x-\epsilon,x+\epsilon) \cap E = \{x\}$$
### Esempi
Tutti i punti di $\mathbb{N}$ sono isolati di $\mathbb{N}$.
L'intervallo $E = (0,1)$ non ha punti isolati.

# Insieme aperto
Un sottoinsieme $E$ dei numeri reali si dice aperto(in $\mathbb{R}$) se $\mathbb{R}\setminus E$ è chiuso.
### Esempi
L'intervallo $(0,1)$ è aperto.
L'intervallo $(0,1]$ non è né aperto né chiuso.
Anche l'insieme vuoto e quello dei reali sono aperti.

# Punto interno ad un insieme
Siano $E\subseteq \mathbb{R}\qquad x\in E$
Il punto $x$ si dice interno ad $E$ se 
$$\exists \epsilon >0:(x-\epsilon,x+\epsilon) \subseteq E$$
Si indica con 
$$int(E)$$
In generale$$int(E) \subseteq E$$
Può anche verificarsi che $int(E) = E$
###Esempi
Un insieme è [[Chiusura di un insieme#Insieme aperto|aperto]] se tutti i suoi punti sono interni.
$int(\mathbb{N} = \emptyset)$  
$int([0,1]) = (0,1)$
