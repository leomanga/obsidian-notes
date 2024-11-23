[SLIDES](https://elearning.unisi.it/pluginfile.php/667732/mod_resource/content/1/FISICA%20I%20sez.THERMO-parte01-%20appunti%20LEZIONI%20FINALE.pdf)
--- 
[[Termodinamica]]
[[Sistema termodinamico]]
[[Grandezze estensive]]
[[Grandezze intensive]]
[[Fase]]
[[Volume specifico]]
[[Densità]]
[[Massa]]
[[Pressione]] Fare il barometro, manometro, ecc fino a pag 23.
[[Temperatura]]
[[Gas perfetti]]
[[Scambi di energia]]
[[Principio di conservazione dell'energia]]
[[Variabili di stato]]
[[Variabili di scambio]]
[[Primo principio della termodinamica]]
[[Conduzione termica]]
[[Convezione termica]]
[[Irraggiamemto termico]]
[[Entalpia]]

[[Energia di pulsione]]



Varianza -> numero di grandezze indipendenti in grado di garantire la piena definizione di equilibrio di un sistema.
é definita sul numero di fasi chimiche e fasi fisiche Nc-Nf+2
Se pensiamo al punto triplo dell'qcqua, dove le fasi fisiche sono 3 e le chimiche 1 avremo infatti che tale punto è univocamente determinato, non ha grandezze indipendenti.

Equazione di Clapeyron

x = mvapore / mvapore + mliquido
Rappresentea il parametro che definisce il rapporto fra la quantità di massa di vapore saturo e quella fra il liquido saturo in equilibrio bifasico. Si chiama titolo della miscela liquido vapore.
Se è 0 la sostanza è in condizioni di liquido saturo, se è 1, la sostanza si trova in condizioni di vapore saturo.

Possiamo trovare ad esempio il volume del liquido durante il cambiamento di fase.
Pag 11 formula

Il secondo principio della termodinamica definisce quali siano le trasformazioni possibili in condizioni reali. Definisce il "verso" delle trasformazioni. Un corpo che si muove con attrito perde energia cinetica trasferendola tramite calore con la superficie ec...

Le trasformazioni termodinamiche possono essere irreversibili, non possono quindi manifestarsi nella direzione inversa riportando il sistema e l'ambiente alle condizioni originarie.

Abbiamo definito la sorgente termica e la macchina termica a pag 32.

Viene introdotto il concetto di rendimento $\eta$ o efficienza termica a pag 35. Sarebbe il rapporto fra il lavoro scambiato rispetto all'energia termica scambiata con la sorgente a temperatura superiore.
Se non cedo calore, il rendimento sarà 1, se ne cedo tutto quello che entra, il rendimento sarà 0.

Dal secondo principio della termodinamica di Kelvin-Planck possiamo dire con certezza che le macchine reali hanno sempre un rendimento inferiore ad 1.

La macchina invece che rispetta questa cosa si chiama macchina perfetta.

A pagina 49 facciamo il ciclo inverso, ovvero scambiamo calore da una sorgente fredda ad una più calda, questo è possibile solo se viene fatto del lavoro sul sistema (quindi se tutto è al contrario fondamentalmente).
Il ciclo inverso viene chiamato anche pompa di calore o ciclo frigorifero.
Comunque in questo sistema l'energia interna iniziale è uguale a quella finale.

Ad esempio in un frigorifero, il lavoro sarà il consumo elettrico (che è giustamente negativo) e il calore scambiato alla sorgente calda (l'aria) avverrà tramite la serpentina dietro.

Anche qui si può parlare di pompa di calore o macchina frigorifera perfetta, ovvero quando l'effetto utile di energia termica avviene con assenza di lavoro. Come nel caso della macchina perfetta, ciò è irrealizzabile, dal secondo principio della termodinamica di Clausius.

L'efficienza di una forma di calore viene descritta in termini di uno scalare detto COP(Coefficiente di Prestazione).

Il coefficiente di prestazione assume valori diversi a seconda che il ciclo abbia lo scopo di raffreddare(frigorifero), oppure di riscaldare.
Avremo $\beta=COP_{raffr}=\frac{Q_{c}}{W}$
Avremo $\delta=COP_{risc}=\frac{Q_{h}}{W}$

A pagina 54 definiamo un processo reversibile, ovvero:
quello che subisce un sistema che, passando attraverso successivi stati di equilibrio, può essere ricondotto allo stato iniziale lungo lo stesso percorso della linea di trasformazione che rappresenta i punti di equilibrio.

Se queste condizioni non sono soddisfatte, si dice che la trasformazione è irreversibile.

Tutte le trasformazioni naturali/reali sono irreversibili, anche se alcuni processi possono essere considerati quasi reversibili, principalmente quelli per i quali le trasformazioni sono molto lente.

Tutto questo è dovuto dai vari effetti dissipativi interi od esterni al sistema:
1) dissipazioni a seguito dell'attrito meccanico o fluidodinamico
2) scambio termico
3) trasformazioni chimiche


Teorema di Carnot afferma che tutte le macchine operanti in maniera ciclica interagendo con le due sorgenti assegnate, il massimo rendimento compete a quella che opera in maniera internamente ed esternamente reversibile, dato che per tale macchina le dissipazioni saranno assenti.
Un ciclo sarà quindi reversibile se non presenta irreversibilità interne e se lo scambio di calore tra il sistema e l'ambiente avviene in condizioni reversibili.
A pag 59 la dimostrazione.

Rendimento di Carnot: $1-\frac{T_{c}}{T_{h}}$ 
Il rendimento di Carnot è quello massimo un dato sistema.
Il rendimento ideale tende ad 1 solo se la temperatura superiore tende ad infinito e quella inferiore a 0.

In un ciclo di Carnot vale
$$\frac{Q_{h}}{Q_{c}}=\frac{T_{h}}{T_{c}}$$

Avremo invece il COP max se $t_{h}=t_{c}$

A pag 73 abbiamo fatto l'entropia $S$, che, come l'energia interna, entalpia e la temperatura, è una funzione di stato.
Si può concettualizzare come la misura della dispersione dell'energia.
$$dS=\frac{dQ_{rev}}{T}$$
$(dQ)_{rev}$ rappresenta il calore trasmesso in processi reversibili, mentre $T$ è la temperatura assoluta del sistema.

L'entropia lungo un ciclo reversibile è costante(Guarda pag 75), quindi
$$\Delta S=\frac{|Q_{h}|}{T_{h}}-\frac{|Q_{c}|}{T_{c}}=0$$

Indichiamo con $\sigma$ l'effetto che abbiamo all'interno di un sistema, rappresenta l'entropia prodotta per effetto delle irreversibilità interne al sistema, avendo rappresentato nulla le irreversibilità esterne dovute allo scambio termico.
In caso di una trasformazione ciclica reversibile, $\sigma =0$, mentre in una trasformazione irreversibile, $\sigma > 0$ dati che $\oint \frac{dQ}{T}=-\sigma\le 0$ 

A pag 82 ci sono le equazioni TdS, che esprimono il rapporto tra entropia ed energia interna o entalpia.

Equazzione del Bilancio per sistemi chiusi

$$S_{2}-S_{1}=\int_{1}^{2}\frac{dQ}{T}+\sigma$$
Entropia nei sistemi aperti?
$$\frac{dS}{dt}=\sum_{j}\frac{\dot{Q}}{T}+\dot m_{i}\cdot s_{i}-\dot m_{u}\cdot s_{u}+\dot \sigma$$
$\sum_{j}\frac{\dot{Q}}{T}$ sono i contributi associati a trasferimenti di energia termica nell'unità di tempo.
$\dot m_{i}\cdot s_{i}-\dot m_{u}\cdot s_{u}$ è il contributo dovuto a flussi di massa entranti ed uscenti dal volume di controllo
$\dot \sigma$ generazione di entropia nell'unità di tempo.

Per i sistemi aperti in regime stazionario avremo che i flussi di massa entranti sono uguali a quelli uscenti e le energie trasferite al sistema sono pari a 0.

La differenza fra le entropie entranti e le entropie uscenti è sempre non nulla.

Avremo quindi
$$s_{2}-s_{1}=\frac{1}{\dot m}\left(\sum_{j}\frac{\dot Q_{j}}{T_{j}}\right)+\frac{\dot\sigma}{\dot m}$$

Viene introdotto a pag 97 il concetto di rendimento isoentropico in espansione o compressione come il rapporto fra le prestazioni reali e le prestazioni raggiunte da un processo ideale(isoentropico) avente condizioni di pressione iniziali e finali uguali al processo reale.
$$\eta_{is}=\frac{(\frac{\dot W_{1-2}}{\dot m})_{r}}{(\frac{\dot W_{1-2}}{\dot m})_{s}}=\frac{h_{2,r}-h_{1}}{h_{2,s}-h_{1}}$$
A pag 100 si vede che il calore è l'area del grafico di una funzione dell'entropia in base alla temperatura.

$$\Delta s = c_{p}\ln(\frac{T_{2}}{T_{1}})- R\ln(\frac{p_{2}}{p_{1}})$$