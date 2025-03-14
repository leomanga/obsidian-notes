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
$x_{n}, n\in \mathbb{Z}$ sono i coefficienti dell’espansione in serie di Fourier del segnale periodico $x(t)$.

Sia $l\in \mathbb{Z}$, allora riarrangiando, 
$$x_{l}=\sum_{n=-\infty}^{\infty}x_{n} \frac{1}{T_{0}}\int_{\alpha}^{\alpha+T_{0}}e^{j\frac{2\pi}{T_{0}}(n-l)t}dt$$
Da qui capiamo che $\frac{1}{T_{0}}\int_{\alpha}^{\alpha+T_{0}}e^{j\frac{2\pi}{T_{0}}(n-l)t}dt=\begin{cases}1\quad n=l\\ 0\quad n\not = l\end{cases}$

Inoltre, sia $x(t)\in \mathbb{R}$ periodico di periodo $T_{0}$ e sviluppabile in serie di Fourier, allora
 $$x_{-n}=\frac{1}{T_{0}}\int_{\alpha}^{\alpha+T_{0}}x(t)e^{j2\pi\frac{n}{T_{0}}(-t)}dt = x_{n}^{*} $$
 dove $x_{n}^{*}$ è il [[Campo dei numeri complessi#^b34f54|coniugato]] di $x_{n}$.
 Allora la sequenza dei coefficienti $|x_n|$ ha simmetria pari: $|x_{n}| = |x_{-n}|$ e la sequenza dei coefficienti $\measuredangle x_{n}$ ha simmetria dispari: $\measuredangle x_{n}= -\measuredangle x_{-n}$
  
 Definendo allora $x_{n}= \frac{a_{n}-jb_{n}}{2}$ si ha che $x_{-n}=\frac{a_{n}+jb_{n}}{2}$
 Allora per $n\ge 1$