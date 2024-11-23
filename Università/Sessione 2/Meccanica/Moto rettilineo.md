---
pagina: 7
---
# Legge oraria
![[Legge oraria]]

# Velocità
![[Velocità#Velocità in 1 dimensione]]
# Accelerazione
![[Accelerazione]]
# Moto rettilineo uniforme
Un corpo si muove di moto rettilineo uniforme quando la sua legge oraria è una funzione lineare$$x(t)=ct+b$$La [[Velocità]] in un moto rettilineo uniforme è costante, dato che 
$$v = \frac{dx}{dt}=c.$$
La costante $b$ nella legge del moto rappresenta la posizione iniziale del punto, ovvero la posizione che occupa per $t = 0$.
# Moto uniformemente accelerato
Analizziamo un grave che cade in direzione verticale con accelerazione di gravità $a = -g= -9,81 \frac{m}{s^2}$ verso il basso.
Possiamo determinare la [[Velocità]] integrando, scoprendo che varia con una legge lineare$$v=v_{0}+gt$$Integrando ancora, determiniamo la [[Legge oraria|Posizione]], che varia con legge parabolica$$y = y_0+v_{0}t-\frac{1}{2}gt^{2}$$
# Moto armonico
![[Moto armonico.png]]
Partiamo analizzando lo spostamento del punto materiale e derivando calcoleremo la velocità e l'accelerazione.
In un moto armonico lo spostamento è dato dalla seguente [[Legge oraria]]$$x(t)=A\sin(\omega t+\phi)\qquad[m]$$Derivando otteniamo che$$v(t)=A\omega\cos(\omega t+\phi)\qquad [\frac{m}{s}]$$Derivando ancora,$$a(t)=-A\omega^{2}\sin(\omega t+\phi)=-\omega^{2}x(t)\qquad[\frac{m}{s^{2}}]$$$A$ è l'ampiezza(lunghezza)
$\omega$ la pulsazione(angolo / tempo)
$\phi$ la fase (angolo)

---
Nel [[Pendolo]]
$$\omega = \sqrt{\frac{g}{L}}$$
---

Essendo la funzione del seno periodica, definiamo il ==periodo dell'oscillazione==  come $$T=\frac{2\pi}{\omega}\qquad [s]$$Inoltre definiamo la ==frequenza== come il reciproco del periodo
$$f=\frac{1}{T}=\frac{\omega}{2\pi}\qquad[\frac{1}{s}]=[H_{z}]$$
# Moto smorzato esponenzialmente
Questo modello fisico si trova quando analizziamo il moto di corpi all'interno di fluidi viscosi.

Si studia il moto smorzato esponenzialmente partendo dall'[[Accelerazione]], che è definita come $$a(t)=-kv(t)$$
Dove $k [\frac{1}{s}]$ è costante.
!! Importante, non si usano gli $H_{z}$ per $k$.
Per trovare la [[Velocità]], dobbiamo risolvere l'equazione differenziale
$$\frac{dv}{dt}=-kv(t)$$
Allora$$\frac{dv}{v}=-kdt\Rightarrow\int_{v_{0}}^{v}dv(v)=\int_{0}^{t}-kdt\Rightarrow \ln(\frac{v}{v_{0}})=-kt$$Allora $$v(t)=v_{0}e^{-kt}$$
Per trovare la [[Legge oraria]], conoscendo la posizione iniziale, integriamo ancora
$$x(t)=x_{0}+\int_{0}^{t}v(t)dt=x_0+\int_{0}^{t}v_{0}e^{-kt}dt$$
Allora
$$x(t) = x_{0}+(1-e^{-kt})\frac{v_{0}}{k}$$
