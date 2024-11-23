---
cap: "16"
---
# Limiti infiniti in un punto
Sia $f:E\subseteq \mathbb{R} \to \mathbb{R}$ e $\bar x \in \bar E$. 
Si dice che $f$ tende a $+\infty$ per $x$ tendente a $\bar x$ su $E$, e scriveremo
$$\lim_{x\to\bar x}f(x) = +\infty\mbox\qquad\mbox{su E}$$
Se per ogni [[Serie numeriche a termini di segno costante#Successione|successione]] $x_n$ di punti di $E$ che converge a $\bar x$ si ha
$$\lim_{n\to+\infty}f(x_{n)}= +\infty$$
- Uguale con segno opposto nel caso di $-\infty$.
### Definizione
Nel caso di $+\infty$
$$\forall M \in \mathbb{R},\ \exists \delta_{M}>0: \forall x\in E, |x-\bar x| < \delta_{M}\ f(x)>M$$
#dimostrazione-da-fare 
# Limiti finiti all'infinito
Sia $\mathbb{E} \subseteq \mathbb{R}$ un insieme non [[Estremo superiore e inferiore#Insieme superiormente e inferiormente limitato|superiormente limitato]], $f:E \to \mathbb{R}$. Si dice che $f$ tende a $\ell$ per $x$ tendente a $+\infty$ su $E$ e scriviamo
$$\lim_{x\to+\infty}f(x) = \ell\qquad \mbox{su E}$$
se per ogni successione $x_n$ di punti di $E$ divergente verso $+\infty$ si ha
$$\lim_{n\to+\infty}f(x_n)=\ell$$
- Stessa cosa nel caso di un insieme non [[Estremo superiore e inferiore#Insieme superiormente e inferiormente limitato|inferiormente limitato]].
### Definizione
Nel caso di $+\infty$.
$$\forall \epsilon > 0\ \exists K_{\epsilon}\in\mathbb{R}: \forall x \in E, x>K_{\epsilon}, |f(x)-\ell| < \epsilon$$
#dimostrazione-da-fare 

# Limiti infiniti all'infinito
Sia $\mathbb{E} \subseteq \mathbb{R}$ un insieme non [[Estremo superiore e inferiore#Insieme superiormente e inferiormente limitato|superiormente limitato]], $f:E \to \mathbb{R}$. Si dice che $f$ tende a $\pm \infty$ per $x$ tendente a $+\infty$ su $E$  e scriviamo
$$\lim_{x\to+\infty}f(x) = \pm\infty\qquad \mbox{su E}$$
se per ogni successione $x_n$ di punti di $E$ divergente verso $+\infty$ si ha
$$\lim_{n\to+\infty}f(x_n)=\pm\infty$$
- Stessa cosa nel caso di un insieme non [[Estremo superiore e inferiore#Insieme superiormente e inferiormente limitato|inferiormente limitato]]

### Definizione
Nel caso di $+\infty$
$$\forall M \in \mathbb{R}\ \exists K_M \in \mathbb{R}: \forall x \in E, x>K_M, f(x)>M$$

# Teorema 16.0.11
Sia $f:E\subseteq \mathbb{R}\to\mathbb{R}$ una funzione. Supponiamo che $E$ non sia  [[Estremo superiore e inferiore#Insieme superiormente e inferiormente limitato|superiormente limitato]] e che $f$ sia non decrescente.
Allora si ha
$$\lim_{x\to+\infty}f(x) = \sup f(E)\mbox{ su E}$$
#dimostrazione-da-fare 