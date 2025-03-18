La trasformata di Fourier è necessaria per lo studio di segnali non periodici. Per lo studio di quelli periodici può anche bastare la serie di Fourier [[Estenzione serie di fourier al caso complesso]]
![[Estenzione serie di fourier al caso complesso#^ee6f2e]]

>[!def] Trasformata di Fourier
> Sia $x(t)$ un segnale che rispetta le [[Estenzione serie di fourier al caso complesso#^ee6f2e|condizioni di Dirichlet]].
> Si definisce la trasformata di Fourier di $x(t)$ come
> $$X(f)=\int_{-\infty}^{\infty}x(t)e^{-j2\pi f tdt}$$
> 
> Abbiamo che $|X(f)|$ rappresenta lo spettro di ampiezza e $\measuredangle X(f)$ la fase del segnale di $x(t)$.

>[!def] Antitrasformata di Fourier
>$$x(t)=\int_{-\infty}^{\infty}X(f)e^{j2\pi ft} df$$

# Trasformate notevoli
## Trasformata della segnale impulsivo
[[Segnale impulsivo]]
$$\mathcal{F}\{\delta(t)\}=1$$

Possiamo anche trasformare $\sum_{n=-\infty}^{\infty}\delta(t-nT_{0})$ passando per la [[Estenzione serie di fourier al caso complesso|serie di Fourier]]
$$\mathcal{F}\left\{\sum_{n=-\infty}^{\infty}\delta(t-nT_{0})\right\})=\frac{1}{T_0}\sum_{n=-\infty}^{\infty}\delta(d- \frac{n}{T_{0}})$$

## Trasformata del rettangolo
[[Segnali canonici#Rettangolo]]
$$\mathcal{F}\{rect(t)\}=\frac{sen(\pi f)}{\pi f}=sinc(f)$$
Dove $sinc$ è [[Segnali canonici#Sinc]]

## Trasformata del segno
[[Segnali canonici#Segno]]
Usiamo il fatto che $sgn(t)=\lim_{n\to\infty}x_{n}(t)$ dove $x_{n} = \begin{cases}e^{\frac{-t}{n}} \quad t> 0 \\ 0 \quad t=0\\ -e^{\frac{t}{n}}\quad t<0\end{cases}$
$$\mathcal{F}\{sgn(t)\}=\frac{1}{j\pi f}$$
## Trasformata del gradino
[[Gradino unitario]]
Si usa il fatto che $\mathbb{1}(t)=\frac{1}{2}+\frac{1}{2}sgn(t)$
Allora
$$\mathcal{F}\{\mathbb{1}(t)\}=\frac{1}{2}\delta(f)+\frac{1}{j2\pi f}$$
## Trasformata del sinc
Il $sinc$ non è assolutamente integrabile, quindi non rispetta le [[Estenzione serie di fourier al caso complesso#^ee6f2e|condizioni di Dirichlet]] e non si può calcolare la trasformata.

## Trasformata del segnale gaussiano
Data $x(t)= e^{-\pi t^{2}}$, la sua trasformata è $e^{-\pi f^{2}}$

## Segnale periodico
Sia $x(t)$ periodico di periodo $T_{0}$ della forma
$$x(t)=\sum_{n=-\infty}^{\infty}x_{n}e^{j2\pi \frac{n}{T_{0}}t}$$
allora
$$\mathcal{F}\{x(t)\}=X(f)=\sum_{n=-\infty}^{\infty}x_{n}\delta(f- \frac{n}{T_{0}})$$
# Proprietà

>[!prp] Proprietà di un segnale reale
>Se $x(t)\in \mathbb{R} \ \forall t$
>$$X(f)=\int_{-\infty}^{\infty}x(t)e^{-j2\pi f t dt} = X^{*}(f)=\int_{-\infty}^{\infty}x(t)e^{j 2\pi ft} dt=X(-f)$$
>Ovvero $|X(f)|=|X(-f)|, \ \measuredangle X(f)=-\measuredangle X(-f)$
>$Re(X(f))=Re(X(-f)),\ Im(X(f))=-Im(X(-f))$
>
>- Se $x(t)=x(-t)$ (pari):
>$X(f)=\int_{-\infty}^{\infty} x(t)\cos(2\pi ft) dt\Rightarrow X(f)\in \mathbb{R}, \ X(f)=-X(f)$
>- Se $x(t) P -x(-t)$ (dispari):
>$X(f)=-j\int_{-\infty}^{\infty}x(t)\sin(2\pi f t)dt\ \Rightarrow X(f)= jIm(X(f)),\ X(f)=-X(-f)$
>

>[!prp] Linearità
>$$\mathcal{F}\{ax_1(t)+bx_2(t)\}=a\mathcal{F}\{x_{1}(t)\}+b\mathcal{F}\{x_{2(t)}\}\quad \forall a,b\in \mathbb{C}$$

>[!prp] Dualità
>$$X(f)=\mathcal{F}\{x(t)\}\Rightarrow x(f)=\mathcal{F}^{-1}\{X(t)\}, X(t)=\mathcal{x(-f)}$$

>[!prp] Traslazione
>$$\mathcal{F}\{x(t-t_{0})\}= e^{-j2\pi ft_{0}}\mathcal{F}\{x(t)\}\ \forall t_{0} $$

>[!prp] Variazione di scala
>$$X(f)=\mathcal{F}\{x(t)\}\Rightarrow \mathcal{F}\{x(at)\}= \frac{1}{|a|}X\left(\frac{f}{a}\right)$$

>[!prp] Convoluzione
>$$\mathcal{F}\{x(t)*y(t)\}=\mathcal{F}\{x(t)\}\mathcal{F}\{y(t)\}=X(f)Y(f)$$

^26c916

>[!def] Traslazione in frequenza
>$$\mathcal{F}\{x(t)\}=X(f)\Rightarrow \mathcal{F}\{x(t)e^{j2\pi f_{0}t}\}=X(f-f_{0})$$

>[!prp] Relazione di Parseval nella trasformata di Fourier
>$$\int_{-\infty}^{\infty}x(t)y^{*}(t)dt=\int_{-\infty}^{\infty}X(f)Y^{*}(f)df$$

>[!prp] Funzione di autocorrelazione temporale
>$$R_{x}(\tau)=\int_{-\infty}^{\infty}x(t)x^{*}(t-\tau)dt=x(\tau)*x^{*}(-\tau)$$
>dunque, da [[#^26c916]] abbiamo
>$$\mathcal{F}\{R_{x}(\tau)\}=X(f)X^{*}(f)=|X(f)|^{2}$$

>[!prp] Derivazione nel tempo
>$$\mathcal{F}\{\frac{d}{dt}x(t)\}=j2\pi fX(f)$$
>In generale 
>$$\mathcal{F}\{\frac{d^{n}}{dt^{n}}x(t)\}=(j2\pi f)^{n}X(f)$$

>[!prp] Derivazione in frequenza
>$$\frac{d}{df}X(f)=\frac{2\pi}{j}\mathcal{F}\{tx(t)\}$$
>In generale
>$$\frac{d^{n}}{df^{n}}X(f)=\left(\frac{2\pi}{j}\right)^{n}\mathcal{F}\{t^{n}x(t)\}$$

>[!prp] Trasformata dell’integrale
>$$\mathcal{F}\{\int_{-\infty}^{t}x(\tau)d\tau\}=\frac{X(f)}{j2\pi f} + \frac{1}{2}X(0)\delta(f)$$

>[!prp] Momento n-esimo
>Comodo per [[Momento n-esimo]]
>$$\int_{-\infty}^{\infty}t^{n}x(t)dt=\left[\left(\frac{j}{2\pi}\right)^{n}\frac{d^{n}}{df^{n}}X(f)\right]_{f=0}$$

