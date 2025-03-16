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
$$
x(t)=\sum_{n=-\infty}^{\infty}x_{n}e^{j2\pi \frac{n}{T_{0}}t}
$$

^09ce92

dove 
$$
x_{n}=\frac{1}{T_{0}}\int_{\alpha}^{\alpha+T_{0}}x(t)e^{-j2\pi\frac{n}{T_{0}}t}dt
$$

^4b4265

$x_{n}, n\in \mathbb{Z}$ sono i coefficienti dell’espansione in serie di Fourier del segnale periodico $x(t)$.

Sia $l\in \mathbb{Z}$, allora riarrangiando, 
$$x_{l}=\sum_{n=-\infty}^{\infty}x_{n} \frac{1}{T_{0}}\int_{\alpha}^{\alpha+T_{0}}e^{j\frac{2\pi}{T_{0}}(n-l)t}dt$$
Da qui capiamo che $\frac{1}{T_{0}}\int_{\alpha}^{\alpha+T_{0}}e^{j\frac{2\pi}{T_{0}}(n-l)t}dt=\begin{cases}1\quad n=l\\ 0\quad n\not = l\end{cases}$

Inoltre, sia $x(t)\in \mathbb{R}$ periodico di periodo $T_{0}$ e sviluppabile in serie di Fourier, allora
 $$x_{-n}=\frac{1}{T_{0}}\int_{\alpha}^{\alpha+T_{0}}x(t)e^{j2\pi\frac{n}{T_{0}}(-t)}dt = x_{n}^{*} $$
 dove $x_{n}^{*}$ è il [[Campo dei numeri complessi#^b34f54|coniugato]] di $x_{n}$.
 Allora la sequenza dei coefficienti $|x_n|$ ha simmetria pari: $|x_{n}| = |x_{-n}|$ e la sequenza dei coefficienti $\measuredangle x_{n}$ ha simmetria dispari: $\measuredangle x_{n}= -\measuredangle x_{-n}$
  
 Definendo allora $x_{n}= \frac{a_{n}-jb_{n}}{2}$ si ha che $x_{-n}=\frac{a_{n}+jb_{n}}{2}$
 Per $n\ge 1$, avremo
 $$x_{n}e^{j2\pi \frac{n}{T_{0}}t}+x_{-n}e^{-j2\pi\frac{n}{T_{0}}t}=a_{n}\cos(2\pi\frac{n}{T_{0}}t)+b_{n}\sin(2\pi\frac{n}{T_{0}}t)$$
 ovviamente $x_{0}=\frac{a_{0}}{2}$, allora
 $$x(t)=\frac{a_{0}}{2}+\sum_{n=1}^{\infty}[a_{n}\cos(2\pi\frac{n}{T_{0}}t)+b_{n}\sin(2\pi\frac{n}{T_{0}}t)]$$
 E qui si arriva a ciò che abbiamo visto in [[Serie di fourier]], ma in modo esteso.
 Inoltre, per calcolare i coefficienti $a_{n}$ e $b_{n}$ avremo, da [[#^4b4265]]
 $$\begin{split}&x_{n}= \frac{a_{n}-jb_{n}}{2}=\frac{1}{T_{0}}\int_{\alpha}^{\alpha+T_{0}}x(t) e^{-j2\pi \frac{n}{T_{0}}t}dt=\\&= \frac{1}{T_{0}}\int_{\alpha}^{\alpha + T_{0}}x(t)\cos(2\pi\frac{n}{T_{0}}t)dt-\frac{j}{T_{0}}\int_{\alpha}^{\alpha+T_{0}}x(t)\sin(2\pi \frac{n}{T_{0}}t)dt\end{split}$$
 quindi
 $$
 a_{n}= \frac{2}{T_{0}}\int_{\alpha}^{\alpha+T_{0}}x(t)\cos(2\pi \frac{n}{T_{0}}t)dt
 $$

^a7e737

 $$
 b_{n}=\frac{2}{T_{0}}\int_{\alpha}^{\alpha+T_{0}}x(t)\sin(2\pi\frac{n}{T_{0}}t)dt
 $$

^af8531

Un’altra espressione della serie di Fourier può anche essere
$$x(t)=x_{0}+2\sum_{n=1}^{\infty}|x_{n}| \cos(2\pi\frac{n}{T_{0}}t+\measuredangle x_{n}) $$
dove $$|x_{n}| = \frac{1}{2}\sqrt{s_{n}^{2}+b_{n}^{2}}$$
$$\measuredangle x_{n}= -\arctan(\frac{b_{n}}{a_{n}})$$
>[!prp] Fourier per segnali pari
>Se $x(t)=x(-t)\ \forall t$, allora da [[#^af8531]]
>$$b_{n}= \frac{2}{T_{0}}\int_{-\frac{T_{0}}{2}}^{\frac{T_{0}}{2}}x(t)\sin(2\pi\frac{n}{T_{0}}t)dt=0$$
>Questo perché $x(t)\sin(2\pi\frac{n}{T_{0}}t)$ è dispari.
>Quindi possiamo scrivere
>$$x(t)= \frac{a_{0}}{2}+\sum_{n=1}^{\infty}a_{n}\cos(2\pi\frac{n}{T_{0}}t)$$
>

>[!prp] Fourier per segnali dispari
>Se $x(t)=-x(-t)\ \forall t$, allora da [[#^a7e737]]
>$$a_{n}=\frac{2}{T_{0}}\int_{-\frac{T_{0}}{2}}^{\frac{T_{0}}{2}}x(t)\cos(2\pi \frac{n}{T_{0}}t)dt= 0$$
>Questo perchè $x(t)\cos(2\pi \frac{n}{T_{0}}t)$ è dispari.
>Quindi possiamo scrivere 
>$$x(t)=\frac{a_{0}}{2}+\sum_{n=1}^{\infty}b_{n}\sin(2\pi\frac{n}{T_{0}}t)$$

>[!prp] Risposta di un sistema [[LTI]] ad un segnale periodico
>Abbiamo che $x(t)$ è rappresentabile in serie di Fourier.
>![[#^09ce92]]
>L’uscita del segnale [[Sistemi lineari tempoinvarianti|LTI]] caratterizzato da una [[Risposta forzata#Risposta impulsiva|risposta impulsiva]] $h(t)$,sarà allora
>$$y(t)=T\{x(t)\}=\sum_{n=-\infty}^{\infty}x_{n}T\left\{ e^{j2\pi \frac{n}{T_{0}}t} \right\}=\sum_{n=-\infty}^{\infty}x_{n}H(\frac{n}{T_{0}})e^{j2\pi \frac{n}{T_{0}}t}$$
>dove $H(f)=\int_{-\infty}^{\infty}h(t)e^ {-j2\pi ft}dt$, da ([[Sistemi in telecomunicazioni#Risposta a un segnale esponenziale complesso]])
>Perciò anche l’uscita $y(t)$ è periodica di periodo $T_{0}$.
>



