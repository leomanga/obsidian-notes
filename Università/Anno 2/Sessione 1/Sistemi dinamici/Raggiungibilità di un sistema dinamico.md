>[!def] Raggiungibilità in un sistema dinamico a tempo discreto
>Uno stato si dice raggiungibile in $k$ passi (dallo stato zero), se assumendo $x(0)=0$, esiste una sequenza di passi $u(0),u(1),\ldots,u(k-1)$ tale che $x(k)=\bar x$.

## Studio della raggiungibilità | problema del controllo
Dato un sistema [[Sistemi lineari tempoinvarianti|LTI]] a tempo discreto
$$\begin{cases}
x(k+1)=Ax(k)+Bu(k)\\ 
y(k)=Cx(k)+Du(k)\\
x(0)=x_{ini}
\end{cases}$$
Noi cerchiamo per un certo $T$, $x(T)=x_{fin}$. 
Lo scopo è quello di determinare, se possibile, la sequenza di ingressi $u(0),u(1),\ldots,u(T-1)$ tale da portare lo stato da $x_{ini}$ a $x_{fin}$.
Da [[Analisi modale nello spazio degli stati per sistemi a tempo discreto]] abbiamo che
$$x(k)=x_{l}(k)+x_{f}(k)=A^{k}x(0)+\sum_{i=0}^{k-1}A^{k-1-i}Bu(i)$$

Possiamo imporre $$A^{T}x_{ini}+\sum_{i=0}^{T-1}A^{T-1-i}Bu(t)=x_{fin}$$
Riscrivendo in forma matriciale abbiamo
$$\underbrace{\begin{bmatrix}
B&&AB&&A^{2}B\ \cdots \ A^{T-1}B
\end{bmatrix}}_{\mathcal{R}_{T}}
\begin{bmatrix}
u(T-1) \\ u(T-2) \\ \vdots  \\ u(0)
\end{bmatrix}=x_{fin}-A^{T}x_{ini}$$
dove $x\in \mathbb{R}^{n}$, $u\in \mathbb{R}^{m}$ e $\mathcal{R}_{T}\in \mathbb{R}^{n\times Tm}$ e viene definita

>[!def] Matrice di raggiungibilità in $T$ passi
>La matrice di raggiungibilità è la matrice 
>$$\mathcal{R}_{T}=\begin{bmatrix}
B&&AB&&A^{2}B\ \cdots \ A^{T-1}B
\end{bmatrix}$$

Dal [[Teorema di Rouchè-Capelli]], il problema ammette soluzione se e solo se 
$$x_{fin}-A^{T}x_{ini}\in Im(\mathcal{R}_{T})$$
(Se non appartenesse all’immagine, la matrice completa avrebbe un rango maggiore di quella incompleta e il sistema non sarebbe risolubile)

>[!def] Stato raggiungibile in $k$ passi
>Uno stato $\bar x\in \mathbb{R}^{n}$ si dice raggiungibile in $k$ passi (dallo stato zero) se, assumendo $x(0)=0$, esiste una sequenza di ingressui $u(0), u(1),\ldots,u(k-1)$ tale che $x(k)=\bar x$.

^f26ad0

>[!prp]
>Lo stato $\bar x$ è [[#^f26ad0|raggiungibile in $k$ passi]] 