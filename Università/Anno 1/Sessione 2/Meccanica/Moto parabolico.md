---
collegamenti:
  - "[[Capitolo 4 - Cinematica moti bidimensionali]]"
---
Analizziamo il moto di un punto materiale $P$ lanciato con una velocità iniziale $v_{0}$che forma un angolo $\vartheta$ con il piano orizzontale dall'origine $O$ di un sistema di riferimento cartesiano con asse $x$ orizzontale e asse $y$ verticale ascendente, tali che il piano $xy$ contiene il vettore $v_0$. 
![[Moto parabolico.png]]

# Componenti della velocità
Rispetto a questo sistema di riferimento, le componenti della [[Velocità#Rappresentazione con coordinate cartesiane|Velocità]] iniziale sono
$$v_{0}=v_{0x}\vec{i}+v_{0y}\vec{j}$$
dove
$$\begin{split}
&v_{0x}=v_{0}\cos\vartheta\\ &v_{0y}=v_{0}\sin\vartheta
\end{split}$$

^34377c

# Accelerazione nel tempo
Il punto materiale inoltre è soggetto ad un'[[Accelerazione#Accelerazione in 2 dimensioni|accelerazione]] costante$$\vec{a}=-g\vec{j}$$
# Velocità nel tempo
Possiamo calcolare la velocità, conoscendo l'accelerazione, tramite un'integrazione nel tempo.
$$\vec{v}=\vec{v}_{0}+\int_{0}^{t}\vec{a}(t)dt$$
Considerando le componenti cartesiane:
$$
\begin{split}&v_{x}=v_{0x}+\int_{0}^{t}0\ dt=v_{0x}\\&v_{y}=v_{0x}-\int_{0}^{t}g\ dt=v_{0y}-gt
\end{split}
$$

^5808d5

Possiamo notare come la componente orizzontale sia costante e quella verticale vari nel tempo con coefficiente angolare $-g$.
# Posizione nel tempo
Possiamo integrare la velocità per ottenere la posizione, tenendo conto della posizione iniziale.
$$\vec{r}=\vec{r}_{0}+\int_{0}^{t}v(t)\ dt$$
Considerando le componenti cartesiane:
$$
x_{0}+\int_{0}^{t}v_{x}\ dt=x_{0}+v_{x}t
$$

$$
y=y_{0}+\int_{0}^{t}v_{y}\ dt=y_{0}+\int_{0}^{t}(v_{0y}-gt)dt=y_{0}+v_{0y}t-\frac{1}{2}gt^{2}
$$

^9465fa

Possiamo analizzare i risultati, ricordando che![[#^34377c]]
 possiamo scrivere 
 $$
 x(t)= \underbrace{v_{0}\cos\vartheta}_{v_{0x}} t
$$

^0d0c1b

 $$
 y(t)=\underbrace{v_{0}\sin\vartheta}_{v_{0y}} t-\frac{1}{2}gt^{2}
$$

^f746d7

Notiamo che [[#^0d0c1b]] varia nel tempo con legge lineare, con coefficiente angolare $v_{0x}=v_{0}cos\vartheta$, mentre notiamo come [[#^f746d7]] varia nel tempo secondo un polinomio di secondo grado, quindi segue una parabola.
![[componenti posizione moto parabolico.png]]

> [!claim] Quota massima
>La quota del punto raggiunge il valore massimo quando $v_{y}$ si annulla, quindi nel tempo
>$$
>t_{M}=\frac{v_{0y}}{g} =\frac{v_{0}\sin\vartheta}{g}
>$$
>Sostituendolo nell'espressione $y(t)$ otteniamo $$y_{M}=\frac{1}{2}\frac{v_{0}^{2}\sin^{2}(\vartheta)}{g}$$ovvero l'altezza massima raggiunta.
>Sostituendo invece nell'espressione $x(t)$ otteniamo$$x_{M}=\frac{v_{0}^{2}\sin\vartheta \cos\vartheta}{g}$$
>ovvero la lunghezza massima raggiunta.

^d25522

> [!Clm] Gittata massima
> Il punto raggiunge la sua massima distanza quando $y=0$, allora basta risolvere l'equazione di secondo grado [[#^9465fa]] con $y=0$ e ipotizzando $y_{0}=0$.
> Le due soluzioni saranno $t=t_{0}=0$, dato che $y(0)=0$ e $$t=t_{G}=2\frac{v_{0y}}{g}=2\frac{v_{0}\sin\vartheta}{g}$$
>Sostituendo nell'espressione $x(t)$ otteniamo
> $$x_{G}=2\frac{v_{0}^{2}\sin\vartheta\cos\vartheta}{g}$$

^082030

> [!proposition] Il tempo di gittata massima è due volte quello di volo
>Ricordando, da [[#^d25522]], che $t_{M}=\frac{v_{0}\sin\vartheta}{g}$ e da [[#^082030]] che $t_{G}=2\frac{v_{0}\sin\vartheta}{g}$, è intuitivo verificare che $t_{G}=2t_{M}$
>

 > [!proposition] La distanza percorsa durante il tempo di gittata massima è due volte quella percorsa durante il tempo di volo
>Ricordando, da [[#^d25522]], che $x_{M}=\frac{v_{0}^{2}\sin\vartheta \cos\vartheta}{g}$ e da [[#^082030]] che $x_{G}=2\frac{v_{0}^{2}\sin\vartheta\cos\vartheta}{g}$, è intuitivo verificare che $x_{G}=2x_{M}$
>

# Traiettoria
Per descrivere la traiettoria dobbiamo cercare una relazione che lega tra loro le componenti cartesiane, quindi scrivere $$y(x).$$
Possiamo esplicitare il tempo dall'espressione [[#^0d0c1b]]:
$$
t = \frac{x}{v_{0x}}
$$
Lo sostituiamo nell'espressione [[#^f746d7]] ed otteniamo
> [!clm] Descrizione della traiettoria del punto
> $$
> \begin{align}y(x)&=v_{0y}\frac{x}{v_{0x}}-\frac{1}{2}g\left(\frac{x}{v_{0x}}\right)^{2}\\
> &=\frac{\sin\vartheta}{\cos\vartheta}x-\frac{1}{2}g\left(\frac{x}{v_{0}\cos\vartheta}\right)^2\\&=\tan\vartheta\ x-\frac{1}{2}g\left(\frac{x}{v_{0}\cos\vartheta}\right)^2
> \end{align}
> $$

^de7afc

Dati $v_{0}$ e $\vartheta$, possiamo notare come questa sia l'equazione di una parabola, da cui il nome del moto.

> [!rmk] Se derivo la traiettoria ottengo i risultati precedenti
> La quota massima, basandoci su [[#^de7afc]], si raggiunge quando $\frac{dy}{dx}=0$.
> Facendo i dovuti calcoli, troveremo il valore $x_M$, per il quale si annulla la derivata e a cui corrisponde l'altezza massima $y_{M}$, che hanno come equazioni le stesse trovate in [[#^d25522]].
>[!prp] Velocità al momento dell'impatto

>[!prp] Velocità al momento dell'impatto
>Ricordandoci [[#^5808d5]] e da [[#^082030]], il tempo di volo, sostituendo a $t,t_{G}$, otteniamo che la velocità al momento dell'impatto sarà uguale a
>$$\begin{align}
>v_{Gy}&=v_{0y}-2g\frac{v_{0y}}{g}\\&=-v_{0y}\\&=-v_{0}\sin\vartheta
>\end{align}$$
>


 














