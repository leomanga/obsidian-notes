Dato un problema di [[Programmazione lineare|PL]] in forma standard [[Programmazione lineare#^0dd399]], definiamo il problema duale il PL:
$$\begin{split}
\max b^{T}y\\
A^{T}y\le c
\end{split}$$
dove $b$ è il vettore per cui $g_{j}\le b_{j}$ ecc.. nel caso primale.
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

^7f9174

>[!thm]
>Dato un problema di PL, il duale del problema duale coincide con il primale

^a1029e

>[!thm]
>Si consideri una coppia primale-duale di problemi di PL, e siano $\bar x$ e $\bar y$ soluzioni ammissibili dei problemi rispettivamente, allora
>$$c^{T}\bar x\ge b^{T}\bar y$$
>(il valore della funzione obiettivo del problema primale è sempre maggiore o uguale del valore della funzione obiettivo del problema duale)

>[!thm] Teorema della dualità forte
>Siano $\bar x$ e $\bar y$ soluzioni ammissibili per una coppia primale-duale di problemi di PL.
>Se $c^{T}\bar x= b^{T} \bar y$, allora $\bar x$ e $\bar y$ sono ottime per i rispettivi problemi.

^37bcdf

A questo punto possiamo chiudere il cerchio. Infatti, dato un problema di PL (primale)
in forma standard:
1. Se $x^*$ e una soluzione ottima del problema primale, allora da [[Programmazione lineare#^41dcfd]], deve soddisfare le [[Condizioni di Karush-Kuhn-Tucker|KKT]]
2. Se un punto $x^*$ soddisfa le [[Condizioni di Karush-Kuhn-Tucker|KKT]], allora il vettore $u^∗$ dei moltiplicatori è ammissibile per il problema duale ([[#^7f9174]]) ed e tale che $c^{T}x^{∗} = b^{T}u^{∗}$ ([[#^a1029e]]);
3. Se $x^{∗}$ e $u^{∗}$ sono ammissibili per i rispettivi problemi e si ha che $c^{T}x^{∗} = b^{T}u^{∗}$, allora $x^∗$ e $u^∗$ sono una coppia di soluzioni ottime per i rispettivi problemi ([[#^37bcdf]]).

In definitiva, sono equivalenti le seguenti affermazioni
- $x^{*}$ è un punto di minimo (globale)
- esiste un vettore $u^{*}$ tale che sono soddisfatte le [[Programmazione lineare#^533680]] 
- esiste un vettore $u^{*}$, ammissibile per il problema duale, tale che $c^{T}x^{*}=b^{T}u^{*}$

>[!thm]
>Se in una coppia primale-duale di problemi [[Programmazione lineare|PL]], uno dei due problemi è illimitato, l’altro non ammette soluzione ammissibile.