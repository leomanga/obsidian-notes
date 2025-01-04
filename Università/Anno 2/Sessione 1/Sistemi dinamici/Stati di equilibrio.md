>[!def] Stato di equilibrio
>$\bar{x}\in \mathbb{R}^{n}$ si dice stato di equilibrio di un sistema dinamico se
>$$x(0)=\bar x\Rightarrow x(t)=\bar x\ \ \forall t>0$$

L’utilità degli stati di equilibrio è quello di avere stati per cui eseguire le [[Tecniche di linearizzazione dei sistemi dinamici non lineari]].
## Caso tempo continuo
Nel caso di un sistema tempo invariante autonomo (non influenzato da un ingresso $u$) avremo $\dot{x}(t)=f(x(t))$.
Gli stati di equilibrio di $\bar x$ sono quelli tali che $$f(\bar x)=0$$

Nel caso di in sistema tempo invariante a tempo continuo non autonomo invece avremo $\dot{x}(t)=f(x(t),u(t))$
Dato $u(t)=\bar{u}\ \ \forall t\ge 0$ gli stati di equilibrio sono quelli tali che $$f(\bar x,\bar u)=0$$
In entrambi i casi dobbiamo risolvere un sistema $n$ equazioni in $n$ variabili. Non esiste un modo generale per farlo e può essere molto complicato.
(Pag 103) appunti per esempio.
## Caso tempo discreto
Nel caso di un sistema tempo invariante avremo $x(k+1)=f(x(k),u(k))$
Dato $u(k)=\bar u\ \ \forall k\ge 0$, gli stati di equilibrio saranno quelli tali che
$$f(\bar x,\bar u)=\bar x\iff f(\bar x,\bar u)-\bar x=0$$
## Stato di equilibrio stabile
Uno stato di equilibrio $\bar x$ si dice stabile se
$$\forall \epsilon>0,\ \ \exists\delta>0:||x(0)-\bar x||<\delta\Rightarrow||x(t)-\bar x||<\epsilon\ \ \forall t\ge 0$$













