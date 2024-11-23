---
collegamenti:
  - "[[Sistemi di misura#Sistema internazionale]]"
  - "[[Legge oraria]]"
---
# Velocità in 1 dimensione
## Velocità media
Consideriamo un punto materiale che si muove di [[Moto rettilineo]].
La velocità media è definita come 
$$v_{m1,2}=\frac{x(t_{2})-x(t_{1})}{t_{2}-t_{1}}=\frac{\Delta x}{\Delta t}\qquad [\frac{m}{s}]$$
dove $x$ è la posizione occupata in funzione di un certo tempo $t_{1}$ e $t_{2}$.
## Velocità istantanea
Si definisce velocità istantanea $v$ nel punto $x$ all'istante $t$ il risultato della seguente espressione
$$v=\lim_{\Delta t\to 0}\left(\frac{x(t+\Delta t)-x(t)}{\Delta t}\right)=\frac{dx}{dt}$$
In poche parole rappresenta la derivata della [[Legge oraria]], valutata in un certo tempo $t$.  ^978331
## Passare dall'accelerazione istantanea alla velocità
Dato che, come definito [[Accelerazione#^eb6080|QUA]],$$a=\frac{dv}{dt}$$Allora$$adt=dv\Rightarrow \int_{0}^{t}a(t)dt=\int_{v_{0}}^{v}dv \Rightarrow v(t)=v_{0}+\int_{0}^{t}a(t)dt$$
# Velocità in 2 dimensioni
## Velocità media
### Rappresentazione con coordinate cartesiane
Supponiamo che $P$ percorra una traiettoria su un piano su cui abbiamo fissato un sistema di riferimento, rappresentiamo il moto nel piano con il vettore geometrico $\vec{r}(t)$.
Allora si definisce velocità media nell'intervallo $[t_{1},t_{2}]$ il vettore $$\vec{v_{m}}=\frac{\Delta \vec{r}}{\Delta t}$$  ![[Velocità media due dimensioni.png]]
La velocità media è un vettore che ha
- Modulo pari a $v_{m}=\frac{\Delta r}{\Delta t}=\frac{|P(t_{2})-P(t_{1})|}{\Delta t}\qquad [\frac{m}{s}]$
- Per direzione la retta che passa per $P(t_{2})$ e $P(t_{1})$
- Verso da $P(t_{1})$ a $P(t_{2})$
## Velocità istantanea
Per definirla è importante conoscere la [[Derivata di un vettore]], dato che la velocità istantanea $\vec{v}$ è definita come$$\vec{v}=\frac{d\vec{r}}{dt}=\lim_{\Delta t\to0} \frac{\Delta\vec{r}}{\Delta t}$$Osserviamo che per $\Delta t\to 0$, 
- La lunghezza del vettore $|\Delta \vec {r}|$ è pari alla lunghezza della corda lungo la traiettoria($\Delta s$). (In poche parole la sua lunghezza è uguale a quella dell'arco, chiaramente dato che $\Delta t\to 0$)
- La direzione è tangente alla traiettoria nel punto $P$, quindi possiamo scrivere $\vec{v}=v\vec{u}_{T}$ dove $v$ è il modulo della velocità e $\vec{u}_{T}$ il versore tangente alla curva, che è variabile nel tempo.

Inoltre possiamo anche trovare la componente scalare della velocità $$v = \frac{ds}{dt}=\dot{s}$$Non ci si deve confondere con il modulo della velocità, dato che $v$ è concorde con il verso di percorrenza della traiettoria.

Allora possiamo scrivere $\vec{v}$ come
$$\vec{v}=\frac{d\vec{r}}{dt}=\frac{ds}{dt}\vec{u_{T}}=v\vec{u}_{T}$$ ^8b051f

Dato che possiamo esprimere $\vec{r}(t)=x(t)\vec{i}+y(t)\vec{j}$, possiamo calcolare la velocità come$$\vec{v}=\frac{dx(t)}{dt}\vec{i}+\frac{dy(t)}{dt}\vec{j}$$
### Rappresentazione con coordinate polari
![[Velocità coordinate polari.png]]
				
Data la posizione di $\vec{r}(t)$ tramite la sua distanza $r(t)$ e dall'angolo $\theta(t)$ tra il segmento $\vec{OP}$ e l'asse $x$, possiamo definire il versore $\vec{u}_{r}$ che identifica la direzione del segmento $\vec{OP}$, allora il vettore posizione può essere scritto come$$\vec{r}=r\vec{u}_{r}$$
==Allora possiamo scrivere la velocità come ==$$\vec{v}=\frac{d\vec{r}}{dt}=\frac{d(r\vec{u}_{r})}{dt}=\underbrace{\frac{dr}{dt}\vec{u}_{r}+r \frac{d\vec{u}_{r}}{dt}}_{dalla\ derivazione\ dei\  vettori}$$
Analizzando la figura qua sotto, possiamo vedere che il vettore $\Delta\vec{u}_{r}$ :
- avrà modulo pari a $$\Delta u_{r}=2u_{r}(t+\Delta t)\sin(\frac{\Delta\vartheta}{2})\underbrace{\cong}_{per\ valori\ piccoli}\Delta\vartheta$$
- avrà direzione perpendicolare a $\vec{u}_{r}$ per $\Delta\vartheta\to 0$.
 ![[Coordinate polari velocità 2.png]]
 Allora possiamo scrivere che $\Delta\vec{u}_{r}\cong\Delta\vartheta\vec{u}_{\theta}$, essendo $\Delta\vec{u}_{\theta}$ un versore perpendicolare a $\vec{u}_{r}$.

==Possiamo riscrivere il vettore della velocità come==
$$\vec{v}=\frac{d\vec{r}}{dt}=\frac{d(r\vec{u}_{r})}{dt}=\frac{dr}{dt}\vec{u_{r}}+r\frac{d\vec{u}_r}{dt}$$
Inoltre, dato che $\Delta\vec{u}_{r}\cong\Delta\vartheta\vec{u}_{\theta}$, scriviamo che $$\vec{v}=\frac{dr}{dt}\vec{u}_{r}+r\frac{d\vartheta}{dt}\vec{u}_{\vartheta}$$
Possiamo allora definire le due componenti scalari della velocità lungo le direzioni di $\vec{u}_r$ e $\vec{u_{\vartheta}}$ come
$v_{r}=\frac{dr}{dt}$ e $v_{\vartheta}=r \frac{d\vartheta}{dt}$.

  ![[Velocità con coordinate polari, componenti.png]]
# Velocità nei moti relativi
[[Velocità - moti relativi]]