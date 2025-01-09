Notazioni:
In questo documento $T$ viene usata come numero, quindi $A^{T}$ è una matrice elevata alla $T$. Per il simbolo del trasposto si usa $'$.

--- 

>[!def] Non osservabilità in un sistema dinamico a tempo discreto
> Uno stato $\bar x \in \mathbb{R}^{n}$ si dice non osservabile (o indistinguibile dallo stato nullo) in $k$ passi se, ponendo $x(0)=\bar{x}$ si ottiene la risposta libera $$y(0)=y(1)=\ldots=y(k-1)=0$$

## Calcolo degli stati non osservabili
Da [[Analisi modale nello spazio degli stati per sistemi a tempo discreto]] abbiamo che
$$x_{l}(k)=A^{k}\cdot x(0)=A^{k}\cdot \bar x$$
Allora la risposta libera nell’uscita sarà
$$y_{l}(k)=C\cdot x_{l}(k)=C\cdot A^{k}\cdot \bar x$$
Per verificare che gli stati non siano osservabili dovremo imporre
$$\begin{cases}y(0)=C\cdot\bar x=0\\y(1)=C\cdot A\cdot \bar x=0\\\vdots\\y(k-1)=C\cdot A^{k-1}\cdot \bar x=0\end{cases}$$
In forma matriciale avremo
$$\underbrace{\begin{bmatrix}C\\CA\\CA^{2}\\\vdots\\CA^{k-1}\end{bmatrix}}_{\mathcal{O}_{k}}\cdot \bar x=0\iff\mathcal{O}_{k}\cdot\bar x=0$$
dove $\bar x\in \mathbb{R}^{n}$, $y\in \mathbb{R}^{p}$ $\mathcal{O}_{k}\in \mathbb{R}^{pk\times n}$
 
>[!def] Matrice di osservabilità in $k$ passi
>La matrice di osservabilità in $k$ passi è la matrice $\mathcal{O}_{k}\in \mathbb{R}^{pk\times n}$
>$$\mathcal{O}_{k}=\begin{bmatrix}C\\CA\\CA^{2}\\\vdots\\CA^{k-1}\end{bmatrix}$$

^1f21d3

## Studio dell’osservabilità | problema della ricostruzione dello stato iniziale
Dato un sistema [[Sistemi lineari tempoinvarianti|LTI]] a tempo discreto
$$\begin{cases}
x(k+1)=Ax(k)+Bu(k)\\ 
y(k)=Cx(k)+Du(k)\\
\end{cases}$$
Cerchiamo di ricostruire $x(0)$ leggendo l’uscita $y(0),y(1),\ldots, y(k-1)$

Avendo definito [[#^1f21d3]] vogliamo che
$$\begin{bmatrix}y(0)\\y(1)\\\vdots\\y(k-1)\end{bmatrix}=\begin{bmatrix}C\\CA\\CA^{2}\\\vdots\\CA^{k-1}\end{bmatrix}\cdot x(0)=\mathcal{O}_{k}\cdot x(0)$$
Dal [[Teorema di Rouchè-Capelli]], il problema ammette unica soluzione solo se $rank(\mathcal{O}_{k})=n$, allora da [[Teorema di nullità + rango]], avremo che ciò è vero se e solo se $\ker\mathcal{O}_{k}=0$.

Possiamo definire il sottospazio
>[!def] Insieme degli stati non osservabili in $k$ passi
>$$\mathcal{X}_{k}^{no}=\ker\mathcal{O}_{k} $$

Quindi il sottospazio osservabile in $1$ passo sarà$$\mathcal{X}_{1}^{no}=\ker\mathcal{O}_{1}=\ker[C]$$
quello osservabile in due passi sarà
$$\mathcal{X}_{2}^{no}=\ker\mathcal{O}_{2}=\ker\begin{bmatrix}C\\CA\end{bmatrix}\subseteq\mathcal{X_{1}^{no}}$$
e così via.
In generale avremo che 
$$\mathcal{X}_{1}^{no}\supseteq\mathcal{X}_{2}^{no }\supseteq\ldots\supseteq\mathcal{X}_{k}^{no }\supseteq\mathcal{X}_{k+1}^{no }\supseteq\ldots$$
>[!def] Sistema completamente osservabile
>Un sistema si dice completamente osservabile se $$\exists\bar k:\mathcal{X}_{\bar k}^{no}=0$$
>ovvero
>$$\ker \mathcal{O}_{k}=0\iff rank(\mathcal{O}_{k})=n$$
>

Per il [[Raggiungibilità di un sistema dinamico#^6af30f|teorema di Caley-Hamilton]], allora $CA^{n}$ è combinazione lineare di $C,CA,CA^{2}\ldots CA^{n-1}$
allora $$\mathcal{X}_{n+h}^{no}=\mathcal X_{n}^{no}\quad \forall h>0$$
Allora
>[!prp] Insieme degli stati osservabili in un qualunque numero di passi
>L’insieme degli stati osservabili in un qualunque numero di passi coincide con
>$$\mathcal{X}^{no}=\ker \mathcal{O}_{n}$$

>[!def] Matrice di osservabilità del sistema
>$$\mathcal{O}=\mathcal{O}_{n}=\begin{bmatrix}C\\CA\\CA^{2}\\\vdots\\CA^{n-1}\end{bmatrix}$$
