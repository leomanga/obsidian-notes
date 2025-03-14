Abbiamo visto in Analisi II la [[Serie di fourier]] per funzioni $f: \mathbb{R}\to \mathbb{R}$

Farà molto comodo esprimere un segnale come combinazione di esponenziali complessi dato che, come abbiamo visto in [[Sistemi in telecomunicazioni#Risposta a un segnale esponenziale complesso]], la risposta a un segnale esponenziale complesso è nuovamente un segnale esponenziale complesso.

# Studio dei segnali periodici
Sia $x(t)$ un [[Serie di fourier#^88ecc8|segnale periodico]] di periodo $T_{0}$.
Supponiamo che $x(t)$ soddisfi le condizioni di Dirichlet

>[!def] Condizioni di Dirichlet
> Sia $x(t): \mathbb{R}\to \mathbb{C}$ periodica di periodo $T_{0}$
> $x(t)$ soddisfa le condizioni di Dirichlet se
> - $\int_{0}^{T_{0}}|x(t)|dt<\infty$, ovvero deve essere assolutamente integrabile sul periodo.
> - Il numero di massimi e minimi di $x(t)$ nel periodo è finito.
> - Il numero di discontinuità di $x(t)$ nel periodo è finito.

allora il segnale periodico si può esprimere come somma pesata di infiniti segnali esponenziali complessi di frequenza multipla di $\frac{1}{T_{0}}$
$$x(t)=\sum_{n=-\infty}^{\infty}x_{n}e^{j2\pi \frac{n}{T_{0}}t}$$
dove $$x_{n}=\frac{1}{T_{0}}\int_{\alpha}^{\alpha+T_{0}}x(t)e^{-j2\pi\frac{n}{T_{0}}t}dt$$
$x_{n}, n\in \mathbb{Z}$