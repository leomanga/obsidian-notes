# Definizione
Sia $(X,d)$ uno [[Spazi metrici|spazio metrico]] e sia $(x_n)\subseteq X$ una successione di punti nello spazio metrico $X$.
Allora si dice che $x_n$ tende a $x\in X$ se e solo se vale 
$$\lim_{n\to+\infty}d(x_n,x)=0$$
Equivalentemente valgono le seguenti proprietà:
$$i)\forall \epsilon > 0\ \exists N_\epsilon\in \mathbb{N}:d(x_n,x)<\epsilon\ \forall n \ge N_\epsilon$$
$$ii)\forall r>0\ \exists N_{r}\in\mathbb{N}: x_{n}\in B_{r(x)}\ \forall n\ge N_r$$
[^1]
# Metodo delle rette
(trovato online) (Qua c'è anche altro [Limiti in due variabili (youmath.it)](https://www.youmath.it/lezioni/analisi-due/varie/814-limiti-di-funzioni-di-due-variabili.html))
In questo metodo si cerca di muoverci lungo una retta, facendo dipendere tutte le variabili ad una sola.

Ad esempio se vogliamo calcolare $$\lim_{(x,y)\to(0,0)}\frac{x^{2}y}{{x+y}}$$
Possiamo scrivere $y-0=m(x-0)$ (Al posto degli zeri chiaramente vanno messi i punti a cui vogliamo far tendere la funzione).

A questo punto potremo riscrivere la funzione, facendola dipendere solo da $x$. Se il limite di $x\to 0$ in questo caso non esistesse o dipendesse da $m$, allora il limite non esisterebbe.
# Definizione | successione convergente
Una successione per la quale esiste $x$ tale per cui $x_{n}\to x$ si dice successione convergente.









[^1]: Br è la [[Palla]] di centro x e raggio r. 