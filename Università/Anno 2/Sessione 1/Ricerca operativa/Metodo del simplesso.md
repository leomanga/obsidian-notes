Algoritmo per risolvere problemi di [[Programmazione lineare|PL]].
L’idea è quella di enumerare tutti i vertici del [[Poliedri|poliedro]] ed individuare il vertice che minimizza la funzione obiettivo corrispondente ad una soluzione ottima del problema.

Per capire se un vertice(ovvero una [[Poliedri#^166e60|SBA]]) è ottimo.
Nel caso peggiore devo guardare tutti i vertici, quindi dovrò compiere un numero $\#$ di iterazioni dell’ordine
$$\#=\binom{n}{m}$$
Questo è dato dalle combinazioni possibili di basi della matrice $A\in \mathbb{R}^{m\times n}$. 

Costruisco il vettore dei costi, sia per le variabili in base, sia quelli per le variabili fuori base. Avrò $c=\begin{bmatrix}c_{b}\\c_{f}\end{bmatrix}$.

$$\begin{cases}c^T x=c_{b}^{T}x_{b}+c_{f}^{T}x_{f}=c_{b}^{T}(B^{-1}b-b^{-1}Fx_{f})+c_{f}^{T}x_{f}\\x_{b}=B^{-1}b-B^{-1}Fx_{f}\end{cases}$$
Quindi $$c^{T}x=c_{b}^{T}B^{-1}b+(c_{f}^{T}-c_{b}^{T}B^{-1}F)x_{f}$$
Prendendo vertici, avrò che $x_{f}=0$, quindi $c^T x=c_{B}^{T}B^{-1}b$

>[!prp]
>Data una soluzione ammissibile associata ad una certa base $B$, allora $x$ è ottima per il problema di $PL$ se il vettore dei costi ridotti è non negativo.
>Il vettore dei costi ridotti è definito come
>$$\bar{c}_f^{T}=c_{f}^{T}-c_{b}^{T}B^{-1}F$$
>