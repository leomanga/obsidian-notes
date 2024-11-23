---
aliases:
  - potenza di calore trasmesso
---
Il flusso di calore è la misura della velocità con cui avviene uno scambio di energia [[Calore]].

$$\dot Q=\frac{\delta Q}{dt}=\frac{Q}{\Delta t}\quad \left[\frac{J}{s}\right]=[W]$$

dove $Q$ è il [[Calore]], $\Delta t$ il [[Tempo]].
$W$ sono i Watt, $J$ i Joule e $s$ i secondi. 

# Caso della [[Conduzione termica]]
Il flusso di calore può essere riscritto tramite l'equazione di Fourier, ![[Conduzione termica#^065013]] e possiamo definire il flusso specifico per unità di superficie, ![[Conduzione termica#^90a6c7]]

## Esempio
Si consideri una geometria di due sistemi piani posti a contatto, aventi spessore $L_{1}$ e $L_{2}$ e coefficienti di conduzione $\lambda_1$ e $\lambda_{2}$.
Si consideri una temperatura alle estremità della geometria di $T_1$ e $T_{2}$ misurata rispettivamente sulla superficie esterna del sistema $1$ e $2$.
Si consideri con $T$ la temperatura all'interfaccia di contatto dei due sistemi.
![[Convezione esempio.png]]

Ipotizziamo $T_{2}>T_{1}$, allora:
$$\dot Q_{1}=\lambda_{1}\cdot A\cdot\frac{T-T_{1}}{L_{1}}\qquad \dot Q_{2}=\lambda_{2}\cdot A\cdot\frac{T_{2}-T}{L_{2}}$$
Il flusso di energia sarà tale che $$\dot Q_{1}=\dot Q_{2}$$
Allora
$$
\lambda_{2}\cdot\frac{T-T_{1}}{L_{1}}=\lambda_{2}\cdot\frac{T-T_{2}}{L_{2}}
$$
Raccogliendo e semplificando otterremo che
$$
T=\frac{\lambda_{1}\cdot L_{2}\cdot T_{1}+\lambda_{2}\cdot L_{1}\cdot T_{2}}{\lambda_{1}\cdot L_{2}+\lambda_{2}\cdot L_{1}}

$$
Inoltre, sostituendo $T$ in [[Conduzione termica#^90a6c7]], otteniamo anche che
$$
\dot q_{1}=\lambda_{1}\cdot \lambda_{2}\cdot\left(\frac{T_{2}-T_{1}}{\lambda_{1}\cdot L_{2}+\lambda_{2}\cdot L_{1}}\right)
$$
Possiamo inoltre ottenere l'espressione del flusso di energia trasferito per [[Conduzione termica]] attraverso due generici sistemi a geometria piana
$$
\dot q_{2}=\dot q_{1}=\dot q =\frac{T_{2}-T_{1}}{\frac{L_2}{\lambda 2}+\frac{L_1}{\lambda 1}}
$$
# Caso della [[Convezione termica]]
Il flusso di calore può essere riscritto tramite la legge di Newton della convezione
![[Convezione termica#^386aa6]]
e possiamo definire il flusso per unità di superficie
![[Convezione termica#^499a82]]
