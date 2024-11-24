# Pendolo semplice
Consideriamo un punto materiale $P$ di massa $m$ sospeso con un filo inestensibile di lunghezza $L$ fissato in un punto $O$.

Indichiamo con $\vartheta$ l'angolo che forma il filo con la verticale in una generica configurazione.

Essendo il filo inestensibile, ed essendo fissato in $O$.
Il punto $P$ si muove lungo un arco di circonferenza di centro $O$ e raggio $L$.
![[Pendolo semplice.png]]

Sul punto agiscono due forze
- La forza peso $\vec{F}_{p}=m\vec{g}$
- La tensione del filo $\vec{T}_{f}$
La risultante delle forze sarà quindi 
$$\vec{R}=\vec{F}_{p}+\vec{T}_{f}$$
Applicando la [[Capitolo 5 - Dinamica del punto materiale 1#^ee9546|seconda legge di Newton]] risulta
$$m\vec{a}=\vec{R}$$

Se il pendolo è nella configurazione in cui il filo è verticale ($\vartheta=0$), $\vec{F}_{p}$ e $\vec{T}_{f}$ hanno la stessa direzione, quindi
$$\vec{R}=0$$
Per una configurazione del pendolo ed applicando la seconda legge di Newton si ottiene
$$m\vec{a}=\vec{R}=\vec{F}_{p}+\vec{T}_{f}=mg+\vec{T}_{f}$$
Ricordiamoci che l'[[Accelerazione#Accelerazione in 2 dimensioni|accelerazione]] in un moto bidimensionale può essere descritta come $$\vec{a}=\vec{a}_{t}+\vec{a}_n$$
$\vec{a}_{t}$ è la componente tangenziale all'arco di circonferenza percorso dal punto materiale
$\vec{a}_{n}$ è la componente normale, diretta come il filo.

Possiamo scomporre la risultante $\vec{R}$ nelle stesse direzioni
$$\vec{R}=\vec{R}_{t}+\vec{R}_{n}=m\vec{a}_{t}+m\vec{a}_{n}$$
Osservando le relazioni geometriche si ottiene
$$R_{n}=T_{f}-mg\cos\vartheta$$
$$\vec{R}_t=-mg\sin\vartheta$$
Ma, dato che $ma_{t}=R_{t}=-mg\sin\vartheta$, allora
$$a_{t}=-g\sin\vartheta$$

## Calcolo di $\vartheta(t)$
Consideriamo la componente tangenziale $\vec{a}_{t}=-g\sin\vartheta\vec{u}_t$
Ricordiamo che $\vec{a}_{t}=\frac{d^{2}s}{dt^{2}}\vec{u}_{t}=-g\sin\vartheta$ 
Inoltre possiamo descrivere l'ascissa curvilinea $s=L\vartheta$, dove $L$ è la lunghezza del filo.
Allora otteniamo che
$\vec{a}_{t}=L\frac{d^{2}\vartheta}{dt^2}\vec{u}_{t}$
$\vec{a}_{n}=\frac{v^{2}}{L}\vec{u}_{n}$
Sostituendo nell'equazione del moto si ottiene
$$L\frac{d^{2}\vartheta}{dt^2}=-g\sin\vartheta$$
Non è facile da risolvere, ma per piccole oscillazioni possiamo approssimare $\sin\vartheta\sim\vartheta$
Otteniamo allora
$$L\frac{d^{2}\vartheta}{dt^2}=-g\vartheta$$
Che possiamo scrivere come 
$$\frac{d^{2}\vartheta}{dt^2}+\frac{g}{L}\vartheta=0$$
Questa è l'equazione differenziale di un [[Moto rettilineo#Moto armonico|moto armonico]], $\vartheta=A\sin(\omega t+\phi)$ con pulsazione $$\omega=\sqrt{\frac{g}{L}}$$
La soluzione è
$$\vartheta(t)=\vartheta_{0}\sin(\omega t+\varphi)$$
L'ascissa curvilinea è quindi data da
$$s(t)=L\vartheta(t)=L\vartheta_{0}\sin(\omega t + \varphi)$$
La velocità è pari a
$$v=\frac{ds}{dt}=L\omega\vartheta_{0}\cos(\omega t+\vartheta)$$
La velocità angolare è pari a
$$\omega=\frac{d\vartheta}{dt}=\omega\vartheta_{0}\cos(\omega t+\varphi)$$
## Calcolo della tensione del filo
Per calcolare la tensione del filo dobbiamo risolvere
$$ma_{n}=m\frac{v^{2}}{L}=T_{f}-mg\cos\vartheta$$

