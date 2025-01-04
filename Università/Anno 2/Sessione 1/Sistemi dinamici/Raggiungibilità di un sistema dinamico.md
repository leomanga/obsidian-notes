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

