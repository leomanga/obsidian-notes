Dato un segnale $S_{m}(t)$, esso può essere rappresentato univocamente a partire da un insieme di funzioni $\{\phi_{k}(t)\}_{k=1}^{N}$ come $S_{m}(t)=\sum_{n=1}^{N}s_{mn}\phi_n(t)$ dove $S_{mn}(t)$ sarà la componente vettoriale e $\phi_k(t)$ comporranno la base.

$$S_{m}(t)\to \vec{S_m}=(S_{m1},S_{m2},\ldots,S_{mN})$$

Spesso sarà utile avere come insieme di funzioni un insieme ortogonale oportonormale.
>[!def] insieme di funzioni ortogonale
>Un insieme di funzioni si dice ortogonale se $$<\phi_{m}(t),\phi_{n}(t)>=\int_{-\infty}^{\infty}\phi_m(t)\phi_{n}(t)dt=\begin{cases}k\quad \mbox{se } m=n\\ 0\quad \mbox{altrimenti}\end{cases}$$

^9ac538


>[!def] Insieme di funzioni ortonormale
>Un insieme di funzioni si dice ortonormale se $$<\phi_{m}(t),\phi_{n}(t)>=\int_{-\infty}^{\infty}\phi_m(t)\phi_{n}(t)dt=\delta_{m,n}$$
>dove $\delta_{m,n}$ è la [[Delta di Kronecker]]
>Vuol dire quindi che le funzioni sono ortogonali fra loro e il prodotto scalare è 1.

Dati $S_m(t)$, $m=1,\ldots,M$ è sempre possibile costruire un set di $N\le M$ funzioni ortonormali $\{\phi_{k}\}_{k=1}^{N}$ che li rappresentano.
Un modo è quello di seguire il [[Procedimento di ortogonalizzazione di Gram-Schmidt]], che vale anche con le funzioni.

# Proprietà
1) $\epsilon_{m}=\int_{-\infty}^{\infty}s_{m}^2(t)=||S_{m}(t)||^{2}=||\vec{S_{m}}||^2$ ($\epsilon$ è l’ [[Segnali#^f4d1be|energia del segnale]])
2) $<\vec{S_{m}},\vec{S_k}>=<S_{m}(t), S_{k}(t)>$


