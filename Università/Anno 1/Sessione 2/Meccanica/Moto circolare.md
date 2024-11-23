---
collegamenti:
  - "[[Punto materiale]]"
  - "[[Capitolo 4 - Cinematica moti bidimensionali]]"
---
# Introduzione
Un moto circolare è un moto in cui la traiettoria è una circonferenza. 
Supponiamo di avere un punto materiale $P$ che si muove di moto circolare, seguendo una circonferenza di centro $O$ e raggio $R$.
Fissiamo un sistema di riferimento che abbia come origine $O$ e asse $x$ diretto in modo tale che il punto materiale si trovi sull'asse stesso per $t=0$.
# Ascissa curvilinea
Al generico istante $t$, il punto si trova nella posizione $P(t)$ sulla circonferenza.
La sua posizione è definita dal raggio vettore $\vec{r}(t)$, che forma un angolo di $\vartheta$ con la direzione positiva dell'asse $x$.
Si può descrivere la posizione dall' ==ascissa curvilinea== $s$, l'arco percorso dal punto materiale a partire dalla sua posizione iniziale.
Essendo un arco di circonferenza risulta
> [!prp] Descrizione dell'ascissa curvilinea
> $$
> s(t)=R\vartheta(t)
> $$
> dove $R$ indica il raggio del cerchio.

Chiaramente per $t=0$, $s(0)=0$, quindi il punto $P$ si trova sull'asse $x$.
![[Ascissa curvilinea 1.png]]
# Componenti cartesiane del vettore posizione
Rispetto al sistema di riferimento, possiamo esprimere le coordinate del punto materiale come 
$$
x = R\cos\vartheta
$$

^75768e

$$
y=R\sin\vartheta
$$

^d21da9

# Velocitò nel tempo
Abbiamo visto, da [[Velocità#Velocità in 2 dimensioni#Velocità istantanea]], che la velocità in un generico istante è data da 
$$
\vec{v}=v\vec{u}_{t}
$$

^02a547

dove $\vec{u}_{t}$ è il vettore tangente alla traiettoria in quell'istante e $v=\frac{ds}{dt}$.
Abbiamo detto che, nel moto circolare, $s$ è definita come l' [[#Ascissa curvilinea|ascissa curvilinea]].
Allora, sostituendo $s=R\vartheta$ otteniamo
$$
v=\frac{ds}{dt}=\frac{dR\vartheta}{dt}=R\frac{d\vartheta}{dt}=R\omega
$$

^cc8e3c

Possiamo a questo punto introdurre
> [!clm] Velocità angolare $\omega$
> $$
> \omega=\frac{d\vartheta}{dt}
> $$
> Dai calcoli precedenti possiamo trovare delle relazioni fondamentali tra la velocità e la velocità angolare: 
> $$
> \omega = \frac{v}{R},\qquad v=R\omega
> $$

^42f45d

## Componenti cartesiane del vettore velocità
Derivando rispetto al tempo le [[#Componenti cartesiane del vettore posizione]] [[#^75768e]] e [[#^d21da9]], possiamo determinare le componenti cartesiane della velocità
$$
v_{x}=\frac{dx}{dt}=-R\frac{d\vartheta}{dt}\sin\vartheta=-R\omega\sin\vartheta=-v\sin\vartheta
$$

^7dbf1f

$$
v_{y}=\frac{dy}{dt}=R\frac{d\vartheta}{dt}\cos\vartheta=R\omega\cos\vartheta=v\cos\vartheta
$$

^8c7b20

# Accelerazione nel tempo
Abbiamo visto, da [[Accelerazione#Accelerazione in 2 dimensioni#Accelerazione istantanea]], che l'accelerazione in un generico istante è composta da un termine normale ed uno tangenziale alla traiettoria![[Accelerazione#^1e403d]]
Possiamo osservare che $R\vec{u}_{n}=-\vec{r}$, e da [[Accelerazione#^d5acd3]] possiamo scrivere la componente normale come:
> [!prp] Componente normale moto circolare
>$$\vec{a}_{n}=\frac{v^{2}}{R}\vec{u}_{n}=R\omega^{2}\vec{u}_{n}=-\omega^{2}\vec{r}
>$$

^079892

Mentre per la componente tangenziale, da [[#^02a547]] e da [[Accelerazione#^5073ea]], possiamo scrivere la componente tangenziale come:
> [!prp] Componente tangenziale moto circolare
> $$
\vec{a}_{t}=\frac{dv}{dt}\vec{u}_{t}=R\frac{d\omega}{dt}\vec{u}_{t}
> $$

^9bf2f6


Possiamo inoltre descrivere l'accelerazione tramite le sue componenti cartesiane.
Dobbiamo derivare le due equazioni 
![[#^7dbf1f]]
![[#^8c7b20]]

Otteniamo allora
$$
\begin{split}
a_x&=\frac{dv_{x}}{dt}=\frac{d(-R\omega\sin\vartheta)}{dt}=\\&\qquad=-R\omega\frac{d(\sin\vartheta)}{dt}-R\frac{d\omega}{dt}\sin\vartheta=\\
&\qquad=-R\omega\cos\vartheta \underbrace{\frac{d\vartheta}{dt}}_{\omega}-R\frac{d\omega}{dt}\sin\vartheta=\\
&=-R\omega^{2}\cos\vartheta-R\frac{d\omega}{dt}\sin\vartheta
\end{split}
$$
$$
\begin{split}
a_{y}&=\frac{dv_{y}}{dt}=\frac{d(R\omega\cos\vartheta)}{dt}=\\&\qquad=R\omega\frac{d(\cos\vartheta)}{dt}+R\frac{d\omega}{dt}\cos\vartheta=\\
&\qquad=-R\omega\sin\vartheta \underbrace{\frac{d\vartheta}{dt}}_{\omega}+R\frac{d\omega}{dt}\cos\vartheta=\\
&=-R\omega^{2}\sin\vartheta+R\frac{d\omega}{dt}\cos\vartheta
\end{split}
$$
> [!prp] Componenti cartesiane dell'accelerazione nel moto circolare
> $$
> a_x=-R\omega^{2}\cos\vartheta-R\frac{d\omega}{dt}\sin\vartheta
>$$
>$$
>a_{y}= -R\omega^{2}\sin\vartheta+R\frac{d\omega}{dt}\cos\vartheta
> $$

Si ottengono gli stessi risultati ruotando $\vec{a_n}$ e $\vec{a}_{t}$ di $\vartheta$.

# Moto circolare uniforme
In un moto circolare uniforme, il punto materiale percorre una traiettoria circolare con velocità costante in modulo.

Allora, dato che $v$ è costante e da [[#^cc8e3c]], $v=R\omega$, possiamo dire che $\omega=\frac{d\vartheta}{dt}$ è costante.

> [!prp] Modulo della velocità e velocità angolare sono costanti nel moto circolare uniforme
> Come visto in precedenza, possiamo affermare che in un moto circolare uniforme, il modulo della velocità e la velocità angolare sono costanti.
> >[!rmk]
> >La velocità non è costante, dato che la sua direzione cambia lungo la traiettoria circolare

Essendo la velocità angolare costante e $\omega =\frac{d\vartheta}{dt}$, possiamo ricavare come varia l'angolo $\vartheta$ nel tempo.
$$
\vartheta=\vartheta_{0}+\int_{0}^{t}\omega dt
$$
Risolvendo e ricordandoci che $\vartheta_{0}=\vartheta(0)=0$, si ottiene
$$\vartheta(t)=\omega t$$
A questo punto possiamo anche ricavare come varia nel tempo l'[[#Ascissa curvilinea]]
$$
s(t)=R\vartheta(t)=R\omega t
$$

> [!prp] Componenti accelerazione moto circolare uniforme
> Nel moto circolare uniforme, la componente tangenziale dell'accelerazione si annulla 
>$$
>\vec{a}_{t}=0
>$$
>Rimane allora solo la componente centripeta [[#^079892]]
>$$
>\vec{a}=\vec{a_n}=-\omega^{2}\vec{r}
>$$


> [!lemma] 
> Si osserva che il moto circolare uniforme è la composizione di due [[Moto rettilineo#Moto armonico|moti armonici]] monodimensionali lunghi uno $x$ e uno $y$, con periodo
>$$
>T=\frac{2\pi}{\omega}
>$$
>
# Vettore velocità angolare
In un moto circolare, oltre che alla [[#^42f45d|velocità angolare]] $\omega$, si può definire il vettore velocità angolare con:
- modulo pari a $\omega\quad [\frac{rad}{s}]$
- direzione perpendicolare al piano del moto, quindi per la nostra definizione, parallela all'asse $z$
- verso tale da vedere il punto ruotare in senso antiorario.
![[Vettore velocità angolare.png]]

Possiamo calcolare il [[Capitolo 2 - Vettori#Prodotto vettoriale|prodotto vettoriale]] fra $$\vec{\omega}\times\vec{r}$$Dato che $\vec{\omega}$ e $\vec{r}$ sono tra loro perpendicolari, il suo modulo sarà pari a $|\vec{w}||\vec{r}|=\omega R$, la direzione sarà perpendicolare a $\omega$, quindi sul piano $xy$ e perpendicolare a $\vec{r}$, quindi tangente alla circonferenza. La direzione perciò è quella del vettore tangente $\vec{u}_{t}$. 
Il verso è quello tale da formare con $\vec{\omega}$ e $\vec{r}$, una terna destrorsa, quindi proprio il verso di $\vec{u}_t$.
Allora 
> [!prp] Vettore velocità come prodotto vettoriale
>$$
\vec{\omega}\times\vec{r}=\vec{v}
>$$
^1bb765
## Vettore accelerazione con il prodotto vettoriale
Avendo descritto il [[#^1bb765]], possiamo anche calcolare l'accelerazione.
$$
\begin{split}
\vec{a}&=\frac{d\vec{v}}{dt}=\frac{d(\vec{w}\times\vec{r})}{dt} = \frac{d\vec{w}}{dt}\times\vec{r}+\vec{w}\times \underbrace{\frac{d(\vec{r})}{dt}}_{\vec{v}=\vec{w}\times\vec{r}}\\
&=\frac{d\vec{w}}{dt}\times\vec{r}+\vec{w}\times(\vec{w}\times\vec{r})
\end{split}
$$
Analizziamo il termine 
$$
\frac{d\vec{\omega}}{dt}\times\vec{r}
$$
- il modulo di $\frac{d\vec{\omega}}{dt}$ sarà pari a $\left|\frac{d\omega}{dt}\right||\vec{r}|=R\frac{d\omega}{dt}$
- la direzione sarà perpendicolare a $\frac{d\vec{\omega}}{dt}$ e a $\vec{r}$, quindi tangente alla circonferenza.
- Il verso sarà tale da formare una terna destrorsa con $\frac{d\vec{\omega}}{dt}$ e $\vec{r}$.
Allora, guardando i risultati trovati in precedenza troviamo:
> [!prp] Altra rappresentazione del vettore accelerazione tangente
> 
$$\vec{a}_{t}=\frac{d\vec{\omega}}{dt}\times \vec{r}$$

Adesso analizziamo il termine $\vec{w}\times(\vec{w}\times\vec{r})$.
- il modulo sarà pari a $\omega^{2}R$
- la direzione sarà perpendicolare a $\vec{\omega}$ e a $\vec{v}=\vec{\omega}\times{r}$, quindi diretto come $\vec{r}$.
- il verso centripeto.
Allora, troviamo che 
$$
\vec{a}_{n}=\vec{\omega}\times(\vec{\omega}\times\vec{r})
$$
Dalle proprietà del [[Capitolo 2 - Vettori#Prodotto vettoriale|prodotto vettoriale]]: $\vec{a}\times(\vec{b}\times\vec{c}) =(\vec{a}\cdot\vec{c})\vec{b}-(\vec{a}\cdot\vec{b})\vec{c}$, 
$$
\vec{\omega}\times(\vec{\omega}\times \vec{r})=(\vec{\omega}\cdot \vec{r})\vec{\omega}-(\vec{\omega} \cdot \vec{\omega})\vec{r}
$$
Dato che $\vec{\omega}$ e $\vec{r}$ sono perpendicolari, $(\vec{\omega}\cdot \vec{r})=0$, mentre $\vec{\omega}\cdot \vec{\omega}=\omega^{2}$.
Allora
$$
\vec{\omega}\times(\vec{\omega}\times \vec{r})=-(\vec{\omega}\cdot \vec{\omega})\vec{r}=-\omega^{2}\vec{r}=\vec{a}_{n}
$$
# Forze
Quali forze dobbiamo applicare ad un punto materiale per far sì che si muova di moto circolare?
Supponendo che il moto del punto sia noto, vogliamo determinare la [[Forza]] necessaria per realizzarlo.
Abbiamo visto, da [[Accelerazione#^1e403d]], che $\vec{a}=\vec{a}_{n}+\vec{a}_t$ e da [[Capitolo 5 - Dinamica del punto materiale 1#^ee9546]] che $\vec{F}=m \vec{a}$.

Sappiamo inoltre come rappresentare la [[#^079892|componente normale]] e la [[#^9bf2f6|componente tangenziale]].

Sostituendo otteniamo $\vec{F}=m(\vec{a}_{n}+\vec{a}_{t})=\vec{F}_{t}+\vec{F}_{n}$.
$\vec{F}_{n}=-m\cdot \omega^{2}\vec{r}$ e $\vec{F}_{t}=m\cdot R\frac{d\omega}{dt}\vec{u}_t$.



