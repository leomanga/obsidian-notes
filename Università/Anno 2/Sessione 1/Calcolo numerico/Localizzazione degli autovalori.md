>[!thm] Gershgorin I
>Gli autovalori di $A\in \mathbb{C}^{n\times n}$ sono contenuti nell’unione
>$$\bigcup_{i=1}^{n}K_{i}:\quad K_{i}:=\{z\in \mathbb{C}:|z-a_{ii}|\le \sum_{j=1,j\not =i}|a_{ij}|\}$$
>$K_i$ si dice $i-$esimo cerchio di Gershgorin.

>[!Prp]
>Dato che $A$ e $A^{T}$ hanno gli stessi autovalori, il teorema si può applicare sia alle colonne che alle righe.
>Se chiamiamo $K_{i}$ il cerchio applicato alle righe e $H_{i}$ il cerchio applicato alle colonne, un autovalore $\lambda$ apparterrà all’unione
>$$\lambda\in(\bigcup_{i=1}^{n}K_{i})\bigcap(\bigcup_{i=1}^{n}H_{i})$$
>

>[!thm] Gershgorin II
>Sia $M_1$ l’unione di $k$ cerchi e $M_{2}$ l’unione dei restanti $n-k$. Se $M_{1}\cap M_{2}=\varnothing$ allora $k$ autovalori di $A$ appartengono ad $M_{1}$ e i restanti $n-k$ a $M_{2}$. 

>[!thm] Gershgorin III
>Sia $A$ [[Matrice irriducibile|irriducibile]] e sia $\lambda$ autovalore di $A$. Se $\lambda$ appartiene alla frontiera dell’unione dei cerchi di Gershgorin, allora $\lambda$ appartiene alla frontiera di tutti i cerchi.

