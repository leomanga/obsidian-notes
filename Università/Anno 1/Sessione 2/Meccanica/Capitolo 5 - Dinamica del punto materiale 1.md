> [!def] Dinamica
> Studio di come il moto di un sistema è influenzato dalle interazioni con l'ambiente circostante.
# Introduzione
Per lo studio della dinamica dobbiamo definire nuove grandezze.
- [[Forza]]
- [[Massa]]
# Tre leggi (o principi) della dinamica
Le tre leggi della dinamica sono alla base della meccanica classica e sono state presentate da Newton.

> [!axiom|1] Principio di inerzia
> Un corpo non soggetto a forze non subisce variazioni di velocità, quindi:
> Se era inizialmente in quiete ($\vec{v}(0)=0$)$\Rightarrow \vec{v}(t)=0\ \forall t$
> Se invece aveva velocità ($\vec{v}(0)=\vec{v}_{0}\not =0$)$\Rightarrow \vec{v}(t)=\vec{v}_{0}$
> 

^538083

> [!axm|2] Secondo principio della dinaminca
> %%display : Seconda legge di Newton%%
> 
> Un punto materiale sottoposto a una o più forze si muoverà con un'accelerazione vettorialmente proporzionale alla risultante di tali forzeù
> 
> $$\vec{F}=m\vec{a}\qquad \left[\frac{1kg\cdot m}{s^{2}}\right]=[N]$$
> $\vec{F}$ è la [[Capitolo 2 - Vettori#Definizione risultante|risultante]] delle forze applicate al corpo.
> $m$ è la [[Massa]] inerziale, una proprietà del punto materiale che descrive la sua resistenza a variare il proprio stato di moto, ossia a modificare la propria velocità.
> $\vec{a}$ è l'accelerazione del punto materiale.
> ---
> 
> Collegamenti : [[#^108ea4]]
> 
> ---
^ee9546

> [!axm|3] Principio di azione e reazione
> Se un corpo $A$ esercita una forza $\vec{F}_{A,B}$ sul corpo $B$, il corpo $B$ a sua volta eserciterà sul corpo $A$ una forza $\vec{F}_{B,A}$ tale che 
> $$
> \vec{F_{B,A}} =-\vec{F}_{A,B}$$

^d51cf7

> [!exercise] Problema dinamico diretto
>Note le forze applicate ad un punto materiale, si vuole determinare il suo moto.
>Applicando [[#^ee9546]], e ricordando che l' [[Accelerazione#Accelerazione in 2 dimensioni#Accelerazione istantanea|accelerazione]] è definita come 
>$$
\vec{a}=m\frac{d^{2}\vec{r}}{dt^{2}}$$
>Il problema allora si riduce a risolvere un'equazione differenziale
>$$
\vec{F}=m\frac{d^{2}\vec{r}}{dt^{2}}$$

> [!exercise] Problema dinamico inverso
> Il moto del punto materiale è noto, si vogliono determinare le forze che vi sono applicate.
>In questo caso conosciamo $\vec{r}$ e possiamo determinare  $\vec{a}=m\frac{d^{2}\vec{r}}{dt^{2}}$.
>Dobbiamo allora risolvere un sistema di equazioni di tipo algebrico
$$\vec{F}=m \vec{a}$$

> [!def] Quantità di moto
> La quantità di moto di un punto materiale è definita come il prodotto tra la sua [[Massa]] e la sua [[Velocità]].
> $$
> \vec{p}=m \vec{v}\quad [kg\cdot\frac{m}{s}]$$
> >La quantità di moto è un vettore che ha:
>>- la stessa direzione di $\vec{v}$
>>- lo stesso verso della velocità $\vec{v}$ (dato che la massa è positiva)
>>- modulo $m|\vec{v}|$ che dimensionalmente sarà una massa per una velocità
>
>> Quantifica la [[Forza]] necessaria a fermare un oggetto in un'unità di tempo.

^63bffd

>[!Axiom] Riformulazione della seconda legge di Newton
>[[#^ee9546|La seconda legge di Newton]] può essere formulata in questo modo:
>$$\vec{F}=\frac{d \vec{p}}{dt}$$
>dove $\vec{p}$ è la [[#^63bffd]].
>Quindi la risultante delle forze applicate a un punto materiale è pari alla variazione della quantità di moto rispetto al tempo.
>
>Rappresenta la situazione di un punto materiale in un certo istante.
>
>**Questa formulazione vale in generale anche per corpi a massa variabile, cosa non vera per la prima formulazione.**
>Si può prendere come esempio un sistema a carburante, che man mano che passa il tempo riduce la sua massa dato che brucia.


^108ea4

![[Impulso di una forza]]

# Applicazioni
Se su un corpo agiscono più forze, la risultante sarà data dalla somma vettoriale.
## Calcolo accelerazione
Ipotizziamo che su un corpo vengano applicate più forze e vogliamo calcolare l'accelerazione, allora, ipotizzando che il corpo abbia massa costante possiamo usare il [[#^ee9546]].
Allora $\vec{a}=\frac{1}{m}\vec{R}$
## Applicazione del teorema dell'impulso
Consideriamo un punto materiale P di massa $m$ che si muove contro un muro a velocità costante $\vec{v}$.
Dopo aver urtato il muro, rimbalza e ripercorre la traiettoria a velocità $-\vec{v}$.
Possiamo calcolare la variazione della quantità di moto durante l'urto. Supponendo che l'urto abbia una durata $\Delta t$, calcoliamo il valore medio della forza con cui il punto colpisce la superficie.
La quantità di moto iniziale sarà $\vec{p}_{0}=m\vec{v}$ e quella finale $\vec{p}_{1}=-m\vec{v}$. Allora $\Delta \vec{p}=\vec{p}_{1}-\vec{p}_{0}= -2m \vec{v}$.

Possiamo inoltre calcolare la [[Forza]] che la superficie esercita sul punto materiale durante l'urto.
Sapendo che $\Delta{\vec{p}}=-2mv\vec{i}$, dal [[Impulso di una forza#^501fb3]] risulta che $\vec{J}=-2mv\vec{i}$.
Allora, per [[Impulso di una forza#^ad2537]], $\vec{J}=\int_{0}^{\Delta t}\vec{F}dt=-2mv\vec{i}$
Allora possiamo valutare il valore medio della forza nel tempo $\Delta t$ come $$\vec{F}_{m}=\frac{1}{\Delta t}\int_{0}^{\Delta t}\vec{F}dt=\frac{1}{\Delta t}\vec{J}=-\frac{2mv}{\Delta t}\vec{i}$$
Allora, per il [[#^d51cf7]], eserciterà una forza di $-\vec{F}_{m}$.

# Moto circolare
![[Moto circolare#Forze]]

# Forza peso
$\vec{F}=m\vec{g}$

# Piano inclinato
La forza che esercita una superficie su un corpo è perpendicolare alla superficie stessa.
Allora la risultante $\vec{R}=\vec{F}_{p}+\vec{N}=m\vec{a}$
dove $\vec{F}_{p}$ è la forza peso e $\vec{N}$ è la forza normale alla superficie.
$\vec{a}$ avrà direzione parallela alla superficie e quindi anche $\vec{R}$ sarà parallela alla superficie.

$$R=mg\sin\alpha$$
dove $\alpha$ è l'angolo fra $F_{p}$ e $N$.

# Corpo sospeso da un filo
Analizziamo un corpo sospeso al soffitto con un filo in condizioni statiche. Il corpo è soggetto alla propria forza peso, e, dato che non cade, il filo deve esercitare sul corpo una forza $T=-\vec{F}_p$.
Inoltre il filo, essendo attaccato al soffitto, esercita una forza di $-T$, quindi il soffitto eserciterà una forza pari a $T$.

Inoltre, in condizioni dinamiche, il corpo sospeso può avere accelerazione diversa da zero e risulta
$$\vec{F}_{p}+\vec{T}=m\vec{a}$$
Dato che il filo può essere solo teso, la direzione della forza $T$ sarà la stessa del filo.

# Attrito
Consideriamo un punto materiale appoggiato su una superficie piana non liscia. Se applichiamo una forza orizzontale $\vec{F}_{t}$, il corpo comunque non si muoverà.
Allora $\vec{F}_{t}+\vec{F}_{p}+\vec{S}=0$, dove $\vec{S}$ è la forza di attrito.

Se il modulo di $\vec{F}_{t}$ aumenta oltre un certo limita, il punto materiale inizierà a muoversi, questo limite, secondo il modello di attrito proposto da Culomb è $\mu_{s}N$.
![[Attrito 1.png]]
$\mu_{s}$ prende il nome di coefficiente di attrito statico e dipende dalle caratteristiche delle superfici.
$$
A\le\mu_{s}N\Rightarrow\frac{A}{N}=\tan\varphi\le\mu_{s}
$$

^439577


FARE MEGLIO

Osservando che la componente normale è $N=mg\cos\alpha$ e $A=\mu_{d} N=\mu_{d}mg\cos\alpha$
$R=mg\sin\alpha-\mu_{d}mg\cos\alpha$ (mettere foto per capire meglio)

# Piano inclinato
![[Piano inclinato]]







