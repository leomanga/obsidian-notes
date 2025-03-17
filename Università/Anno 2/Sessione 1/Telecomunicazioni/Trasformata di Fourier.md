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
## Trasformata del rettangolo
[[Segnali canonici#Rettangolo]]
$$\mathcal{F}\{rect(t)\}=\frac{sen(\pi f)}{\pi f}=sinc(f)$$
Dove $sinc$ è [[Segnali canonici#Sinc]]
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

>[!def] Modulazione nel tempo
>$$\mathcal{F}\{x(t)\}=X(f)\Rightarrow \mathcal{F}\{x(t)e^{j2\pi f_{0}t}\}=X(f-f_{0})$$

>[!prp] Relazione di Parseval nella trasformata di Fourier
>$$\int_{-\infty}^{\infty}x(t)y^{*}(t)dt=\int_{-\infty}^{\infty}X(f)Y^{*}(f)df$$

