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
$\mathcal{F}\{rect(t)\}=\frac{sen(\pi f)}{\pi f}=sinc(f)$
Dove $sinc$ è [[Segnali canonici#Sinc]]
# Proprietà

>[!prp] Proprietà di un segnale reale
>Se $x(t)\in \mathbb{R} \ \forall t$
>$$X(f)=\int_{-\infty}^{\infty}x(t)e^{-j2\pi f t dt} = X^{*}(f)=\int_{-\infty}^{\infty}x(t)e^{j 2\pi ft} dt=X(-f)$$
>Ovvero $|X(f)|=|X(-f)|, \ \measuredangle X(f)=-\measuredangle X(-f)$
>$Re(X(f))=Re(X(-f)),\ Im(X(f))=-Im(X(-f))$
>
>- Se $x(t)=x(-t)$ (pari):
>$X(f)=\int_{-\infty}^{\infty} x(t)\cos(2\pi ft) dt\Rightarrow X(f)\$




>