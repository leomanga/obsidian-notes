Se seguiamo il modello classico dell’atomo, abbiamo che gli elettroni di carica $-e$ si muovono di velocità costante $v$ attorno al nucleo. Ciò equivale ad una spira di corrente $i_{a}=\frac{-e}{T}=\frac{-ev}{2\pi r}$ (es. idrogeno $I_{a}\simeq 1 mA$).
Alla spira associamo un momento magnetico orbitale $\vec{m}_{0}$ di modulo $m_{0}=I_{a}\pi r^{2}=- \frac{1}{2}evr$ (es. idrogeno $m_{0}\simeq 9.35\cdot 10^{-24} Am^{2}$).

Avendo l’elettrone una massa $\vec{m}_{e}$, al moto possiamo associare un momento meccanico angolare $L_{e}=m_{e}vr$ orientato nel verso opposto a $\vec{m}_{0}$

Possiamo ora legare il momento magnetico e quello meccanico con la relazione
$$\vec{m}_{0}=-(\frac{e}{2m_{e}})\vec{L}_{e}$$

Si può anche associare all’elettrone un momento magnetico intrinseco $\vec{m}_{e}^{s}$ associato allo spin. (L’elettrone non gira fisicamente su se stesso, è un fenomeno relativistico).
In meccanica quantistica il modulo del momento magnetico di spin vale $m_{e}^{s}=-\frac{eh}{2m_{e}}$

Nella maggior parte degli atomi, la somma dei momenti magnetici, orbitali e di spin è nulla e non esiste un momento di dipolo magnetico atomico.
In alcuni atomi, però, non si ha la totale compensazione dei momenti, quindi è possibile che un atomo possegga un momento di **dipolo magnetico atomico** $\vec{m}$ diverso da 0.
Possiamo allora immaginare ogni atomo di un materiale con $\vec{m}\not =0$ come una piccola spira di corrente.

Essendo però l’orientamento del momento dei vari atomi casuale, allora il momento magnetico risultante del materiale risulterà nullo. Di conseguenza non avrà effetti magnetici.

# Paramagnetismo
Nel caso dei materiali con atomi dotati di momento di dipolo atomico, se applichiamo dall’esterno un [[Campo di induzione magnetica]], allora le spire elementari tenderanno a disporsi perpendicolarmente al campo, dando origine ad un momento magnetico parallelo e concorde al campo di induzione esterno.

![[Pasted image 20241230120734.png]]

# Diamagnetismo
Nel caso dei materiali con atomi dotati di un momento magnetico atomico nullo, se applichiamo un [[Campo di induzione magnetica]], il moto degli elettroni viene perturbato e si genera un momento magnetico che tende ad opporsi al campo esterno. Ciò è dovuto al fatto che gli elettroni sono sottoposti alla forza magnetica $q\vec{v}\times \vec{B}_{ext}$, ciò fa aumentare la velocità orbitale dell’elettrone se ha momento antiparallelo al campo, mentre la fa ridurre se ha momento parallelo al campo.
A questo punto i momenti magnetici non si compensano più e la sostanza acquista un momento magnetico opposto a quello del campo applicato.
Questo meccanismo è sempre presente, anche se il momento magnetico generato è piccolissimo.

![[Pasted image 20241230123900.png]]

# Ferromagnetismo
Un piccolo numero di sostanze cristalline (ferro, cobalto, nichel, …) mostra fenomeni magnetici marcati.
Tutti i materiali ferromagnetici contengono regioni microscopiche, dette **domini di Weiss**($10^{-18}:10^{-12} m^{3}$), all’interno dei quali i momenti magnetici sono tutti allineati (dovuto all’interazione quantistica degli spin).

In un materiale non magnetizzato, i momenti magnetici dei domini sono orientati in modo casuale ed il momento magnetico risultante è in media nullo.

Se il materiale viene posto in un campo di induzione magnetica esterno, le dimensioni dei domini aventi momenti magnetici allineati con il campo applicato crescono e la sostanza si magnetizza.

Rimuovendo l’induzione esterna applicata, il materiale conserva una magnetizzazione nella direzione della induzione applicata. (Solo ad alte temperature si può distruggere questa orientazione preferenziale).

![[Pasted image 20241230124649.png]]

# Vettore magnetizzazione
Dalle considerazioni fatte, un materiale magnetizzato può essere considerato come un insieme di atomi o molecole dotati di momento magnetico complessivo non nullo.
Se considero un punto $(x,y,z)$ e di un volumetto $\Delta V$ che contiene un numero significativo $\Delta N$ di dipoli magnetici $\vec{m}_{i}$
Allora si definisce il **vettore di magnetizzazione** $\vec{M}(x,y,z)$ come
$$\vec{M}(x,y,z)=\frac{\sum_{i=1}^{\Delta N}\vec{m}_{i}}{\Delta V}\quad \frac{A}{m}$$
e rappresenta per ugni punto, un momento di dipolo magnetico per unità di volume.
# Correnti di magnetizzazione
Se prendiamo in esame un materiale di forma cilindrica, magnetizzato lungo l’asse del cilindro stesso ($\vec{M}$ sarà parallelo all’asse del cilindro), se l’intensità di magnetizzazione è uniforme in tutto il materiale, allora il numero di spire per unità di volume sarà costante, quindi le correnti atomiche interne al cilindro si annulleranno l’una con l’altra.

Sulla superficie però, $\vec{M}$ subirà una discontinuità, passando bruscamente dal valore che assume internamente, al valore zero che ha esternamente.
Non essendoci sulla superficie compensazioni di correnti atomiche, verrà generata una [[Densità di corrente elettrica]] superficiale $\vec{J}_{ms}$.

Questa corrente superficiale è in grado di produrre un campo di induzione magnetica $\vec{B}_{m}$ che si somma vettorialmente a quello applicato $\vec{B}_{0}$, sia dentro che fuori il materiale.

![[Pasted image 20241230154400.png]]

Se l’intensità di magnetizzazione non è uniforme, allora le correnti interne non si annullano. Esisterà quindi anche una [[Densità di corrente elettrica]] volumetrica $\vec{J}_{m}$ che fluisce all’interno del materiale.

Si dimostra che, per un punto generico del materiale magnetizzato,
$$
\vec{J_{m}}=\nabla\times \vec{M}(\vec{r})\quad [\frac{A}{m^{2}}]
$$

^c2674c

$$
\vec{J}_{ms}=\vec{M}(\vec{r})\times \hat{n}\quad [\frac{A}{m}]\mbox{ con }\hat n\mbox{ la normale alla superficie}
$$

^bc8454

# Legge di circuitazione di Ampere nei materiali magnetizzati
Nel vuoto abbiamo che ![[Campo di induzione magnetica#^acacd5]]
Nel caso in cui il campo di induzione magnetica $\vec{B}(\vec{r})$ sia generato, oltre che da correnti, anche dalle correnti di magnetizzazione presenti nei materiali magnetizzati, scriveremo
$$
\nabla\times \vec{B}(\vec{r}) = \mu_{0}[\vec{J}(\vec{r})+\vec{J}_m (\vec{r})]
$$
Dato che, da [[Magnetostatica nei mezzi materiali#^c2674c]] $\vec{J_{m}}=\nabla\times \vec{M}(\vec{r})$, si può scrivere $$\nabla \times[\frac{\vec{B}(\vec{r})}{\mu_{0}}-\vec{M}(\vec{r})]=\vec{J}(\vec{r})$$
Si definisce ora il [[Vettore campo magnetico]] $\vec{H}(\vec{r})=\frac{\vec{B}(r )}{\mu_{0}}-\vec{M}(\vec{r})$

La forma differenziale della legge di circuitazione di Ampere diventa quindi 
$$\nabla \times \vec{H}(\vec{r})=\vec{J}(\vec{r})$$
Nel vuoto, dove $\vec{M}=0$ si avrà $$\vec{B}(\vec{r})=\mu_{0}\vec{H}(\vec{r})$$
>[!prp]
>Applicando il teorema di Stokes
>$$\iint_S\nabla\times \vec{H}(\vec{r})\hat n ds = \iint_{S}\vec{J}(\vec{r})\hat n\hat ds=\oint_{C}\vec{H}(\vec{r})d\vec{l}=I$$
>Dove $\vec{H}$ è il [[Vettore campo magnetico]], $\vec{J}$ è la [[Densità di corrente elettrica]] e $I$ è la [[Corrente elettrica]].

# Suscettività e permeabilità magnetica
Per i materiali omogenei, lineari e isotropi si ha 
$$\vec{M}(\vec{r})=\chi_{m}\vec{H}(\vec{r})$$
dove $\chi_{m}$ è detta suscettività magnetica.

Avremo allora il legame
$$\vec{B}(\vec{r})=\mu_{0}[\vec{H}(\vec{r})+\vec{M}(\vec{r})]=\mu_{0}[\vec{H}(\vec{r})+\chi_{m}\vec{H}(\vec{r})]=\mu_{0}(1+\chi_{m})\vec{H}(\vec{r})=\mu_{0}\mu_{r}\vec{H}(\vec{r})$$
dove $\mu_{r}=1+\chi_{m}$ e prende il nome di **permeabilità magnetica relativa**.
#da-finire(pag 17 slides magnetostatica)

