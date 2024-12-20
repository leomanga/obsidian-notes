![[Generatore di forza elettromotrice.excalidraw]]

Se voglio mantenere costante la [[Corrente elettrica]] all’interno di un [[Materiali conduttori|conduttore]], dobbiamo fare in modo che il [[Campo elettrostatico]] all’interno del conduttore sia costante.
Il campo elettrico totale, in questo caso non sarà conservativo, dato che viene prelevata un po’ di energia dalle cariche in moto, ad esempio dall’effetto Joule ([[Resistenze#^2b0c5c]]). Allora
$$\oint \vec{E}\cdot d\vec{l}\not = 0$$
Per mantenere correnti stazionarie, dobbiamo poter generare un campo elettrostatico $\vec{E}_{e}$ non conservativo, che porti le cariche dal punto a potenziale più basso a quello più alto. $\vec{E}_{e}$ è detto **campo elettromotore**.
(Il campo elettrostatico $\vec{E}_{s}$ invece è per sua natura conservativo)

Possiamo definire ora
>[!def] Forza elettromotrice
>$$f = \int_{A}^{B}\vec{E}_{e}\cdot d\vec{l}\quad [V]$$
>La forza elettromotrice rappresenta il lavoro fatto dal campo elettromotore per  spostare una carica positiva unitaria dal morsetto negativo a quello positivo.
>

Possiamo quindi trovare la caduta di potenziale totale attraverso il circuito chiuso
Abbiamo che
$$\oint_{C}\vec{E}\cdot d\vec{l}=RI+rI\Rightarrow f=RI+rI=\Delta V+rI$$
Dove $R$ è la [[Resistenze|resistenza]] esterna (del circuito) e $r$ è quella interna al generatore.
La caduta di potenziale del circuito sarà allora 
$$
\Delta V_{AB}=f+rI=\epsilon+rI
$$

^862722

$f$ talvolta viene scritta come $\epsilon$ che rappresenta la tensione ideale.

Possiamo schematizzare un circuito composto da un generatore di tensione e da una resistenza come

![[Circuito con generatore.excalidraw]]

Supponiamo di avere questo ramo di un circuito

![[Ramo di un circuito.excalidraw]]

Posso calcolare la differenza di potenziale ai capi del circuito, usando [[#^862722]]
$$V_{A}-V_{B}=R_{1}I -\epsilon_{1} +R_{2}I+R_{3}I+\epsilon_{2}$$

