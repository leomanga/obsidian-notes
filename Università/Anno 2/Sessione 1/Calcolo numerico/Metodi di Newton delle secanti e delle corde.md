Il principio di questi metodi è quello di linearizzare una data funzione $f(x)$ partendo da un punto $x_{0}$
$$y=f(x_{0})+m(x-x_{0})$$
Otterremo che, per $f(x)=0$, $y=0$, quindi
$$x_{1}=x_{0}-\frac{f(x_{0})}{m}$$
In generale $$x_{i+1}=x_{i}-\frac{f(x_{i})}{m_{i}}$$
In base alla scelta di $m_{i}$ otteniamo
- metodo delle corde per $m_{i}= m$
- metodo delle secanti e di Newton

# Metodo delle secanti
Prendiamo un $m_{i}$ come coefficiente angolare della retta per $(x_{i}, f(x_{i}))$  e $(x_{i-1},f(x_{i-1}))$
$$m_{i}=\frac{f(x_{i})-f(x_{i-1})}{(x_{i}-x_{i-1})}$$
Allora $$x_{i+1}=x_{i}-f(x_{i})\frac{(x_{i}-x_{i-1})}{f(x_{i})f(x_{i-1})}$$
## Convergenza
La convergenza è garantita se le approssimazioni iniziali sono “abbastanza vicine” alla radice $\alpha$, quindi avremo una [[Metodi numerici per equazioni non lineari#^7b166b|convergenza locale]].

# Metodo di Newton
Prendiamo $m_{i}$ come derivata prima di $f$ in $x_{i}$
$$m_{i}=f^{'}(x_{i})$$
$$x_{i+1}=x_{i}-\frac{f(x_{i})}{f^{'}(x_{i})}$$
## Convergenza
Abbiamo una convergenza locale ed un aumento del costo computazionale, però la [[Metodi numerici per equazioni non lineari#^d65c76|velocità di convergenza]] è di ordine superiore al primo. (In generale è quadratica).

>[!thm] convergenza globale
>Sia $f\in C^{2}[\alpha,\alpha+\rho]$ tale che
>$f(x)f''(x)>0$ in ($\alpha, \alpha+\rho$)
>$f’(x)\not = 0$ in ($\alpha,\alpha+\rho$)
>Allora $\forall x_{0}\in (\alpha, \alpha +\rho]$ la successione originata dal metodo di Newton DECRESCE monotonicamente ad $\alpha$.
>Per gli intorni sinistri $[\alpha-\rho,\alpha)$ si ottiene una successione che converge in modo monotono CRESCENTE ad $\alpha$.

