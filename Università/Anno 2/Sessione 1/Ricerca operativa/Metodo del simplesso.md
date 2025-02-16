Algoritmo per risolvere problemi di [[Programmazione lineare|PL]].
L’idea è quella di enumerare tutti i vertici del [[Poliedri|poliedro]] ed individuare il vertice che minimizza la funzione obiettivo corrispondente ad una soluzione ottima del problema.

Per capire se un vertice(ovvero una [[Poliedri#^166e60|SBA]]) è ottimo.
Nel caso peggiore devo guardare tutti i vertici, quindi dovrò compiere un numero $\#$ di iterazioni dell’ordine
$$\#=\binom{n}{m}$$
Questo è dato dalle combinazioni possibili di basi della matrice $A\in \mathbb{R}^{m\times n}$. 