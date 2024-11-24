---
collegamenti:
  - "[[Sistemi di misura#Sistema internazionale]]"
  - "[[Legge oraria]]"
  - "[[Velocità]]"
---
# Accelerazione in 1 dimensione
## Accelerazione media
Consideriamo un punto materiale che si muove di [[Moto rettilineo]], in cui la posizione è descritta dalla [[Legge oraria]] $x(t)$, da cui possiamo ottenere la [[Velocità]] $v(t)=\frac{dx(t)}{dt}$.
L'accelerazione media è definita come
$$a_{m1,2}=\frac{v(t_{2}-v(t_{1}))}{t_{2}-t_{1}}=\frac{\Delta v_{1,2}}{\Delta t_{1,2}}\qquad [\frac{m}{s^{2}}]$$
dove $v$ è la velocità in funzione di un certo tempo $t_{1}$ e $t_{2}$.
## Accelerazione istantanea
Si definisce accelerazione istantanea $a$ nel punto $x$ all'istante $t$ il risultato della seguente espressione
$$a=\lim_{\Delta t\to 0}\left(\frac{v(t+\Delta t)-v(t)}{\Delta t}\right)=\frac{dv}{dt}$$
In poche parole rappresenta la derivata della [[Velocità]], valutata in un certo tempo $t$. 
Dato che $v=\frac{dx}{dt}$, possiamo definire $a$ come
$$a = \frac{d^{2}x}{dt^{2}}$$
Dove $x$ è la [[Legge oraria]]. ^eb6080

# Accelerazione in 2 dimensioni
## Accelerazione istantanea
Si definisce il vettore accelerazione come la derivata rispetto al tempo del [[Velocità#Velocità in 2 dimensioni#Velocità istantanea|velocità istantanea]], che è a sua volta una [[Derivata di un vettore|derivata]] del vettore posizione.
$$\vec{a}=\frac{d\vec{v}}{dt}$$
Il vettore velocità ($v=$ [[Velocità#^8b051f]]) può variare sia in modulo che in direzione in funzione del tempo, sviluppiamo allora la sua derivata
$$
\begin{split}
\vec{a}=\frac{d\vec{v}}{dt}=\frac{d(v\vec{u}_{t})}{dt}=\frac{dv}{dt}\vec{u}_{t}+v\frac{d\vec{u}_{t}}{dt}

\end{split}
$$
Possiamo osservare quindi che il vettore accelerazione ha 2 componenti. 
- $\frac{dv}{dt}\vec{u}_{t}$ è una componente ==diretta come== $\vec{u}_{t}$ (è tangente allora alla curva della posizione) e ==descrive come varia il modulo della velocità lungo la traiettoria== grazie al termine $\frac{dv}{dt}$.
- $v\frac{d\vec{u}_{t}}{dt}$ descrive come varia il versore $\vec{u}_{t}$ nel tempo, ==tiene conto quindi di come varia la direzione della velocità.== 

Focalizziamoci ora sul secondo termine $v\frac{d\vec{u}_{t}}{dt}$ e calcoliamo innanzi tutto $$\frac{d\vec{u}_{t}}{dt}=\lim_{\Delta t\to 0}\frac{\Delta\vec{u}_{t}}{\Delta t}$$
dove $\Delta\vec{u}_{t}=\vec{u}_{t}(t+\Delta t)-\vec{u}_{t}(t)$.
Osserviamo che la costruzione di $\Delta\vec{u}_{t}$ forma un triangolo isoscele, quindi possiamo calcolare il suo modulo$$|\Delta\vec{u}_{t}|=d|\vec{u}_{t}(t)|\sin(\frac{\Delta\varphi}{2})\cong\Delta\varphi$$
Possiamo quindi scrivere $$\left|\frac{\Delta\vec{u}_{t}}{\Delta t}\right|\cong\frac{\Delta\varphi}{\Delta t}$$
Per $\Delta t\to 0$, la direzione di $\Delta \vec{u}_{t}$ tende alla direzione perpendicolare a $\vec{u}_{t}$, definita dal versore $\vec{u}_{n}$, ovvero il versore normale. 
![[Componenti accelerazione 2 dim.png]]

Possiamo ora sviluppare il rapporto $\frac{\Delta\varphi}{\Delta t}$.

Possiamo approssimare localmente la curva con una circonferenza di raggio $R$ e centro $\Omega$, detta ==circonferenza osculatrice==.

Allora $\Delta\varphi=\frac{\Delta s}{R}$ e per $\Delta t\to 0$ risulta$$\frac{d\varphi}{dt}=\lim_{\Delta t\to 0}\frac{\Delta\varphi}{\Delta t}=\lim_{t\to 0}\frac{\Delta s}{\Delta t}\frac{1}{R}=\frac{1}{R}\frac{ds}{dt}=\frac{v}{R}$$
Il passaggio da $\frac{ds}{dt}$ a $v$ si trova qua [[Velocità#^8b051f]].
![[Circonferenza osculatrice.png]]
 
 Osservazioni
- Il centro e il raggio della circonferenza osculatrice variano lungo la traiettoria.
- Il versore normale $\vec{u}_{n}$ è diretto sempre verso il centro della traiettoria. (direzione centripeta)

Adesso possiamo riscrivere il vettore $\vec{a}$ come $$\vec{a}=\frac{d\vec{v}}{dt}=\frac{dv}{dt}\vec{u}_{t}+v\frac{d\vec{u}_{t}}{dt}=\frac{dv}{dt}\vec{u}_{t}+\frac{v^2}{R}\vec{u}_{n}$$
Abbiamo quindi verificato che il vettore accelerazione è formato da due componenti,
uno diretto secondo la tangente della traiettoria $\vec{u}_{t}$ e l'altro secondo la direzione normale $\vec{u}_{n}$
$$
\vec{a}=a_{t}+a_{n}
$$

^1e403d

dove 
$$
\vec{a}_{t}=\frac{dv}{dt}\vec{u}_{t}
$$

^5073ea

e
$$
\vec{a}_{n}=\frac{v^{2}}{R}\vec{u}_{n}
$$

^d5acd3

$\vec{a}_{n}$ è sempre maggiore o uguale a zero, non può mai andare verso il fuori.
![[Componenti accelerazione.png]]

Il modulo del vettore accelerazione si può calcolare come $$a = \sqrt{a_{t}^{2}+a_{n}^{2}}$$
Possiamo inoltre esprimere l'accelerazione attraverso le componenti cartesiane
$a_{x}=\frac{dv_{x}}{dt}=\frac{d^{2}xt}{dt}$
$a_{y}=\frac{dv_{y}}{dt}=\frac{d^{2}yt}{dt}$
