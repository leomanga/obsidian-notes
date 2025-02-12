La ricerca degli zeri  di una funzione $f$ è ridotta allo studio dei punti fissi di un’opportuna funzione $g$:
$$f(\alpha)=0\iff g(\alpha)=\alpha$$
La successione delle approssimazioni sarà definita, assegnato $x_{0}$ come
$$x_{i+1}=g(x_{i})$$
La funzione $g$ non è unica e può essere costruita nei modi più diversi.

Possiamo risalire a [[Metodi di Newton delle secanti e delle corde]]
- Ex corde
$$f(x)=0\iff x- \frac{f(x)}{m}=x\Rightarrow g(x)=x-\frac{f(x)}{m}$$
- Ex newton
$$f(x)=0\iff x-\frac{f(x)}{f^{'}{(x)}}=x\Rightarrow g(x)=x-\frac{f(x)}{f^{'}(x)}$$

## Convergenza

>[!thm] Ostrowski
>Sia $\alpha$ un punto fisso di $g\in C^{1}[\alpha-\rho,\alpha+\rho]$ ([[Classi di funzioni#^08c68a]])
>Se $|g'(x)|<1,\forall x\in[\alpha-\rho,\alpha+\rho]$
>Allora $\forall x_{0}\in [\alpha-\rho,\alpha +\rho]$ la successione delle iterate generata da $g$ è tale che 
>$$\begin{split}&x_{i}\to \alpha\mbox{ unico punto fisso di } g\\&x_{i}\in [\alpha-\rho,\alpha +\rho]\end{split}$$ 

La convergenza può esserci anche in insiemi molto più grandi di quelli in cui $|g'(x)<1|$

>[!thm]
>Sia $\alpha\in I$ punto fisso di $g\in C^{p}[I]$ con $p\ge 2$. ([[Classi di funzioni]])
>Se per un punto $x_{o}\in I$ la successione $\{x_i\}$ è convergente e se 
>$$g'(\alpha)=g''(\alpha)=\ldots=g^{(p-1)}(\alpha)=0\mbox{ e } g^{(p)}(\alpha)\not=0$$
>allora il metodo ha [[Metodi numerici per equazioni non lineari#^d65c76|ordine di convergenza]] $p$ e risulta 
>$$\lim_{i\to\infty}\frac{|x_{i+1}-\alpha|}{|x_{i}-\alpha|^{p}}=\frac{g^{(p)}(\alpha)}{p!}$$
>