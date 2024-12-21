Gli elettroni in un corpo [[Materiali conduttori|conduttore]] sono liberi di muoversi (in minima parte anche nei [[Materiali isolanti|dielettrici]]).

Gli elettroni si muovono in modo disordinato urtando gli ioni che scambiano a loro volta elettroni.
Si può calcolare la velocità media di ogni elettrone è detta velocità termica,
$$v_{T}^{m}\simeq\sqrt{\frac{3kT}{m_{e}}}$$
dove $m_{e}$ è la massa di un elettrone.
Indichiamo inoltre con $\tau$ il tempo medio tra un urto e il successivo e con $l$ il libero cammino medio tra due urti successivi. Allora avremo $\tau = \frac{l}{v_{t}^{m}}$.
Indichiamo con $\vec{v}_{i}$ la velocità di un elettrone subito dopo un urto.
Dopo ogni urto, la distribuzione di velocità è casuale, quindi facendo la media su un corpo, quindi con molti elettroni avremo
$$\frac{1}{N}\sum_{i}^{N}\vec{v}_{i}=0$$

Se però applichiamo al conduttore un campo elettrostatico esterno, ogni elettrone acquisterà un’accelerazione $\vec{a}=-\frac{e\vec{E}}{m_{e}}$ opposta al campo elettrico.
Se indichiamo con $\vec{v}_{i+1}$ la velocità prima del successivo urto, allora
$$\vec{v}_{i+1}=\vec{v}_{i}-\frac{e\vec{E}}{m_{e}}\tau$$
Se effettuiamo nuovamente la media avremo
$$\frac{1}{N}\sum_{i}^{N}\vec{v}_{i+1}=-\frac{e\vec{E}}{m_{e}}\tau$$
Allora possiamo dire che se guardiamo globalmente, gli elettroni avranno un carattere di moto uniforme, con una velocità media, che prende il nome di **velocità di deriva** $\vec{v}_{d}=-\frac{e\vec{E}}{m_{e}}\tau$.
Gli elettroni allora avranno un moto ordinato.

Se  guardiamo ora il disegno,

![[Conduttore attraversato da un flusso.excalidraw]]

Se $V_{A}>V_{B}$, allora nasce un campo elettrostatico e gli elettroni si muoveranno in modo da cercare di raggiungere l’equilibrio. (ci vogliono circa $10^{-15}\quad s$) Gli elettroni andranno dalla parte ad alto potenziale a quella a basso potenziale e quindi possiamo immaginare che si generi un flusso di cariche positive cha va dalla carica a minor potenziale fino a quella a maggior potenziale.
Si genera allora una **corrente elettrica di conduzione**.

>[!def] Corrente elettrica
>$$I(t)=\frac{dQ}{dt}\quad [\frac{Q}{s}][A]$$
>Dove $\frac{dQ}{dt}$ è la quantità di cariche che passano per il conduttore per un tempo infinitesimo.
>$A$ indica gli **ampere**.
>(Per convenzione il segno segue la direzione delle cariche positive).

^5dcb3a

> [!prp] Calcolo della potenza elettrica
> Dato che da [[#^5dcb3a]] possiamo scrivere $dQ=Idt$ e da [[Potenziale elettrostatico]] possiamo dire che il lavoro è $dL=dQ(V_A -V_{B})$, allora
>$$dL=I(V_{A}-V_{B})dt$$
>Allora possiamo scrivere che $$\frac{dL}{dt}=I(V_{A}-V_{B})\quad [V\cdot A][W]$$ che, essendo un lavoro nel tempo è proprio la [[Potenza]] elettrica.
. 

[[Densità di corrente elettrica]]
