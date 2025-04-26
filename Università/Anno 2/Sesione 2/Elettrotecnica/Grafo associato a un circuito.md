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

Aggiungiamo due definizioni:
- Albero: Insieme connesso di lati del grafo che tocca tutti i nodi senza formare percorsi chiusi
  Come proprietà, i rami saranno $n-1$, inoltre i tagli fondamentali sono in corrispondenza biunivoca con i rami dell’albero. I tagli fondamentali sono tagli che contengono un ramo dell’albero e solamente corde del coalbero. Ogni taglio si orienta secondo il verso della corrente del ramo corrispondente.
- Coalbero: Insieme di lati del grafo che non fanno parte dell’albero.
  Come proprietà, le sue corde saranno $\ell-n-+1$ e non contiene tagli, ovvero non si può tagliare il grafo in due parti intersecando solo corde.
  Inoltre le maglie fondamentali sono in corrispondenza biunivoca con le corde del coalbero(ci sono $\ell-n+1$ maglie fondamentali.) Le maglie fondamentali sono quelle maglie composta da solo rami ed una sola corda.

Con le nuove definizioni possiamo ora rappresentare le tensioni indipendenti e quelle dipendenti.
Sia $$\vec{v}=(v_1,v_2,\ldots,v_\ell)^T$$
il vettore delle tensioni, indicheremo con $\vec{v_{a}}$ il vettore delle $n-1$ tensioni dei rami dell’albero e con $\vec{v_{c}}$ il vettore delle $\ell -n+1$ tensioni delle corde dell’albero.
Le tensioni $\vec{v_{a}}$ formeranno una base per lo spazio delle tensioni dei lati del grafo dato che sono indipendenti fra loro e si possono determinare le tensioni dipendenti $\vec{v_{c}}$ scrivendo $\ell-n+1$ [[Legge di Kirchhoff per le tensioni (KV)|KV]] alle maglie fondamentali associate all’albero.

Sia $$\vec{i}=(i_1,i_2,\ldots,i_\ell)^T$$
il vettore delle correnti dei lati del grafo.
Indicheremo con $\vec{i_c}$ il vettore delle $\ell-n+1$ correnti delle corde del coalbero e con $\vec{i_a}$ il vettore delle $n-1$ correnti dei rami dell’albero.
Le correnti $\vec{i_c}$ formeranno una base per lo spazio delle correnti dei lati del grafo dato che sono indipendenti fra loro e si possono determinare le correnti dipendenti $\vec{i_{a}}$ scrivendo $n-1$ [[Legge di Kirchhoff per le correnti (KI)|KI]] ai tagli fondamentali associati all’albero.

