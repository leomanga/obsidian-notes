I condensatori sono [[Materiali conduttori]], caratterizzati da:
- [[Materiali conduttori#Induzione elettrica]] completa
- Due superfici conduttrici affacciate
- Sistema isolato
- La quantità di carica sulle armature è uguale in valore assoluto
# Tipi
## Condensatore sferico
![[Condensatore sferico.excalidraw]]
Dato che questo conduttore è messo a terra avremo un [[Potenziale elettrostatico]] $V(R_{2})=V(R_{3})=0$
Invece $V(R_{1})-V(R_{2})?-\int_{R_{2}}^{R_{1}}k_{e}\frac{Q_{1}}{r^{2}}\hat{r}\cdot \hat{r}\cdot dr = k_{e}Q_{1}(\frac{R_{2}-R_{1}}{R_{1}R_{2}})$

Possiamo allora calcolare la [[Materiali conduttori#Capacità]]
$$c =4\pi\epsilon_{0}(\frac{R_{1}R_{2}}{R_{2}-R_{1}})$$
## Condensatore piano
![[Condensatore piano.excalidraw]]

Dato che in $V_{2}$ ho carica negativa, allora la differenza di [[Potenziale elettrostatico]] $\Delta V = V_{1}-V_{2}>0$.
Si ha uno sfrangiamento ai bordi, ma lo approssimiamo nullo, più $d<< a$, meno sfrangiamento avviene.
Abbiamo che 
$$\Delta V=\int_{0}^{d}\frac{\sigma}{\epsilon_{0}}(-\hat{z})\hat{z}\cdot dz=\frac{\sigma}{\epsilon_{0}}d$$
Allora abbiamo che la [[Materiali conduttori#Capacità]] è
$$c=\frac{\epsilon_{0}S}{d}$$
dove $S$ è la superficie del condensatore

## Condensatore cilindrico ideale
![[Condensatore cilindrico.excalidraw]]
La carica sarà
$$c=\frac{2\pi\epsilon_{0}L}{\ln[\frac{R_{2}}{R_{1}}]}$$


# Serie di condensatori
## Condensatori in parallelo
Dato che il sistema totale avrà una carica pari alla somma delle cariche nei condensatori $Q=Q_{1}+Q_{2}$, allora avremo che 
$$c_{tot}=\frac{Q}{\Delta V}=\frac{C_{1}\Delta V+C_{2}\Delta V}{\Delta V}=C_{1}+C_2$$
(ho usato la formula inversa per ottenere $Q_{1}$ e $Q_{2}$ da $C_{1}$ e $C_{2}$)

## Condensatori in serie
Dato che il sistema totale avrà la stessa carica dall’inizio alla fine, $Q_{1}=c\cdot \Delta V=c_{1}(V_{1}-V_{p})=C_{2}(V_{p}-V_{2})$
dove $V_{p}$ è il [[Potenziale elettrostatico]] in un punto in mezzo ai due condensatori.

Calcolando $\Delta V=V_{1}-V_{2}=V_{1}-V_{p}+V_{p}-V_{2}=\frac{Q_{1}}{c_{1}}+\frac{Q_{1}}{c_{2}}=Q_{1}\cdot (\frac{1}{c_{1}}+\frac{1}{c_{2}})$
Allora $$c=\frac{1}{(\frac{1}{c_{1}}+\frac{1}{c_{2}})}$$
# Calcolo del lavoro o energia per caricare un condensatore
In un sistema di cariche abbiamo visto il lavoro totale ![[Lavoro totale]]
Allora avrò che $$U=\frac{1}{2}QV_{1}-\frac{1}{2}QV_{2}=\frac{1}{2}Q\Delta V=\frac{1}{2}c(\Delta V)^{2}$$
Un’altra scrittura (guarda appunti 15/11/2024) è
$$U=\frac{1}{2}\epsilon_{0}E^{2}\cdot s\cdot d=u\cdot s\cdot d$$
Dove $E$ è il campo espresso in modulo, $s$ è la superficie del condensatore e $d$ è l’altezza del condensatore.(vale chiaramente per i [[#Condensatore piano|condensatori piani]])
$u=\frac{1}{2}\epsilon_{0}E^{2}\quad [\frac{J}{m^{2}}]$ è costante all’interno del condensatore e prende il nome di **densità di energia elettrostatica**.