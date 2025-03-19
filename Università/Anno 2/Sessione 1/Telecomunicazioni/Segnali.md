I segnali possono essere a tempo continuo o a tempo discreto.
Quelli a tempo discreto si possono ottenere da quelli a tempo continuo ideali tramite un campionamento.
Sia $T_{0}$ il periodo di campionamento, il segnale a tempo discreto sarà $x[n]=x(nT_{0})$

I segnali a tempo discreto a valori complessi si rappresentano tramite il loro modulo e fase.
![[Serie di fourier#^88ecc8|Segnale periodico]]

# Segnale sinusoidale a tempo continuo
$x(t)=A\cos(2\pi f_{0}t+\phi)$, dove $f_{0}=\frac{1}{T_{0}}$
$x(t+T_{0})=A\cos(2\pi f_{0}t+2\pi f_{0}T_{0}+\phi)=x(t)$
# Segnale sinusoidale a tempo discreto
$x[n]=A\cos(2\pi f_{0}n+\phi)$
Perché sia periodico di periodo $N_{0}$ dovrà essere, dalla definizione $x[n]=x[n+N_{0}]\ \forall n$
dunque $\forall n$, con $N_{0}\in \mathbb{N}, m\in \mathbb{Z}$ è necessario che
$2\pi f_{0}(n+N_{0})+\phi=2\pi f_{0}n+\phi + 2m\pi$
allora è necessario che $f_{0}=\frac{n}{N_{0}}\Rightarrow f_{0}\in \mathbb{Q}$
# Segnale esponenziale complesso a tempo continuo
$x(t)=Ae^{j(2\pi f_{0}t+\phi)}$, dove $f_{0}=\frac{1}{T_{0}}$
$x(t+T_{0})=Ae^{j\phi}e^{j(2\pi f_{0}t)}e^{j(2\pi f_{0}T_{0})}=x(0)$

>[!def] Segnali causali
>Un segnale $x(t)$ è detto causale quiando $x(t)=0\forall t<0$
>Se non fosse così il segnale viene chiamato **anticausale**.

>[!def] Segnale pari
>$x(t)$ è pari se $x(t)=x(-t)\ \forall t$

>[!def] Segnale dispari
>$x(t)$ è dispari quando $x(t)=-x(-t)\ \forall t$

>[!prp]
>Un segnale qualsiasi può essere scritto come la somma della sua parte pari $x_{e}(t)$ e della sua parte dispari $x_{0}(t)$ definite come
>$$x_e(t)=\frac{x(t)+x(-t)}{2}\quad x_{o}(t)=\frac{x(t)-x(-t)}{2}$$

>[!def] Simmetria Hermitiana
>$x(t)\in \mathbb{X}$ ha simmetria Hermitiana se ($x_r$ è la componente reale e $x_{i}$ è la componente immaginaria)
>$$\begin{cases}x_{r}(t)=x_{r}(-t)\ \forall t\\x_i(t)=-x_{i}(-t)\ \forall t\end{cases}$$
>oppure, equivalentemente
>$$\begin{cases}|x(t)|\mbox{ è pari}\\ \measuredangle x(t)\mbox{ è dispari}\end{cases}$$

>[!def] Energia di un segnale
>$$E_{x}=\int_{-\infty}^{\infty}|x(t)|^2dt=\lim_{T\to \infty}\int_{\frac{-T}{2}}^{\frac{T}{2}}|x(t)|^{2}dt=\lim_{T\to \infty}E_{x,T}$$
>dove $E_{x,t}$ è l’energia parziale al tempo $T$.

^f4d1be

>[!def] Potenza media di un segnale
>$$P_{x}=\lim_{T\to \infty} \frac{1}{T}\int_{\frac{-T}{2}}^{\frac{T}{2}}|x(t)|^{2}dt=\lim_{T\to \infty}\frac{E_{x,T}}{T}$$
>Dove $E_{x,t}$ è definita in [[#^f4d1be]]

^5a2215

>[!prp]
>I segnali ad energia finita hanno potenza media nulla.
>Esempio $x(t)=\begin{cases}2 \quad 0<t<5\\ 0 \quad \mbox{altrimenti}\end{cases}$
>$E_{x}=20$, $P_{x}=0$

>[!prp] Potenza media su segnale periodico
>$x(t)$ è un [[Serie di fourier#^88ecc8|segnale periodico]], allora
>$$P_{x}= \frac{1}{T_{0}}\int_{\frac{-T_{0}}{2}}^{\frac{T_{0}}{2}}|x(t)|^{2}dt$$
>[[Estenzione serie di fourier al caso complesso#^b91efd]]

![[Segnali canonici#Segnali utili per telecomunicazioni]]

![[Segnali caratterizzati in energia o in potenza]]