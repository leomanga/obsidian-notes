>[!def] Segnale caratterizzato in energia
>Un segnale si dice caratterizzato in [[Segnali#^f4d1be|energia]] se $E_{x}<\infty$

^57d0e5


>[!def] Segnale caratterizzato in potenza
>Un segnale si dice caratterizzato in [[Segnali#^5a2215|potenza]] se $0<P_{x}<\infty$

^65ebe9

>[!prp]
>Un segnale non può essere sia caratterizzato in [[#^57d0e5|energia]] che in [[#^65ebe9|potenza]].
>Questo è dovuto al fatto che se la potenza media finita non nulla implica energia infinita ed energia finita implica potenza media nulla.

>[!prp] I segnali periodici sono caratterizzati in potenza

>[!def] Funzione di autocorrelazione per segnali [[Segnali caratterizzati in energia o in potenza#^57d0e5|caratterizzati in energia]]
>$$R_{x}(\tau)=x(\tau)*x^{*}(-\tau)$$
>$R_{x}(0)=E_{x}=\int_{-\infty}^{\infty}|X(f)|^{2}df$


>[!def] Densità spettrale di energia di un [[#^57d0e5|segnale caratterizzato in energia]]
>$$\mathcal{G}_{x}(f)=|X(f)|^2=\mathcal{F}\{R_{x}(\tau)\}$$

>[!def] Media temporale della funzione di autocorrelazione per segnali [[#^65ebe9|caratterizzati in potenza]]
>$$R_{x}(\tau)=\lim_{T\to \infty}\frac{1}{T}\int_{-\frac{T}{2}}^{\frac{T}{2}}x(t)x^{*}(t-\tau)d\tau$$
>$$R_{x}(0)=\lim_{T\to \infty}\frac{1}{T}\int_{-\frac{T}{2}}^{\frac{T}{2}}|x(t)|^{2}dt=P_{x}$$
>

^bb4353

>[!def] Densità spettrale di potenza per segnali [[#^65ebe9|caratterizzati in potenza]]
>$R_{x}(\tau)$ la [[#^bb4353|media temporale della funzione di autocorrelazione]]
>$$\mathcal{S}(f)=\mathcal{F}\{R_{x}(\tau)\}$$
>$$\int_{-\infty}^{\infty}\mathcal{S}_{x}(f)df=P_{x}$$

^af7d4c
