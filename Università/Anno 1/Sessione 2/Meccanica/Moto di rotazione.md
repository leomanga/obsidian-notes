---
collegamenti:
  - "[[Capitolo 9 - Corpi rigidi]]"
---
In un moto di rotazione, tutti i punti si muovono di [[Moto circolare]] con la stessa velocità angolare $\omega$. 
La direzione di $\omega$ è quella dell'asse di rotazione, fisso.
Per lo studio di questo moto ci concentriamo sull'equazione ([[Capitolo 8 - Sistemi di punti materiali#^a907c0|*]]) $$\vec{M}=\frac{d\vec{L}}{dt}$$
dove $\vec{M}$ è il momento delle forze esterne calcolato rispetto ad un determinato polo, che per semplicità verrà preso sull'asse di rotazione.
$\vec{L}$ è il momento angolare del corpo, calcolato sempre rispetto allo stesso polo scelto per $\vec{M}$.

Inoltre, dato che $\omega$ può cambiare in modulo, dobbiamo definire il vettore accelerazione angolare $$\alpha = \frac{d\omega}{dt}$$
$\alpha$ avrà stessa direzione di $\omega$.

Avremo che $\vec{a}_{ni}$, ovvero l'accelerazione normale del punto $i-$esimo sarà $$\vec{a}_{ni}=\omega \times \omega \times \vec{r}_{ni}=-\omega \vec{r}_{ni}$$
mentre $\vec{a}_{ti}$, ovvero l'accelerazione tangenziale sarà pari a
$$\vec{a}_{ti}=\vec{\alpha}\times \vec{r}_{ni}$$
([[Capitolo 7 - Cinematica dei moti relativi#^a59d9e]])


Vogliamo ora calcolare il momento angolare di una generica particella che costituisce il corpo rigido.
Definiamo $\theta_{i}$, l'angolo tra l'asse $\vec{r}_{i}$ e l'asse di rotazione $\vec{z}$.

Dalla definizione di momento angolare
$$\vec{L}_{i}=\vec{r}_{i}\times m_{i}\vec{v}_{i}$$
da cui deduciamo che $\vec{L}_{i}$ è perpendicolare a $\vec{r}_{i}$ e $\vec{v}_{i}$.
Ci possiamo calcolare la componente sull'asse $z$, 
>[!def] Componente di $\vec{L}_{i}$ sull'asse $z$
>$$L_{iz}=m_{i}R^{2}_{i}\omega$$ (vedi pag 61).

Inoltre, per l'intero corpo rigido, costituito da $n$ punti discreti, $$\vec{L} = \sum_{i=1}^{n}\vec{L}_{i}=\sum_{i=1}^{n}\vec{r}_{i}\times m_{i}\vec{v}_{i}$$
Calcolando $\vec{L}$ lungo l'asse di rotazione otteniamo
$$L_{z}=I_{z}\omega$$ (vedi pag 62)
dove $I_z$ è il momento di inerzia del corpo rigido rispetto all'asse $z$.
>[!def] Momento di inerzia del corpo rigido
>$$I_{z}=\sum_{i=1}^{n}m_{i}R^{2}_{i}=\sum_{i=1}^{n}m_{i}(x_{i}^{2}+y_{i}^{2})$$

^a5ff25

Inoltre possiamo calcolare la proiezione di $\vec{L}_{i}$ in direzione perpendicolare all'asse $z$.
>[!def] Componente di $\vec{L}_{i}$ in direzione perpendicolare all'asse $z$
$$L_{i\perp}=r_{i}m_{i}R_{i}\omega\cos\theta_{i}$$

Esistono casi in cui $\vec{L}$ è parallelo a $\vec{\omega}$, ad esempio se l'asse di rotazione è un asse di simmetria.

>[!def] Moto di precessione
>Si parla di moto di precessione quando $\vec{L}$ non è parallelo a $\omega$.
>Inoltre se $\omega$ è costante si parla di precessione uniforme. In questo caso avremo $$\vec{M}=\frac{d\vec{L}}{dt}=\omega\times L$$

 >[!def] Energia cinetica nel moto di rotazione
 >$$E_{k}= \sum_{i=1}^{n} \frac{1}{2}m_{i}v_{i}^2=\sum_{i=1}^{n} \frac{1}{2}m_{i}R_{i}^2\omega^{2}=\frac{1}{2}I_{z}\omega^{2}$$

^a759cd

Ricordandoci che $W=\Delta E_{k}$, dove $W$ è il [[Lavoro]], allora 
$$W=\int_{\theta_{in}}^{\theta_{fin}}Md\theta$$
Dimostrazione a pag 76
>[!def] Potenza
>$$P = \frac{dW}{dt}=M\omega$$
>

>[!thm] Teorema di Huygens
>Il momento di inerzia dipende dalle caratteristiche del corpo come la geometria, la densità e la posizione dell'asse di rotazione.
>Il momento di inerzia inoltre è sicuramente un valore positivo.
>Il momento di inerzia rispetto ad un asse $\vec{u}$ è pari a 
>$$I_{u}=I_{x}u_{x}^{2}+I_{y}u_{y}^{2}+I_{z}u_{z}^{2}-2I_{xy}u_{x}u_{y}-2I_{yz}u_{y}u_{z}-2I_{xz}u_{x}u_{z}$$
>Dove $I_{x},I_{y},I_{z}$ sono i momenti di inerzia rispetto agli assi $x,y,z$, mentre $I_{xy},I_{yz},I_{xz}$ sono i cosiddetti momenti di inerzia centrifughi
>$$I_{xy}=\sum_{i=1}^{n}m_{i}x_{i}y_{i}$$
>$$I_{yz}=\sum_{i=1}^{n}m_{i}y_{i}z_{i}$$
>$$I_{xz}=\sum_{i=1}^{n}m_{i}x_{i}z_{i}$$
>Possiamo calcolare le componenti cartesiane del momento angolare come il risultato del prodotto matrice vettore $$\vec{L}=[\vec{I}]\vec{\omega}$$
>dove $$[\vec{I}]=\begin{bmatrix}I_{x}& -I_{xy}&-I_{xy}\\
-I_{xy}&I_{y}&-I_{yz}\\
-I_{xz}&-I_{yz}&I_{z}\end{bmatrix}$$
>

>[!def] Energia cinetica in generale
>Abbiamo  già calcolato l'[[#^a759cd|energia cinetica]] nel caso in cui $\vec{I}$ fosse parallelo all'asse di rotazione $z$. In generale, però:
>$$E_{k} = \vec{\omega}\cdot \vec{L}$$
>

^5ff6dc
