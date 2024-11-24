Analizziamo un sistema costituito da due punti materiali che durante il loto moto urtano tra loro.
Analizziamo in particolare quello che succede durante l'urto stesso.

Durante l'urto possiamo assumere che i punti non si muovono uno rispetto all'altro.
Nel contatto si sviluppano forze molto elevate che agiscono in un tempo molto breve.

Faremo uso del concetto di [[Impulso di una forza]].

La quantità di moto del sistema prima dell'urto è:
$$\vec{P}_{in}=m_{1}\vec{v}_{1,in}+m_{2}\vec{v}_{2,in}$$
La quantità di moto dopo l'urto è
$$\vec{P}_{fin}=m_{1}\vec{v}_{1,fin}+m_{2}\vec{v}_{2,fin}$$
![[Urti.png]]

Le forze che si sviluppano durante l'urto sono interne e sono di tipo impulsivo.
Si dice che una [[Forza]] è impulsiva quando agisce in un tempo limitato con un modulo elevato.
Le altre forze esterne in genere sono non impulsive e quindi se consideriamo un tempo molto piccolo, il loro impulso è molto piccolo.

Da queste considerazioni possiamo assumere che la [[Capitolo 5 - Dinamica del punto materiale 1#^63bffd|quantità di moto]] si conserva, allora
$$\vec{P}_{in}=\vec{P}_{fin}$$
Possiamo quindi giungere alla conclusione che (vedi pag 68) che
$$
\vec{v}_{CM,in}=\vec{v}_{CM,fin}
$$

^78f490

dove $\vec{v}_{CM}$ è la [[Capitolo 8 - Sistemi di punti materiali#^9ec079|velocità del centro di massa]].

Possiamo quindi concludere che in un urto, la quantità di moto e la velocità del centro di massa rimane costante, variano però nei singoli punti.
$$\Delta \vec{p}_{1}= -\Delta \vec{p}_{2}\Rightarrow \vec{J}_{21}=-\vec{J}_{12}$$

Dopo aver visto che si conserva la quantità di moto $\vec{P}$, vogliamo capire cosa succede al [[Capitolo 5 - Dinamica del punto materiale 2#^daccc8|momento angolare]] $\vec{L}$.
$$\vec{L}_{1}=\vec{r}_{1}\times m_{1}\vec{v}_{1}$$
$$\vec{L}_{2}=\vec{r}_{2}\times m_{2}\vec{v}_{2}$$
Il momento angolare totale vale allora
$$\vec{L} = \vec{L}_{1}+\vec{L}_{2}=\vec{r}_{1}\times m_{1}\vec{v}_{1}+\vec{r}_{2}\times m_{2}\vec{v}_{2}$$
Dato che in prossimità dell'urto $\vec{r}_{1}\approx \vec{r}_{2}=\vec{r}$, risulta
$$\vec{L}=\vec{r}\times (m_{1}\vec{v}_{1}+ m_{2}\vec{v}_{2})=\vec{r}\times \vec{P}$$
Dato che $\vec{r}$ è circa costante al momento dell'urto e $\vec{P}$ si conserva, allora anche $\vec{L}$ si conserva.

Ora vogliamo vedere cosa succede all'energia cinetica.
Ci possiamo trovare però in due casi, uno in cui le forze si conservano ed uno in cui non si conservano.

>[!def] Urto perfettamente elastico
>Quando le forze interne sono conservative si parla di urto perfettamente elastico.
>$$W_{urto}^{(I)}=\Delta E_{k}=-\Delta E_{p}$$

>[!def] Urto anelastico
>Quando le forze interne non sono tutte conservative si parla di urto anelastico.
>$$W_{urto}^{(I)}\not = 0$$
>$$W_{urto}^{(I)}=E_{k,fin}-E_{k,in}<0$$

Come abbiamo visto in [[Capitolo 8 - Sistemi di punti materiali]], possiamo rappresentare l'energia cinetica come
![[Capitolo 8 - Sistemi di punti materiali#^074e87]]

Cosa succede ai termini durante l'urto?

Abbiamo visto che $\vec{v}_{CM}$ si conserva ([[#^78f490]]), quindi anche $E_{k,CM}$ si conserva durante l'urto.

Anche $E^{'}_{k}$, nel caso in cui l'urto sia ==perfettamente elastico==, si conserva.
Quindi 
$$v^{'}_{1,fin}=-v^{'}_{1,in}$$
$$v^{'}_{2,fin}=-v^{'}_{2,in}$$

Se invece l'==urto fosse anelastico==, una parte dell'energia cinetica dei punti rispetto al centro di massa verrebbe dissipata, quindi
$$E^{'}_{k,in}\not = E^{'}_{k,fin}$$
Allora $$E_{k,fin}=E_{k,CM}+E^{'}_{k,fin}\not=E^{'}_{in}$$
Può esserci anche il caso in cui l'urto sia ==perfettamente anelastico==, nel quale l'energia cinetica viene dissipata, quindi 
$$E^{'}_{k,fin}=0\Rightarrow v^{'}_{1,fin} = v^{'}_{2,fin}=0$$
Allora 
$$
E_{k,fin}=E_{k,CM}\Rightarrow v_{1,fin}=v_{2,fin}=v_{CM}
$$
Vuol dire che i punti materiali rimangono attaccati tra loro dopo l'urto.


In generale possiamo allora dire che
>[!def] Relazione fra velocità iniziale e finale
>$$v^{'}_{1,fin}=-e_{r}v^{'}_{1,in}$$
>$$v^{'}_{1,fin}=-e_{r}v^{'}_{1,in}$$

Dove $e_{r}$ è una costante definita come
>[!def] Coefficiente di restituzione
>$$e_{r}=-\frac{v^{'}_{1,fin}}{v^{'}_{1,in}}=-\frac{v^{'}_{2,fin}}{v^{'}_{2,in}}$$
>$$0\le e_{r}\le 1$$
>Se $e_{r}= 1$ si parlerà di un urto perfettamente elastico.
>Se $e_{r}=0$ si parlerà di urto perfettamente anelastico.

>[!def] Energia cinetica in un urto 
>$$\begin{split}
>&E^{'}_{k,fin}=\\&&=\frac{1}{2}m_{1}v^{'}_{1,fin}+\frac{1}{2}m_{2}v^{'}_{2,fin}=\\
&&=\frac{1}{2}m_{1}e_{r}^{2}v^{'}_{1,fin}+\frac{1}{2}m_{2}e_{r}^{2}v^{'}_{2,fin} = \\ &=e_{r}^{2}E^{'}_{k,in}
  \end{split}$$

Possiamo calcolare la variazione relativa di energia cinetica
>[!def] Variazione relativa di energia cinetica
>$$\delta=\frac{E^{'}_{k,fin}-E^{'}_{k,fin}}{E^{'}_{k,in}}=e_{r}^{2}-1$$Se $\delta = 0$ si parlerà di urto perfettamente elastico.
>Se $\delta = -1$ si parlerà di urto perfettamente anelastico.

