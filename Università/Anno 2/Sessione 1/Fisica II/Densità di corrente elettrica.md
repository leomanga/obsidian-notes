Consideriamo un conduttore, all’interno del quale si abbiano $N$ portatoti di carica per unità di volume, ognuno di carica $q$.
Ogni carica ha la sua velocità di deriva $\vec{v}_{d}$, che avrà direzione parallela al campo $\vec{E}$ localmente presente nel conduttore. 
Possiamo considerare un tubo di flusso elementare dato dalla velocità in un istante infinitesimo e da una sezione $d\vec{S}$.

Allora la quantità di carica $dQ$ che in un tempo $dt$ passa attraverso $d\vec{S}$ con normale $\hat{n}$ vale
$$dQ = Nq\vec{v}_{d}\cdot d\vec{S}dt=Nqv_{d}dS_{n}dt$$
Sove $dS_{n}=dS\cos \theta$

![[Densità di corrente.excalidraw]]

Abbiamo allora che $\frac{dQ}{dt}=dI=Nqv_{d}dS$
Definiamo

>[!def] Densità di corrente
>$$\vec{J}=Nq\vec{v}_{d}\quad [\frac{A}{m^{2}}]$$

Allora $$I = \iint_{S}\vec{J}(\vec{r})\cdot \vec{n}dS$$


In un [[Materiali conduttori|conduttore]] metallico, avremo
$$\vec{J}=\frac{N(-e)(-e)\vec{E}\tau}{m_{e}}$$