
>[!prp] Relazione costitutiva
>Da [[Induttanza]] avremo
>$$v(t)=\frac{d\Phi(t)}{dt} = L\frac{di(t)}{dt}$$
>oppure
>$$i(t)=i(0)+\frac{1}{L}\int_{0}^{t}v(\tau)d\tau$$
>

^cbd7cc

Dalla relazione costitutiva si vede che l’induttore è un elemento con memoria. Per conoscere $i(t)$ devo conoscere lo stato iniziale $i(0)$ e l’andamento di $v(t)$.

>[!prp] Potenza istantanea
>$$p(t)=v(t)i(t)=i(t)L\frac{di(t)}{dt}=\frac{d}{dt}(\frac{1}{2}Li^{2}(t))=\frac{d}{dt}E_{L}(t)$$
>dove $E_{L}(t)$ è l’energia associata al campo magnetico di $L$.

# Regime sinusoidale
Dalla sua [[Induttanza]], avremo $$v(t)=L\frac{d}{dt}i(t)=\frac{d\phi_{conc}}{dt}$$
dove $\phi_{conc}=Li$ è il [[Flusso di un campo vettoriale|flusso]] magnetico concatenato, generato dalla spira.

Se il nostro induttore fosse percorso da una corrente continua, allora $v(t)=0$, quindi potremmo interpretarlo come un corto circuito.
Se invece fosse attraversato da una corrente di tipo $i(t)=I_M\cos(\omega t+\phi_{i})$.
Allora
$$\begin{split}v(t)&=V_M \cos(\omega t+\phi_v)=L\frac{d}{dt}i(t)\\ &-\omega LI_{M} \sin(\omega t+\phi_{i})=\omega L I_{M}\cos(\omega t+\phi_{i}+\frac{\pi}{2})\end{split}$$
quindi $$V_{M}=\omega LI_{M}=X_{L}I_{M}\quad \phi_{v}=\phi_{i} + \frac{\pi}{2}$$
dove $X_{L}$ è la [[Reattanza]]
