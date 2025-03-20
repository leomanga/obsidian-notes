La trasformata non è una vera e propria trasformata come può essere quella di fourier o laplace, ovvero non rappresenta un segnale dal dominio del tempo ad un altro.
La trasformata di Hilbert cambia un segnale nel dominio del tempo in un altro segnale sempre nel dominio del tempo.

Assumiamo $x(t)\in \mathbb{R}$ e $X(f)|_{f=0}=0$ dove $X(f)$ è la [[Trasformata di Fourier]] di $x(t)$.

$x(t)\to \hat x(t)$
$\hat x$  ha lo stesso spettro di ampiezza di $x(t)$ mentre lo spettro di fase è modificato introducendo un ritardo di $90°$ ad ogni frequenza.

Dunque alla frequenza $f_{0}>0$ (rotazione antioraria)
	la componente $e^{j2\pi f_{0}t}$ è trasformata in $e^{j(2\pi f_{0}t-\frac{\pi}{2})}=-je^{j2\pi f_{0}}$
Alla frequenza $-f_{0}<0$ (rotazione oraria)
	la componente $e^-{j2\pi f_{0}t}$ è trasformata in $e^{-j(2\pi f_{0}t - \frac{\pi}{2} )}=je^{-j(2\pi f_{0}t)}$

Nel dominio di Fourier(in frequenza) possiamo scrivere
$$\mathcal{F}\{\hat x(t)\}=\begin{cases}-j\mathcal{F}\{x(t)\}\quad f>0\\j\mathcal{F}\{x(t)\}\quad f<0\end{cases}=-jsgn(f)\mathcal{F}\{x(t)\}=-jsgn(f)X(f)$$
Poichè $\mathcal{F}\{sgn(t)\}=\frac{1}{j\pi f}$, allora $\mathcal{F}\{\frac{1}{j\pi t}\}=sgn(-f)=-sgn(f)$ da [[Trasformata di Fourier#^6317a1]].
Allora $\mathcal{F}\{\frac{1}{\pi t}\}=-jsgn(f)$

Quindi, in definitiva
$$\mathcal{F}\{\hat x(t)\}=\mathcal{F}\{\frac{1}{\pi t}\}\mathcal{F}\{x(t)\}$$
Allora
$$\hat x(t)=x(t)*\frac{1}{\pi t}=\frac{1}{\pi}\int_{-\infty}^{\infty}\frac{x(\tau)}{t-\tau}d\tau$$
>[!prp]
>Se $x(t)=A\cos(2\pi f_{0} t + \phi)\Rightarrow \hat x(t)=A\sin(2\pi f_{0} t + \phi)$

>[!prp]
>Se $x(t)$ pari allora $\hat x(t)$ è dispari

>[!prp]
>Se $x(t)$ dispari allora $\hat x(t)$ è pari

>[!prp]
>$$\hat{\hat x(t)}=-x(t)$$

>[!prp]
>$$E_{x}=E_{\hat{x}}$$
>Dove $E$ è l’[[Segnali#^f4d1be|energia del segnale]]

>[!prp] Ortogonalità
>$$\int_{-\infty}^{\infty}x(t)\hat x(t)dt=0$$

