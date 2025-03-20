I processi aleatori definiscono i segnali aleatori, che, a differenza di quelli “normali”, non hanno un andamento definito, ma dipendono dal singolo esperimento o dalla specifica osservazione.

Si possono interpretare in due possibili modi:
- L’insieme delle possibili realizzazioni delle forme d’onda di un segnale(Es. il rumore termico nei circuiti elettronici)
- Una serie infinita ed ordinata nel tempo di variabili aleatorie.

Un segnale aleatorio inoltre si può caratterizzare conoscendo le [[Densità di probabilità]] congiunte per ogni n-upla di tempi $t_{1}, t_{2}, \ldots, t_{n}$ delle variabili aleatorie $X(t_{1}), X(t_{2}), \ldots , X(t_{n})$
$$f_{X(t_{1}), X(t_{2}),\ldots, X(t_{n})}(x_{1},x_{2},\ldots, x_{n})$$
Si dice che una caratterizzazione è di ordine $M$ se sono note le probabilità congiunte per ogni $n\le M$.

Spesso, nei sistemi di telecomunicazioni è sufficiente una caratterizzazione del secondo ordine

## Funzione di autorrelazione

Per un processo $X(t)$ reale, la sua funzione di autocorrelazione è
$$R_{x}(t_{1}, t_{2})=E[X(t_{1})X(t_{2})]=\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}x_{1}x_{2}f_{X(t_{1}),X(t_{2})}(x_{1},x_{2})dx_{1}dx_{2}$$
>[!prp]
>$$R_X(t_{1},t_{2})=R_X(t_2,t_1)$$

## Funzione di (auto)covarianza
$$C_{X}(t_1,t_{2})=E[(X(t_1)-m_x(t_{1}))(X(t_2)-m_X(t_2))]$$


COntinua da processi stazionari pag 5