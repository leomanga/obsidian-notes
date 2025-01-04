>[!def] Stato di equilibrio
>$\bar{x}\in \mathbb{R}^{n}$ si dice stato di equilibrio di un sistema dinamico se
>$$x(0)=\bar x\Rightarrow x(t)=\bar x\ \ \forall t>0$$

L’utilità degli stati di equilibrio è quello di avere stati per cui eseguire le [[Tecniche di linearizzazione dei sistemi dinamici non lineari]].
# Casi
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
# Diversi tipi di equilibri
![[Stabilità dei sistemi dinamici#^3ca209]]

^a3abc3

>[!def] Stato di equilibrio convergente
>Uno stato di equilibrio $\bar x$ si dice convergente se
>$$\exists \delta>0:||x(0)-\bar x||<\delta\Rightarrow\lim_{t\to{\infty}}||x(t)-\bar x||=0$$
>In poche parole se, perturbando minimamente lo stato di equilibrio, il sistema, nel tempo, tornerà allo stato di equilibrio.
>Un esempio può essere una pallina in fondo ad un avvallamento. Se le cambiamo posizione, essa tornerà all’equilibrio in fondo all’avvallamento.

^8441cb
# Studio degli stati di equilibrio
### Sistemi autonomi
Consideriamo un sistema autonomo a tempo continuo
$$\dot x(t)=A\cdot x(t)$$
Gli stati di equilibrio saranno $\bar x:A\cdot \bar x=0$
Risolvendo il sistema lineare di $n$ equazioni in $n$ incognite si ha che
- Se $\det(A)\not = 0$ allora $\bar x=0$ è l’unico stato di equilibrio
- Se $\det(A)=0$ allora esistono infiniti stati di equilibrio $\bar x\in \ker(A)$. ($\ker$ è il [[Kernel di una funzione lineare|Kernel]])

Se consideriamo un sistema autonomo a tempo discreto
$$x(k+1)=A\cdot x(k)$$
Gli stati di equilibrio saranno $\bar x:A\cdot \bar x=\bar x\iff (I-A)\cdot \bar x=0$
Risolvendo il sistema lineare di $n$ equazioni in $n$ incognite si ha che
- Se $\det(I-A)\not = 0$ allora $\bar x=0$ è l’unico stato di equilibrio
- Se $\det(I-A)=0$ allora esistono infiniti stati di equilibrio $\bar x\in \ker(I-a)$. ($\ker$ è il [[Kernel di una funzione lineare|Kernel]])

### Sistemi non autonomi
Consideriamo un sistema autonomo a tempo continuo
$$\dot x(t)=A\cdot x(t)+B\cdot u(t)$$
con $u(t)=\bar u\ \ \forall t$. 
Gli stati i equilibrio saranno
$$\bar x:A\cdot \bar x+B\cdot \bar u =0$$
Avremo un sistema di $n$ equazioni in $n$ incognite
$$A\cdot \bar x=-B\cdot \bar u$$
Si ha che
- Se $\det(A)\not = 0$ allora $\bar x=-A^{-1}\cdot B\cdot \bar u$ è l’unico stato di equilibrio
- Se $det(A)=0$ allora
	- esistono infiniti stati di equilibrio se $-B\cdot \bar u\in Im(A)$
	- non esistono stati di equilibrio se $-B\cdot \bar u\not\in Im(A)$
# Stabilità
![[Stabilità dei sistemi dinamici]]



 









