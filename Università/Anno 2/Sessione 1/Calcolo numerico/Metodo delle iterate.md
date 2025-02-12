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

>[!thm] Ostrowski
>Sia $\alpha$ un punto fisso di $g\in C^{1}[\alpha-\rho,\alpha+\rho]$