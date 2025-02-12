Data una funzione $f:\mathbb{R}\to \mathbb{R}$ consideriamo il problema di trovare di zeri o radici della funzione, ovvero i valori di $x$ tali che
$$f(x)=0$$

Il nostro scopo, dato che non sono disponibili formule esplicite per la determinazione di radici di una funzione(ad esempio per equazioni algebriche di $n>4$)

Facciamo allora uso di metodi iterativi
>[!def] Metodi iterativi
>Metodi che consentono di approssimare le soluzioni di $$f(x)=0$$ con un prestabilito grado di precisione.
>Si $P$ un problema ed $\alpha$ una soluzione del problema $P$, si vuole utilizzare il procedimento iterativo che genera una successione $\{x_{i}\}_{i=0,1,\ldots}$ convergente ad $\alpha$
>$$\lim_{i\to\infty}x_{i}=\alpha$$


Sono fondamentali 3 concetti
- L’innesco
- La convergenza 
- L’arresto

## Scelta dell’innesco e convergenza
Consideriamo procedimenti iterativi ad un passo
$$x_{i+1}=\phi(x_{i})$$
Sarà necessario, per poter innescare il procedimento $x_{0}$

>[!def] Convergenza locale
>Un metodo converge localmente ad $\alpha$ se la convergenza della successione $\{x_i\}_{i=1,2,\ldots}$ dipende in modo critico dalla vicinanza di $x_{0}$ a $\alpha$

>[!def] Convergenza globale
>Un metodo converge localmente ad $\alpha$ quando la convergenza non dipende da quanto $x_{0}$ sia vicino ad $\alpha$.

>[!def]