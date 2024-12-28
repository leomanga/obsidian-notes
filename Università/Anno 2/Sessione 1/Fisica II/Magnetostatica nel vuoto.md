Come per le forze di natura elettrostatica, interpretiamo l’azione che hanno i magneti a distanza come un campo, chiamato **campo magnetico**.
I poli magnetici, ovvero le estremità degli oggetti capaci di attrarre o repellere si manifestano solamente sottoforma di dipoli magnetici.
(Se taglio una barra magnetica con polo nord e polo sud realizzando due barre più piccole, ancora il polo sud e polo nord agli estremi)

Grazie anche all’utilizzo della [pila di volta](https://it.wikipedia.org/wiki/Pila_di_Volta)  si è potuto comprendere che esiste una relazione tra il magnetismo e l’elettricità.
Ad esempio se facciamo scorrere una [[Corrente elettrica]] in un filo ed avviciniamo un ago magnetico, vedremo come si orienterà parallelamente al campo magnetico.

Ipotizziamo che i circuiti percorsi da corrente generino nel loro intorno un [[Campo vettoriale]] $\vec{B}(r)$ che prende il nome di [[Campo di induzione magnetica]].
Consideriamo un filo metallico di sezione costante $S$ e lunghezza $L$, percorso da una [[Corrente stazionaria]] $I$ e posto in una regione dello spazio dove esiste un campo magnetico uniforme di induzione $\vec{B}$.
Le dimensioni di $\vec{B}$ sono $[\frac{N}{C}\frac{m}{s}][T]$ dove $T$ sta per “Tesla”. Un’altra dimensione è quella dei $\left[\frac{W_{b}}{m^{2}}\right]= [V\cdot s]$ dove $W_{b}$ è l’unità di misura del flusso magnetico e sta per “Weber”.

![[Induzione magnetica.excalidraw]]

Si trova sperimentalmente che sul filo conduttore agisce una forza 
$$\vec{F}=I\vec{L}\times \vec{B}$$
dove $\vec{L}$ ha modulo uguale alla lunghezza del filo e direzione e verso councidenti con quelli in cui fluisce la corrente.

>[!def] Seconda formula di Laplace
>Ogni elemento infinitesimo di filo $d\vec{l}(\vec{r})$ percorso dalla corrente $I$ su cui agisce un campo di induzione magnetica $\vec{B}(\vec{r})$ è sottoposto ad una forza 
>$$d\vec{F}(\vec{r})=Id\vec{l}(\vec{r})\times \vec{B}(\vec{r})$$
>

^6d31e9

La forza complessiva che agisce su un tratto di un circuito $I$ percorso da [[Corrente stazionaria]] $I$ è ottenibile integrando la [[#^6d31e9|seconda formula di Laplace]].
$$\vec{F}=\int_{L}Id\vec{l}(\vec{r})\times\vec{B}(\vec{r})$$
Inoltre la quantità $Id\vec{l}$ può essere scritta da [[Densità di corrente elettrica#^cd6c08]] come
$$Id\vec{l}=\vec{J}Sdl=Nq\vec{v}_{d}Sdl$$
dove $N$ indica il numero di portatori di carica per unità di volume, $\vec{v}_{d}$ la loro velocità di deriva e $q$ la carica di ciascuno di essi.
Se chiamiamo $n=NSdl$ il numero di portatori totali contenuti all’interno del tratto $dl$ e sostituiamo alla [[#^6d31e9]]
$$d\vec{F}=nq\vec{v}_{d}\times \vec{B}$$
Allora ci aspettiamo che ogni singola carica puntiforme $q$ che si muove con velocità $\vec{v}$ in un campo di induzione magnetica $\vec{B}(\vec{r})$ subisca una forza $\vec{F}(\vec{r})$ data da
>[!def] Forza di Lorentz
>$$\vec{F}=q\vec{v}\times \vec{B}$$
>Dove $q$ è la [[Carica elettrica]], $\vec{v}$ la sua velocità e $\vec{B}$ il campo di induzione magnetica.
>La forza di Lorentz è ortogonale alla direzione della velocità, quindi non compie alcun lavoro, modifica il moto di una particella che si muove ad una certa velocità ma non varia la sua energia cinetica.

Nel caso in cui in una regione dello spazio agisce oltre al campo di induzione magnetica, anche un [[Campo elettrostatico]], allora una particella è sottoposta alla forza totale
$$\vec{F}(\vec{r})=q(\vec{E}(\vec{r})+\vec{v}\times \vec{B}(\vec{r}))$$
Studiamo ora una spira quadrata.
Abbiamo per ipotesi che la spira sia piana e rigida, la [[Corrente elettrica]] sia [[Corrente stazionaria|stazionaria]] e che il [[Campo di induzione magnetica]] sia uniforme,
$$\vec{B}=B_{x}\hat{x}+B_{z}\hat{z}$$

![[Spira quadrata.excalidraw]]

Possiamo calcolare ora le forze nei vari rami della spira con [[#^6d31e9]].
Allora 
$$\begin{split}&dF_{SP}=Idx\hat{x}\times\vec{B}=Idx\hat{x}\times(B_{x}\hat{x}+B_{z}\hat{z})=-IdxB_{z}\hat{y}\\
&\Rightarrow F_{SP}=\int_{0}^{a}dF_{SP}=-IaB_{z}\hat{y}\end{split}$$
Con lo stesso sistema otteniamo che 
$$F_{QR} = IaB_{z}\hat y$$
Essendo le due forze uguali ed opposte, allora si annullano.
Inoltre possiamo calcolare, sempre nello stesso modo
$$\begin{split}
&\vec{F}_{PQ}=Ia\hat{y}\times(B_{x}\hat x +B_{z}\hat{z})=-IaB_{x}\hat{z}+IaB_{z}\hat x\\
&\vec{F}_{QS}=I(-a\hat{y})\times(B_{x}\hat x +B_{z}\hat{z})=IaB_{x}\hat z-IaB_{z}\hat x
\end{split}$$
Le forze, essendo uguali ed opposte si annullano ma danno vita ad un [[Momento di una forza]].
$$\vec{M}=Ia^{2}|\vec{B}|\sin{\alpha}\hat{y}$$
Se definiamo ora il **momento di dipolo**(**momento magnetico**) come
$$\vec{m} = Ia^{2}\hat{n}\quad [A\cdot m^{2}]$$
dove $\hat{n}$ è la normale della spira che segue il verso antiorario, quindi in questo caso $\hat n = \hat z$.

Allora possiamo scrivere 
$$\vec{M}=\vec{m}\times \vec{B}=Ia^{2}\hat{n}\times \vec{{B}}$$

Enunciamo ora la prima formula di Laplace.
>[!prp] Prima formula di Laplace
>Questa formula è stata trovata sperimentalmente.
>$$d\vec{B}(\vec{r})=k_{m}\frac{Id\vec{l}(\vec{r}^{'})\times(\vec{r}-\vec {r^{'}})}{|\vec{r}-\vec{r^{'}}|^{3}}$$
>Dove $k_{m}=\frac{\mu_{0}}{4\pi}$, $\mu_{0}$ è la [[Permeabilità magnetica nel vuoto]], $I$ la [[Corrente elettrica]], $d\vec{l}$ il percorso fatto in un istante infinitesimo.
>
>

^b6258f

# Casi canonici
## Filo infinito | Legge di Biot-Savart

![[Induzione nel filo.excalidraw]]

Abbiamo che $d\vec{l}(\vec{r}^{'})=dz\vec{z}^{'}$, $\vec{r}^{'}=z^{'}\hat{z}$
$d\vec{l}(\vec{r}^{'})\times (\vec{r}-\vec{r}^{'}) = d\vec{z}^{'}|\vec{r}-\vec{r^{'}}|\sin(\theta)\hat{\phi}$ 
Allora da [[#^b6258f]]
$$d\vec{B}(\vec{r})=k_{m}\frac{Idz^{'}|\vec{r}-\vec{r^{'}}|\sin(\phi)}{|\vec{r}-\vec{r^{'}|^{3}}}$$
Se facciamo il cambio variabili, $\tan\alpha= \frac{\rho}{z^{'}}$ allora
$$z^{'}=\frac{\rho}{\tan \alpha}=-\frac{\rho}{\tan \theta}$$
Allora $$\frac{dz^{'}}{d\theta}=\frac{\rho}{\sin^{2}\theta}\Rightarrow dz^{'}=\frac{\rho}{\sin^{2}\theta}d\theta$$
Inoltre 
$\rho=|\vec{r}-\vec{r}^{'}|\sin\alpha=\rho=|\vec{r}-\vec{r}^{'}|\sin(\pi-\theta)=|\vec{r}-\vec{r}^{'}|\sin(\theta)$
Allora 
$$\vec{B}(\vec{r})=k_{m}I[\int_{0}^{\pi}\frac{\rho}{\sin^{2}\theta}\sin(\theta)\cdot \frac{\sin^{2}\theta}{\rho^{2}}]\hat \phi=\frac{\mu_{0}}{2\pi}\frac{I}{\rho}\hat \phi$$

