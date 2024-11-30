Cerchiamo trovare una funzione di trasferimento totale $G(s)$ dati una serie di sistemi dinamici connessi fra loro.
# Interconnessione in serie
![[Sistema dinamico in serie.excalidraw]]

In questo caso avremo che 
$$
\begin{cases}Y_{1}(s) = G_{1}(s) \cdot U_{1}(s) \\Y_{2}(s)=G_{2}(s)\cdot U_{2}(s) \\U_{2}(s)=Y_{1}(s) \end{cases}
$$
Allora avremo che 
$$Y_{2}(s)=\underbrace{G_{2}(s)\cdot G_{1}(s)}_{G(s)}\cdot U_{1}(s)$$
In generale allora 
$$G(s)=(G_{n}(s)\cdot G_{n-1}(s)\cdot\ldots\cdot G_{1}(s))$$
(Nota che potendo le $G_{i}$ essere matrici, allora è importante l’ordine di moltiplicazione)
# Interconnessione in serie
![[Sistema dinamico in parallelo.excalidraw]]

Il punto $D$ in figura prende il nome di **punto di derivazione**. 
Il punto $S$ in figura prende il nome di **sommatore**.

In questo caso avremo
$$\begin{cases}
Y_{1}(s)=G_{1}(s)\cdot U_{1}(s)\\ Y_{2}(s)=G_{2}(s)\cdot U_{2}(s)\\
U_{1}(s)=U(s)\\
U_{2}(s)=U(s)\\
Y(s)=Y_{1}(s)+Y_{2}(s)\end{cases}$$
Allora avremo che
$$
Y(s)=\underbrace{[G_{1}(s)+G_{2}(s)]}_{G(s)}U(s)
$$

In generale allora

$$G(s)=G_{1}(s)\pm G_{2}(s)\ldots \pm G_{n}(s)$$
# Interconnessione in retroazione
![[Sistema dinamico in retroazione.excalidraw]]

La retroazione può essere **positiva** o **negativa** in base all’operazione fatta fra $r$ e $y_{2}$.

In questo caso avremo (guarda appunti per il procedimento)

$$Y(s)=\underbrace{[I\mp G_{1}(s)\cdot G_{2}(s)]^{-1}\cdot G_{1}(s)}_{G(s)}\cdot R(s)$$
(se la retroazione è positiva avremo segno “$-$”, sennò segno “$+$”)