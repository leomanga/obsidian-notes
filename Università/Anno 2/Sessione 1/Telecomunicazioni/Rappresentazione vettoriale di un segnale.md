Dato un segnale $S_{m}(t)$, esso può essere rappresentato univocamente a partire da un insieme di funzioni $\{\phi_{k}(t)\}_{k=1}^{\infty}$.

Spesso sarà utile avere come insieme di funzioni un insieme ortonormale.

>[!def] Insieme di funzioni ortonormale
>Un insieme di funzioni si dice ortonormale se $$<\phi_{m}(t),\phi_{n}(t)>=\int_{-\infty}^{\infty}\phi_m(t)\phi_{n}(t)dt=\delta_{m,n}$$
>dove $\delta_{m,n}$ è la [[Delta di Kronecker]]
>Vuol dire quindi che le funzioni sono ortogonali fra loro e il prodotto scalare è 1.

Dati $S_m(t)$, $m=1,\ldots,M$ è sempre possibile costruire un set di $N\le M$ funzioni ortonormali $\{\phi_{k}\}_{k=1}^{N}$ che li rappresentano.
Un modo è quello di seguire il [[Procedimento di ortogonalizzazione di Gram-Schmidt]]