Consideriamo un conduttore, all’interno del quale si abbiano $N$ portatoti di carica per unità di volume, ognuno di carica $q$.
Ogni carica ha la sua velocità di deriva $\vec{v}_{d}$, che avrà direzione parallela al campo $\vec{E}$ localmente presente nel conduttore. 
Possiamo considerare un tubo di flusso elementare dato dalla velocità in un istante infinitesimo e da una sezione $d\vec{S}$.

Allora la quantità di carica $dQ$ che in un tempo $dt$ passa attraverso $d\vec{S}$ con normale $\hat{n}$ vale
$$dQ = Nq\vec{v}_{d}\cdot d\vec{S}dt=Nqv_{d}dS_{n}dt$$
Sove $dS_{n}=dS\cos \theta$

![[Densità di corrente.excalidraw]]

Abbiamo allora che $\frac{dQ}{dt}=\vec{dI}=Nqv_{d}dS$
Definiamo

>[!def] Densità di corrente
>$$\vec{J}=\frac{dQ}{dt}=\vec{dI}=Nq\vec{v}_{d}\quad [\frac{A}{m^{2}}]$$

^cd6c08

Allora $$I = \iint_{S}\vec{J}(\vec{r})\cdot \vec{n}dS$$


In un [[Materiali conduttori|conduttore]] metallico, avremo, da [[Corrente elettrica#^3a4386]]
$$\vec{J}=\frac{N(-e)(-e)\vec{E}\tau}{m_{e}}=\underbrace{\frac{Ne^{2}\tau}{m_{e}}}_{conducibilità\ elettrica}\vec{E}$$
Definiamo così
>[!def] Conducibilità elettrica
>$$\sigma = \frac{Ne^{2}\tau}{m_{e}}$$
>dove $N$ è il numero di portatori di cariche, $e$ è la carica di un elettrone, $m_{e}$ è massa dell’elettrone e $\tau$ è il tempo medio tra un urto ed un altro fra gli elettroni.

Ora possiamo definire l’**equazione di continuità della carica elettrica**.
>[!def] Equazione di continuità della carica
>Sapendo che $$Q(t)=\iiint_V\rho({r,t})dv$$
>dove $\rho$ è la [[Densità volumetrica di carica elettrica|densità volumetrica di carica elettrica]].
>Allora, da [[#^cd6c08]], in una superficie chiusa, dato che la carica non si può distruggere e deve necessariamente passare dal bordo della superficie chiusa
>$$-\frac{dQ}{dt}=\oint \vec{J}(\vec{r},t)\cdot \hat n\cdot ds=I(t)$$
>(Il segno è negativo perchè rappresentiamo la carica uscente)
