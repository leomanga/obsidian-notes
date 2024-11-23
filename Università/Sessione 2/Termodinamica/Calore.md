---
collegamenti:
  - "[[Variabili di scambio]]"
aliases:
  - Energia termica
  - energia termica
---
Il calore è l'energia termica che viene scambiata da un sistema attraverso il suo contorno in ragione di una differenza di temperatura tra il sistema e l'ambiente (assenza di equilibrio termico).

Esprime uno scambio di energia, non lo stato di un sistema. Il calore si misura in calorie ($cal$), anche se nel [[Sistemi di misura#Sistema internazionale|sistema internazionale]] si usa l'unità di misura dell' [[Energia]], ovvero il Joule.

La caloria è definita come l'energia necessaria che permette di innalzare la temperatura di un grammo di acqua di $1°C$ dai $14,5°C$ ai $15,5°C$ alla pressione di $1 atm$.
Si può trovare che 
$$
1 [cal] = 4,186[J]
$$
# Termodinamica
Si immagini di fornire energia sottoforma di calore ad un sistema in assenza di [[Energia cinetica]] ed [[Energia potenziale della forza peso]].
A meno di non trovarsi nelle condizioni di transizione di fase, si osserverà una variazione nella [[Temperatura]].

Esiste quindi una relazione fra l'energia ($Q$) trasferita o scambiata dal sistema e la variazione di temperatura del sistema. 
Questa relazione è caratteristica di ogni sostanza e viene definita con la capacità termica $C$.
> [!def] Capacità termica ($C$)
> $$C = \frac{Q}{\Delta T}\quad [\frac{J}{K}]$$
>  $Q$ è l'energia trasferita attraverso il calore e $\Delta T$ la variazione di temperatura.
>  $J$ sono i Joule e $K$ i gradi kelvin.

^2c368a

Si definisce inoltre il calore specifico $c$, prendendo a riferimento una massa unitaria di sostanza.
> [!Def] Calore specifico ($c$)
> $$c = \frac{C}{m}\quad [\frac{J}{kg\cdot K}]$$
> Dove $C$ è la [[#^2c368a]] e $m$ la massa.

^29983e

Possiamo trovare a questo punto una relazione che lega il calore scambiato $Q$ da un sistema termodinamico di massa $m$ e calore specifico $c$ in presenza di una temperatura $\Delta T$ laddove $\frac{dE_{c}}{dt}$ e $\frac{dE_{p}}{dt}$ siano nulle.
>[!def] Calore
>$$Q=m\cdot c\cdot \Delta T=C\cdot\Delta T$$
>dove $m$ è la massa, $\Delta T$ la variazione di [[Temperatura]], $c$ il [[#^29983e]], $C$ la [[#^2c368a]].
>---
>

^f1806b



In assenza di variazioni di volume ([[Lavoro#Caso di compressione]]), $\Delta T$ rappresenta la variazione di [[Energia interna]] $U$.

>[!def] Calore specifico molare 
>$$c^{M}=\frac{C}{n}=c\cdot MM\qquad \left[\frac{J}{kmol\cdot K}\right]$$
>$C$ è la [[#^2c368a]]
>$n$ è il [[Mole|numero di moli]]
>$c$ è il [[#^29983e]]
>$MM$ è la massa molare.

^2b9c33

>[!def] Riscrittura del calore
>La dimensione del [[#^f1806b]] scambiato può anche essere riferito alle moli di sostanza
>$$Q=n\cdot c^{M}\cdot \Delta T$$
>$n$ è il [[Mole|numero di moli]]
>$c^M$ è il [[#^2b9c33]]
>$\Delta T$ la variazione di [[Temperatura]]

>[!prp] Costante universale dei gas espressa con i calori specifici
>$$R_{u}=c_{p}^{M}-c_{v}^{M}$$
>$R_{u}$ è la [[Costante universale dei gas]]
>$c_{p}^{M}$ è il [[#^2b9c33]] a [[Pressione]] costante
>$c_{v}^{M}$ è il [[#^2b9c33]] a [[Volume]] costante

^fb7889
>[!def] Rapporto fra i calori specifici
>$$k=\frac{c_{p}}{c_{v}}=\frac{c_{p}^{M}}{c_{v}^{M}}$$
>$c_{p}^{M}$ è il [[#^2b9c33]] a [[Pressione]] costante
>$c_{v}^{M}$ è il [[#^2b9c33]] a [[Volume]] costante

Definiamo inoltre la quantità di energia trasferita in un certo intervallo di tempo come il 
![[Flusso di calore]]
