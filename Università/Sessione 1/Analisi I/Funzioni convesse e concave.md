---
capitolo: 18
---
# Definizione | funzione convessa
Una funzione $f:I\to\mathbb{R}$ si dice convessa in $I$ se per ogni $x_0,x_{1}\in I$ e per ogni $t\in(0,1)$ vale
$$f(tx_0+(1-t)x_{1})\le tf(x_0)+(1-t)f(x_1)$$
- Si parla di "strettamente convessa" se ci fosse il "$<$".
- In poche parole tutto il segmento che congiunge due punti appartenenti al grafico di $f$ è tutto contenuto nel sopragrafico di $f$:
$$sopragraf(f):= \{(x,y)\in I \times \mathbb{R}:y\ge f(x)\}$$
### Esempi
$f:\mathbb{R}\to\mathbb{r}, f(x)=|x|$ è convessa in $\mathbb{R}$.
N.B. Non necessariamente una funzione convessa è derivabile in ogni punto del suo dominio. Deve però essere continua(anche se non specificato dalla definizione, perchè immediato).

# Definizione | funzione concava
Una funzione $f:I\to\mathbb{R}$ si dice concava in $I$ se $-f$ è convessa in $I$.
- Si dice strettamente concava se $-f$ è strettamente convessa.

# Teorema 1
Sia $f:I\to\mathbb{R}$ convessa e supponiamo che sia derivabile in $I$ con derivata continua. 
Allora $$f \mbox{ strettamente convessa}\Rightarrow f^{'}\mbox{ è non decrescente in }I$$
# Teorema 2
Sia $f:I\to\mathbb{R}$ convessa in $I$ e supponiamo che $f$ sia derivabile 2 volte in $I$, con derivata seconda continua in $I$.
Allora 
$$f \mbox{ è convessa}\iff f^{''}\ge0\mbox{ in } I$$
- Sarà strettamente convessa con "$>$"