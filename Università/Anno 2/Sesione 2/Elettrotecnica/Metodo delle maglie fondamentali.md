Il metodo delle maglie fondamentali usa [[Grafo associato a un circuito]].
Si usa per le reti di bipoli [[Bipoli controllabili in tensione o corrente|controllabili in corrente]].

Possiamo, grazie a questo metodo, scrivere un sistema risolvente.
In generale otterremo $$R\vec{i}_{C}=\vec{v}_{gen}$$
dove $\vec{I_c}$ sono le correnti cicliche associate alle maglie fondamentali, $\vec{v_{gen}}$ le tensioni dei generatori e $R\in \mathbb{R}^{\ell -n+1}$ la matrice che rappresenta la relazioni fra di esse.
Di seguito la costruzione del sistema, che vale solo per reti di generatori indipendenti di tensione.
- Costruiamo gli elementi di $R_{kk}$ sommando tutte le resistenza sulla maglia $k$.
- Costruiamo gli elementi $R_{hk}, h\not = k$ sommando algebricamente le resistenze a comune fra la maglia $k$ ed $h$, prendendo con il segno $+$ le resistenze se $I_{k}$ e $I_{h}$ sono in senso concorde, altrimenti con il $-$.
- Costruiamo $\vec{v}_{k}$ sommando algebricamente le tensioni dei generatori indipendenti di tensione della maglia fondamentale, prendendo con il $+$ le tensioni se $I_{k}$ esce dal morsetto $+$ del generatore, altrimenti con il $-$.

>[!nota]
>La matrice $R$ è simmetrica.

Se ci fossero generatori indipendenti di corrente, che sono quindi non controllabili in corrente, dovremo usare una versione modificata.
Associamo ad ogni generatore di corrente una tensione incognita.
A questo punto avremo 2 passi: 
1) Facciamo il passaggio visto sopra usando le tensioni incognite come se fossero erogate dai generatori di corrente.
2) Utilizziamo le relazioni costitutive del generatore di corrente per scrivere equazioni aggiuntive dette equazioni di vincolo e le includiamo come nuove righe della matrice. Le colonne nasceranno spostando le tensioni incognite nel vettore $\vec{I}_{c}$, allungandolo.



