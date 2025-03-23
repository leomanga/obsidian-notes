>[!def] Processi congiuntamente Gaussiani
>I processi $X(t)$ e $Y(t)$ sono congiuntamente Gaussiani se $\forall n,m$, $\forall (t_1,t_2,\ldots,t_{n})$ e $\forall(\tau_{1},\tau_{2},\ldots,\tau_{m})$ il vettore di variabili aleatorie
>$$[X(t_1),X(t_{2}),\ldots, X(t_{n}), Y(\tau_1),\ldots, Y(\tau_{m})]$$
>è distribuito secondo una distribuzione congiuntamente Gaussiana di dimensione $n+m$
>#TODO scrivere in statistica la distribuzione cong gaussiana

^a4f7e2

>[!def] Processo Gaussiano
$X(t)$ è un processo Gaussiano se per ogni $n$ e per ogni $(t_{1},t_{2}, \ldots, t_{n})$ le variabili aleatorie $\{X(t_{1),}X(t_{2}),\ldots, X(t_n)\}$ sono [[#^a4f7e2|congiuntamente Gaussiani]]

>[!prp] Proprietà
>1) $X(t)$ Gaussiano in ingresso ad un sistema [[Sistemi lineari tempoinvarianti|LTI]] $\Rightarrow$ $Y(t)$ di uscita è ancora Gaussiano e i due processi $X(t)$ e $Y(t)$ sono congiuntamente Gaussiani.
>	(Importante perchè solo per i processi Gaussiani, la conoscenza delle proprietà statistiche del segnale aleatorio in ingresso fornisce la conoscenza delle proprietà statistiche del processo di uscita).
>2) Se $X(t)$ e $Y(t)$ sono congiuntamente Gaussiani, allora
>	$$X(t)\mbox{ e } Y(t)\mbox{ incorrelati}\iff X(t)\mbox{ e } Y(t)\mbox{ indipendenti}$$
>	(In genere vale solo $\Leftarrow$)
>	

