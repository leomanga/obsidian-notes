A ciascun [[Bipolo]] facciamo corrispondere astrattamente un lato del grafo.
In generale, chiameremo con $\ell$ il numero di lati del grafo.
A questo punto si formeranno dei nodi, ovvero punti in cui sono connessi due o più bipoli. 
In generale, chiameremo con $n$ il numero di nodi.

A questo punto numeriamo i lati del grafo e assegniamo arbitrariamente un verso id riferimento per la corrente di ciascun lato indicando il verso con una freccia. Seguendo la [[Convenzioni|convenzione degli utilizzatori]], fisseremo anche la corrente di conseguenza.

A questo punto scegliamo una maglia (un percorso chiuso formato da lati del grafo), fissiamo un orientazione (oraria o antioraria) ed applichiamo le [[Leggi di Kirchhoff]](KV).

Chiaramente ogni [[Legge di Kirchhoff per le tensioni (KV)|KV]] implica un vincolo di dipendenza fra le tensioni dei lati della maglia.
Per la teoria dei grafi, le KV indipendenti sono in generale $\ell - n+1$, quindi le tensioni indipendenti dei lati sono $\ell - (\ell - n +1)=n-1$

Ogni [[Legge di Kirchhoff per le correnti (KI)|KI]] implica un vincolo di dipendenza fra le correnti dei lati intersecati dalla linea Gaussiana.
Per la teoria dei grafi, le KI indipendenti sono pari a $n-1$, quindi le correnti indipendenti dei lati del grafo sono $\ell -(n-1)=\ell -n+1$.

Unendo le KV e le KI, allora potremo ottenere tutte le tensioni e tutte le correnti.