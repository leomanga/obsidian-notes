---
capitolo: 17
collegamenti:
  - "[[Limiti finiti di una funzione in un punto]]"
---
Sia $I\subseteq\mathbb{R}$
# Definizione| Derivata di una funzione in un punto
Una funzione reale $f$ definita in $I$ si dice derivabile in un punto $x_{0}\in I$ se esiste il limite del rapporto incrementale:
$$\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_{0}}\ \mbox{ su }I\setminus\{x_0\}$$
$x_{0}\in \overline{I\setminus\{x_0\}}$
Il limite deve essere un numero reale.
#### Un altro modo per scrivere la definizione
$$\lim_{h\to 0}\frac{f(x_0+h)-f(x_0)}{h}\ \mbox{ su }(I-x_0)\setminus\{0\}$$

# Una funzione derivabile è continua
Sia $f$ una funzione reale definita su $I$, e derivabile in un punto $x_{0}\in I$. Allora $f$ è continua in $x_0$.
#dimostrazione-da-fare 

# La derivata della somma è la somma delle derivate
$$D(f+g)(x_0)=D(f)(x_0)+D(g)(x_0)$$
#dimostrazione-da-fare 

# Derivata del prodotto
$$D(fg)(x_{0})=g(x_0)D(f)(x_0)+f(x_0)D(g)(x_0)$$
#dimostrazione-da-fare 

# Derivata di una funzione costante = 0
$$*D*(kf)(x_0)=kD(f)(x_0)$$

# Derivata di $\frac{1}{f}$
$$D(\frac{1}{f})(x_{0})= - \frac{D(f)(x_0)}{(f(x_0))^2}$$
#dimostrazione-da-fare 

# Derivata del quoziente
$$D(\frac{f}{g})(x_{0})= \frac{D(f)(x_0)}{g(x_{0})}-\frac{f(x_0)D(g)(x_0)}{(g(x_0))^2}$$
#dimostrazione-da-fare 

da es 17.0.13

# Derivata funzione inversa
Sia $\phi:[a,b]\to\mathbb{R}$ una funzione reale definita su un intervallo chiuso e limitato $[a,b]$. L'insieme dei valori $\phi$ sia un intervallo chiuso e limitato $[c,d]$, e la funzione $\phi$ sia invertibile. Indichiamo con $\psi:[c,d]\to[a,b]$ la funzione inversa di $\phi$. 
Supponiamo che $\phi$ sia derivabile in un punto $x_{0}\in [a,b]$, e sia $\phi^{'}(x_{0})\not= 0$.
Supponiamo che $\psi$ sia [[Funzioni continue|continua]] nel punto $y_{0}= \phi(x_0)$
Allora $\psi$ è derivabile in $y_0$ e si ha
$$\psi^{'}(y_{0})= \frac{1}{\phi^{'}(x_0)}$$
Equivalentemente si può scrivere
$$\psi^{'}(y_{0})= \frac{1}{\phi^{'}(\psi(y_0))}\qquad \mbox{oppure}\qquad \psi^{'}(\phi(x_0))= \frac{1}{\phi^{'}(x_0)}$$
#dimostrazione-da-fare 

# Derivata funzione composta
Sia $f:[a,b]\to \mathbb{R}$. Supponiamo che i valori di $f$ appartengano all'intervallo $[c,d]$, e sia $x_0\in[a,b]$. 
Sia $g:[c,d]\to\mathbb{R}$  e poniamo $y_{0}= f(x_0)\in[c,d]$.
Supponiamo che $f$ sia derivabile in $x_0\in[a,b]$ e che $g$ sia derivabile in $y_0=f(x_0)$.
Allora $F:=g\circ f$ è derivabile in $x_0$ e si ha
$$(g\circ f)^{'}(x_{0)} = g(f(x_{0})) f^{'}(x_{0})$$
#dimostrazione-da-fare 

# Punti di minimo agli estremi
Sia $f:[a,b]\to\mathbb{R}$ una funzione
- Se $f$ è derivabile in $a$ e se $f(a)$ è il valore minimo di $f$ allora$$f^{'}(a)\ge0$$- Se $f$ è derivabile in $b$ e se $f(b)$ è il valore minimo di $f$ allora$$f^{'}(b)\le0$$
#dimostrazione-da-fare 
# Punti di massimo agli estremi
Esattamente come sopra ma a segno invertito
#dimostrazione-da-fare 

# Corollario 17.2.4 | Punti di minimo e massimo interni
Sia $I \subseteq \mathbb{R}$ un intervallo, e $f:I\to\mathbb{R}$ una funzione reale. 
- Se in un punto $c$ interno all'intervallo la $f$ assume il suo valore minimo, e se $f$ è derivabile in $c$, allora
$$f^{'}(c)=0$$
 - Se in un punto $c$ interno all'intervallo la $f$ assume il suo valore massimo, e se $f$ è derivabile in $d$, allora 
$$f^{'}(d)=0$$
#dimostrazione-da-fare 

# Rolle
[[Teorema di Rolle]]
# Cauchy
[[Teorema di Cauchy]]
# Lagrange
[[Teorema di Lagrange]]

# Teorema 17.2.13
Se una funzione derivabile $f:I\to\mathbb{R}$ ha derivata positiva in ogni punto $x\in I$ allora $f$ è crescente in $I$.
#dimostrazione-da-fare 