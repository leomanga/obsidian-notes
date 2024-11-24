Finora abbiamo studiato la dinamica di un solo [[Punto materiale]], ma adesso consideriamo un sistema costruito da $n\ge 1$ punti materiali.

Indichiamo con $$P_{i}\mbox{ il generico punto materiale}\qquad i\in 1,\ldots,n$$
Sul piano inoltre agiranno delle forze
Indicheremo con
$$\vec{F}_{i}=m\vec{a}_{i}\mbox{ la risultante delle forze applicate sul punto i-esimo}$$

Possiamo inoltre suddividere le forze agenti su $P_{i}$ in due gruppi:
- Forze dovute all'interazione con l'ambiente esterno (FORZE ESTERNE) $F_{i}^{(E)}$
- Forze dovute all'interazione con altri punti (FORZE INTERNE) ($F_{i}^{I}$), dove $\vec{F}_{ji}$ è la forza che il punto $j$ esercita sul punto $i$.
  Dal [[Capitolo 5 - Dinamica del punto materiale 1#^d51cf7|terzo principio della dinamica]], $\vec{F}_{ji}=-\vec{F}_{ij}$
  Le forze interne inoltre non per forza sono tutte conservative, può capitare che all'aumentare dei punti le forze interne aumentino dato l'aumento delle interazioni.
  Inoltre la risultante delle forze interne in un punto non per forza è nulla, sarà però nulla la risultante di tutte le forze del sistema.

>[!def] Centro di massa
>Dato un sistema costituito da $n$ punti materiali $P_{i}$ di massa $m_{i}$ e coordinate $x_{i},y_{i}, z_{i}$, rispetto  ad un sistema di riferimento cartesiano di origine $O$ e assi $x,y,z$, si definisce il ==centro di massa==($CM$) degli $n$ punti materiali, la cui posizione è identificata rispetto all'origine dal vettore $\vec{r}_{CM}$ tale che
>$$\vec{r}_{CM}=\frac{\sum_{i=1}^{n}m_{i}\vec{r_{i}}}{\sum_{i=1}^{n}m_{i}}$$
>Il centro di massa è una proprietà del sistema e non del sistema di riferimento scelto. Si verifica a pag 23.

^a2fd88

>[!def] Velocità del centro di massa
>Derivando in base al tempo il [[#^a2fd88|centro di massa]], otterremo 
>$$\vec{v}_{CM}=\frac{\sum_{i=1}^{n}m_{i}\vec{v}_{i}}{m}$$
>Ricordiamo che la [[Capitolo 5 - Dinamica del punto materiale 1#^63bffd|quantità di moto]] è definita come $\vec{p}_{i}=m_{i}\vec{v_{i}}$.
>La quantità di moto totale $P$ del sistema sarà pari a$$\vec{P}=\sum_{i=1}^{n}\vec{p}_{i}$$
>Potremo allora scrivere che 
>$$\vec{v}_{CM}=\frac{\vec{P}}{m}$$
>

^9ec079

>[!def] Accelerazione del punto di massa
>Basta derivare la [[#^9ec079|velocità del centro di massa]]
>Otteniamo allora $$\vec{a}_{CM}=\frac{\sum_{i=1}^{n}m_{i}\vec{a}_{i}}{m}$$

^93b374

Guarda slides 32,33,34

Dato che la somma delle forze interne in un sistema è pari a zero, allora $m\vec{a}_{CM}$ rappresenterà la somma delle esterne applicate al sistema e chiameremo $\vec{R}^{(E)}$ la risultante. ù
$$m \vec{a}_{CM}=\frac{d\vec{P}}{dt}=\vec{R}^{(E)}$$
Deduciamo quindi che se $\vec{R}^{(E)}=0$, allora $\vec{P}$ è costante.

>[!def] Sistema isolato
>Un sistema si dice isolato quando $$\vec{R}^{(E)}=0$$
>Avremo allora che $\vec{a}_{CM}=0$, $\vec{v}_{CM}=0$ e $\vec{P}$ costante.
>In un sistema di punti materiali isolati quindi si conserva la quantità di moto totale. (Non è detto che si conservi quella dei singoli punti).
>

>[!def] Momento della quantità di moto
>$$\vec{L}=\sum_{i=1}^{n}\vec{L}_{i}=\sum_{i=1}^{n}\vec{r}_{i}\times m_{i}\vec{v}_{i}$$
>---
>
>[[Momento angolare della quantità di moto]]

^3b51e4


>[!thm] Teorema del momento angolare
>$$\frac{d \vec{L}}{dt}=-\vec{v}_{O}\times m \vec{v}_{CM}+\vec{M}^{(E)}$$
>$\vec{v}_{O}\times m \vec{v}_{CM}$ si annulla se:
>- Il polo per il calcolo dei momenti è fisso ($\vec{v}_{0} = 0$)
>- Il polo concide con il centro di massa, quindi $\vec{v}_{CM}\times m\vec{v}_{CM}=0$
>- $\vec{v}_{0}$ e $\vec{v}_{CM}$ sono paralleli
>  
>  Avremo che se i termini sono nulli, allora $\vec{L}$ è costante
>  
>---
>$\vec{M}^{E}$ è il momento delle forze esterne. [[Momento di una forza]]
>

^a907c0

Possiamo calcolare il lavoro delle forze applicate sui punti del sistema per uno spostamento infinitesimo.

Per un punto $i-$esimo risulta
$$dW_{i}=\vec{F}_{i}\cdot d\vec{r}_{i}$$
Chiaramente il lavoro può essere diviso fra le forze interne ed esterne.
$$dW_{ij}^{(I)}=\vec{F}_{ij}\cdot d\vec{r}_{ij}$$
dove $d\vec{r}_{ij}=d\vec{r}_{j}-d \vec{r}_{i}$ è lo spostamento relativo tra i punti $i$ e $j$.
(Guarda a pag 53, ci sarebbe altro da dire).

Dato che in generale può essere che $d\vec{r}_{ij}\not = 0$, di conseguenza il lavoro sarà diverso da zero. Il lavoro dipende infatti da quanto i punti si spostano uno rispetto all'altro.

Il [[Lavoro]] totale inoltre sarà la differenza di [[Energia cinetica]] fra un istante iniziale ed uno finale dei punti del sistema.

>[!thm] Teorema dell'energia cinetica per i sistemi di punti materiali
>$$W_{AB}^{(E)}+W_{AB}^{(I)}=E_{kB}-E_{kA}$$

Se le forze sono conservative avremo inoltre che 
$$W_{AB}^{(I)}=-\Delta E_{p}^{(I)}=-(E_{P,B}^{(I)}-E_{P,A}^{(I)})$$
Stessa cosa per il lavoro dalle forze esterne.

>[!def] Energia potenziale della forza peso di un sistema di punti
>$$E_{p}=mgz_{CM}$$
>Dove $z_{CM}$ è la componente nelle $z$ del [[#^a2fd88]].
>Guarda pag 60 per capire come ci si arriva


Abbiamo visto che possiamo calcolare l'energia potenziale ($E_{p}$) e la quantità di moto ($\vec{P}$) tenendo di conto solo il centro di massa.

Non possiamo fare però ciò con l'energia cinetica ($E_{k}$) e il momento angolare $\vec{L}$.
Spiegazione a pag 62, si usano i [[Capitolo 7 - Cinematica dei moti relativi|moti relativi]]. 

>[!thm] Secondo teorema di Koning
>$$E_{k}=\sum_{i=1}^{n} \frac{1}{2}m_{i}\vec{v}_{i}^{2}= \frac{1}{2}m \vec{v}_{CM}^{2}+\sum_{i=1}^{n} \frac{1}{2}m_{i}v^{'2}_{i}$$
>Più brevemente 
>$$E_{k}=E_{kCM}+E^{'}_{k}$$
>$\vec{v}^{'}$ è la velocità del punto rispetto al centro di massa.

^074e87

# Urti
![[Urti]]

