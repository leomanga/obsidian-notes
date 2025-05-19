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

Il condensatore è un elemento conservativo, immagazzina sotto forma di energia del campo elettrico tutta l’energia elettrica assorbita.

# Parte di elettrotecnica

>[!prp] Relazione costitutiva
>Da [[Materiali conduttori#Capacità]]
>$$q(t)=Cv(t)$$
>Allora, dato che $i(t)=\frac{dq(t)}{dt}$
>$$i(t)=C\cdot \frac{dv(t)}{dt}$$
>Oppure
>$$v(t)=v(0)+\frac{1}{C}\int_{0}^{t}i(\tau)d\tau$$

^bb070a

Dalla relazione costitutiva si vede che il condensatore è un elemento con memoria. Per conoscere $v(t)$ devo conoscere lo stato iniziale $v(0)$ e l’andamento di $i(t)$.

## Regime sinusoidale
Dalla sua [[#^bb070a]] si ha che
$$i(t)=C\frac{dv}{dt}=\frac{dq_c}{dt}$$
dove $q_{c}=Cv$ è la carica sulle sue armature.

Se applicassimo una tensione costante, avremo $i(t)=0$, quindi il condensatore si comporterà come circuito aperto.
Se applichiamo una tensione alternata sinusoidale del tipo $v(t)=V_{M}\cos(\omega t+\phi_v)$, avremo
$$i(t)=I_{M}\cos(\omega t+\phi _{i})=C\frac{dv}{dt}=\omega CV_{M}\sin(\omega t+\phi_v)= \omega CV_{M}\cos(\omega t+\phi_v+\frac{\pi}{2})$$
quindi $$I_{M} =\omega CV_M =\frac{V_M}{X_{c}} \quad \phi_{i}= \phi_{v}+\frac{\pi}{2}$$
dove $X_C$ è la [[Reattanza]]

>[!def] Relazione costitutiva nel dominio dei fasori
>[[Fasori]]
>$$\bar I = j\omega C\bar V=\frac{j}{X_{C}}\bar V= \frac{1}{\bar Z_{C}}\bar I$$
>$X_{C}$ è la [[Reattanza]].
>
>Si definisce da qui l’[[Impedenza]] e l’[[Ammettenza]] del condensatore
>
>