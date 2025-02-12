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

^7b166b

>[!def] Convergenza globale
>Un metodo converge localmente ad $\alpha$ quando la convergenza non dipende da quanto $x_{0}$ sia vicino ad $\alpha$.

>[!def] Velocità di convergenza
>Data una successione $\{x_{i}\}$ convergente ad $\alpha$, si ponga $e_{i}:=x_{i}-\alpha$.
>Se esistono due numeri reali $p$ e $C$ tali che sia 
>$$\lim_{i\to\infty}\frac{|e_{i+1}|}{|e_{i}|^{p}}=C$$
>si dice che la successione ha ordine di convergenza $p$ e fattore di convergenza $C$.

^d65c76

## Criteri di arresto
Non è chiaramente possibile generare infinite iterate della successione, il metodo dovrebbe arrestarsi ad ina certa tolleranza
$$|e_{i}|=|x_{i}-\alpha|<toll$$
Non disponendo una soluzione $\alpha$, si approssima $e_{i}$ con $|x_{i+1}-x_{i}|<toll_{A}$
Questo criterio prende il nome di **criterio di arresto assoluto** e può chiaramente fallire, in base alla grandezza della tolleranza e di $x_{i}$.

Un altro modo è quello di usare un **criterio di arresto relativo**, dato da
$$\frac{|x_{i+1}-x_{i}|}{|x_{i+1}|}<toll_{R} $$
Dove è importante che $toll_{R}>\epsilon_{r}$ che è la  [[Rappresentazione numeri nei calcolatori#^ff68fc|precisione di macchina]].
Questo metodo non è molto affidabile se la convergenza è lenta.

Per equazioni non lineari si piò anche usare il **controllo del residuo**
$$|f(x_{i+1})|\le toll$$
In questo caso però
- Se $|f^{'}(\alpha)|>>1$ il controllo sarà troppo restrittivo.
- Se $|f^{'}(\alpha)|<<1$ il controllo sarà inaffidabile.
- Se $|f^{'}(\alpha)|\simeq 1$ avremo un’ indicazione soddisfacente. 

# Lista di metodi
[[Metodo di bisezione]]
[[Metodi di Newton delle secanti e delle corde]]
[[Metodo delle iterate]]
