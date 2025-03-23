I processi aleatori definiscono i segnali aleatori, che, a differenza di quelli “normali”, non hanno un andamento definito, ma dipendono dal singolo esperimento o dalla specifica osservazione.

Si possono interpretare in due possibili modi:
- L’insieme delle possibili realizzazioni delle forme d’onda di un segnale(Es. il rumore termico nei circuiti elettronici)
- Una serie infinita ed ordinata nel tempo di variabili aleatorie.

Un segnale aleatorio inoltre si può caratterizzare conoscendo le [[Densità di probabilità]] congiunte per ogni n-upla di tempi $t_{1}, t_{2}, \ldots, t_{n}$ delle variabili aleatorie $X(t_{1}), X(t_{2}), \ldots , X(t_{n})$
$$f_{X(t_{1}), X(t_{2}),\ldots, X(t_{n})}(x_{1},x_{2},\ldots, x_{n})$$
Si dice che una caratterizzazione è di ordine $M$ se sono note le probabilità congiunte per ogni $n\le M$.

Spesso, nei sistemi di telecomunicazioni è sufficiente una caratterizzazione del secondo ordine

>[!def] Funzione di autorrelazione
>Per un processo $X(t)$ reale, la sua funzione di autocorrelazione è
$$R_{X}(t_{1}, t_{2})=E[X(t_{1})X(t_{2})]=\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}x_{1}x_{2}f_{X(t_{1}),X(t_{2})}(x_{1},x_{2})dx_{1}dx_{2}$$
>>[!prp]
>>$$R_X(t_{1},t_{2})=R_X(t_2,t_1)$$

^2bc971

>[!def] Funzione di (auto)covarianza
>$$C_{X}(t_1,t_{2})=E[(X(t_1)-m_x(t_{1}))(X(t_2)-m_X(t_2))]$$

>[!def] Processi stazionari
>Si dice che $X(t)$ è stazionario in senso stretto se $\forall(t_1,t_2,\ldots,t_{n}) \mbox{ e }\forall \Delta$ 
>$$f_{X(t_1),X(t_2),\ldots,X(t_{n})}(x_1,x_2,\ldots,x_n)=f_{X(t_1+\Delta),X(t_2+\Delta),\ldots, X(t_n+\Delta)}(x_1,x_2,\ldots,x_{n})$$
>
>Es: Il rumore bianco fa parte dei processi stazionari

^6ade42

>[!def] Processi stazionari in senso lato
>$X(t)$ si dice che è stazionario in senso lato se soddisfa le seguenti proprietà:
>- $m_X(t)=m_{X}\ \forall t$
>- $R_X(t_1,t_2)=R_X(t_1+\tau,t_1)=R_{X}(\tau)\ \forall t_{1}$ con $\tau =t_1-t_2$
>
>Di conseguenza, per un processo stazionario in senso lato
>- $R_{X(\tau)}=R_{X}(-\tau)\ \forall \tau$
>- $R_{X}(\tau)\le R_{X}(0)\ \forall \tau$
>- $E[X^{2}(t)]=R_{X}(0)\ \forall t$ (potenza media di $X(t)$

>[!def] Cross-correlazione di due processi
>Siano $X(t)$ e $Y(t)$ due processi, allora la funzione di cross-correlazione fra di essi è definita come
>$$R_{XY}(t_1,t_2)=E[X(t_1)Y(t_2)]$$
>[[#^2bc971]]

>[!def] Cross-covarianza di due processi
>Siano $X(t)$ e $Y(t)$ due processi, allora la funzione di cross-covarianza fra di essi è definita come
>$$C_{XY}(t_1,t_2)=E[(X(t_1)-m_X(t_1))(Y(t_2)-m_{Y}(t_{2}))]$$

>[!def] Processi indipendenti
>$X(t)$ e $Y(t)$ sono indipendenti se $\forall m,n,\forall t_1,t_2,\ldots,t_{n}, \forall T_1,T_{2},\ldots,T_{m}$ i vettori aleatori
>$$[X(t_1),\ldots,X(t_{n})], [Y(T_{1),}\ldots, Y(T_{m})]$$
>sono indipendenti.

>[!def] Processi incorrelati
>#TODO guarda appunti statistica per finire(stesasa cosa dei processi indipendenti)

>[!def] Processi congiuntamente stazionari in senso lato
>$X(t)$ e $Y(t)$ si dicono congiuntamente stazionari in senso lato se
>1) $X(t), Y(t)$ sono entrambi stazionari in senso lato
>2) $R_{XY}(t_1,t_2)=R_{XY}(t_1-t_2)=R_{XY}(\tau)$ (La cross-correlazione dipende solo da $\tau$)

>[!prp] Somma di segnali aleatori congiuntamente stazionari
>Se $X(t)$ e $Y(t)$ sono segnali aleatori a valori reali, congiuntamente stazionari in senso lato, allora
>1) $Z(t)=X(t)+Y(t)$ è stazionario in senso lato
>2) $R_{Z}(\tau)=R_{X}(\tau)+R_{Y}(\tau)+R_{XY}(\tau)+R_{XY}(-\tau)$
>3) $S_{z}(f)=S_{X}(f)+S_{Y}(f)+S_{XY}(f)+\underbrace{S_{YX}(f)}_{S^{*}_{XY}(f)}=S_{X}(f)+S_{Y}(f)+2Re[S_{XY}(f)]$ 

>[!thm] Caratterizzazione in frequenza di un processo stazionario (Teorema di Wiener-Khinchin)
>Sia $X(t)$ un processo [[#^6ade42|stazionario]].
>Allora $$S_{X}(f)=\mathcal{F}\{R_{X}(\tau)\}=\int_{-\infty}^{\infty}R_{X}(\tau)e^{-j2\pi f\tau}d\tau$$
>$$R_{X}(0)=P_{m}=E[X^{2}(t)]=\int_{-\infty}^{\infty}S_{X}(f)df$$
>Dove $S_X(f)$ è la [[Segnali caratterizzati in energia o in potenza#^af7d4c|densità spettrale di potenza]] del processo $X(t)$
>>[!prp]
>>- $S_{X}(f)\in \mathbb{R}$
>>- $S_{X}(f)=S_{X}(-f)\ \forall f$
>>- $P_{(f_{1},f_{2})}=2\int_{f_{1}}^{f_{2}}S_{X}(f) df$, $0\le f_{1}<f_{2}$
>>- $S_{X}(f)\ge 0\ \forall f$

[[Processi Gaussiani]]
[[Processi bianchi]]