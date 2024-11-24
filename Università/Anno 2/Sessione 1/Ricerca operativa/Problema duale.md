Dato un problema di [[Programmazione lineare|PL]] in forma standard [[Programmazione lineare#^0dd399]], definiamo il problema duale il PL:
$$\begin{split}
\max b^{T}y\\
A^{T}y\le c
\end{split}$$
Se uniamo di due problemi avremo la lagrangiana
$$L(y,v)=-b^{T}y-v^{T}(c-A^{T}y)$$
dove la funzione obiettivo è cambiata di segno data la massimizzazione.
Le [[Condizioni di Karush-Kuhn-Tucker]] saranno
$$\begin{split}
Av^{*}=b\\
c^{T}-y^{*T}A\ge 0\\
v^{*}\ge 0\\
(c^T-y^{*T}A)v^{*}=0\quad \forall j=1,\ldots,n
\end{split}$$

^655736

>[!thm] 
>Dato un problema di PL, se e solo se esistono una soluzione $x^{*}$ ammissibile e un vettore $u^{*}$ tale da soddisfare il problema in forma standard, allora esistono un vettore $y^{*}$ ammissibile per il problema duale e un vettore $v^{*}$ tali da soddisfare [[#^655736]]

>[!thm]
>Dato un problema di PL, il duale del problema duale coincide con il primale

>[!thm]
>Si consideri una coppia primale-duale di problemi di PL, e siano $\bar x$ e $\bar y$ soluzioni ammissibili dei problemi rispettivamente, allora
>$$c^{T}\bar x\ge b^{T}\bar y$$
>(il valore della funzione obiettivo del problema primale è sempre maggiore o uguale del valore della funzione obiettivo del problema duale)

>[!thm]
>Siano $\bar x$ e $\bar y$ soluzioni ammissibili per una coppia primale-duale di problemi di PL.
>Se $c^{T}\bar x= b^{T} \bar y$, allora $\bar x$ e $\bar y$ sono ottime per i rispettivi problemi.

A questo punto possiamo chiudere il cerchio. Infatti, dato un problema di PL (primale)
in forma standard:
1. Se $ x^*$ `e una soluzione ottima del problema primale, allora (Teorema 4) deve soddis-
fare le KKT;
2. Se un punto x∗ soddisfa le KKT, allora il vettore u∗ dei moltiplicatori `e ammissibile
per il problema duale (Teorema 6) ed `e tale che cTx∗ = bTu∗ (Teorema 5);
3. Se x∗ e u∗ sono ammissibili per i rispettivi problemi e si ha che cTx∗ = bTu∗, allora
x∗ e u∗ sono una coppia di soluzioni ottime per i rispettivi problemi (Teorema 9).