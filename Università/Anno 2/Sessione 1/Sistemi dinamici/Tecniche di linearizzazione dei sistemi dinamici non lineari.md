Dato un sistema iso non lineare
![[Sistemi non lineari#^c46d8f]]
Sia $\bar{x}(0), \bar{y}(0)$ la soluzione relativa a $\bar x_{0}$ e $\bar{u}(t)$.
Allora $\bar{x}(t)=f(\bar{x}(t),\bar{u}(t),t)$ e $\bar{y}(t)=h(\bar{x}(t),\bar{u}(t),t)$ 

Definiamo gli scostamenti della soluzione partiocolare
$$\Delta x(t)=x(t)-\bar x(t)$$
$$\Delta y(t)=y(t)-\bar{y}(t)$$
$$\Delta u (t)=u(t)-\bar{u}(t)$$
Cerchiamo di costruire un modello che abbia come variabili gli scostamenti
$\Delta\dot{x}(t)=\dot{x}(t)-\dot{\bar{x}}(t)=f(x(t),u(t),t)-f(\bar{x}(t),\bar{u}(t),t)$

Applicando la [[Formula di Taylor con resto di Peano]] in più dimensioni si ha
$$\begin{split}
\Delta\dot x(t)=&f(\bar{x}(t),\bar{u}(t),t) 
&&+\left[\frac{\partial f}{\partial x}\right]_{x=\bar x(t), u =\bar u(t)}\cdot \underbrace{(x(t)-\bar x(t))}_{{\Delta}x(t)}\\
&&&+\left[\frac{\partial f}{\partial u}\right]_{x=\bar x(t), u =\bar u(t)}\cdot \underbrace{(u(t)-\bar u(t))}_{{\Delta}u(t)}\\
&&&+o(||\begin{bmatrix}x(t)-\bar x(t)\\u(t)-\bar u(t)\end{bmatrix}||^{2})\\
&-f(\bar{x}(t),\bar{u}(t),t)\end{split}
$$
dove $\frac{\partial f}{\partial x}$ è la [[Ottimizzazione vincolata#^2dcc57|Jacobiana]] rispetto a $x$ e $\frac{\partial f}{\partial u}$ quella rispetto a $u$.

Trascurando i termini di grado $\ge 2$ e semplificando si ottiene un sistema lineare linearizzato nell’intorno della soluzione $\bar x(t),\bar u(t)$
$$\Delta x(t)\simeq A(t)\cdot \Delta x+B(t)\cdot u(t)$$
dove $A(t)=\left[\frac{\partial f}{\partial x}\right]_{x=\bar x(t), u =\bar u(t)}$ e $B(t)=\left[\frac{\partial f}{\partial u}\right]_{x=\bar x(t), u =\bar u(t)}$

Analogamente 
$$\Delta y(t)=C(t)\Delta x(t)+D(t)\Delta u(t)$$
dove $C(t)=\left[\frac{\partial h}{\partial x}\right]_{x=\bar x(t), u =\bar u(t)}$ e $D(t)=\left[\frac{\partial h}{\partial u}\right]_{x=\bar x(t), u =\bar u(t)}$.