>[!def] Calcolo superficie
>Dati due vettori $a,b\in \mathbb{R}^{3}$ denotiamo con
>$$a \wedge b=\underbrace{a\times b
}_{prodotto\ vettoriale}=(a_{2}b_{3}-a_{3}b_{2},a_{3}b_{1}-a_{1}b_{3}, a_{1}b_{2}-a_{2}b_{1})$$
$a=(a_{1},a_{2},a_{3})\qquad b=(b_{1},b_{2},b_{3})$
$\Rightarrow a\wedge b\in \mathbb{R}^{3}$

>[!clm]
>Per ricordarsi $a\wedge b$ si può calcolare il [[Determinante di M|determinante]] 
>$$a\wedge b= det\begin{pmatrix}  a_{1} & a_{2} & a_{3} \\ 
>b_{1} & b_{2} & b_{3}\\
>i & j & k\end{pmatrix}=\begin{split}&i(a_{2}b_{3}-b_{2}a_{3})+\\&j(a_{3}b_{1}-a_{1}b_{3})+\\
>&k(a_{1}b_{2}-a_{2}b_{1})\end{split}$$

>[!prp] Alcune proprietà
>1) $a\wedge b=-b\wedge a$
>2) $\forall \lambda \in \mathbb{R}\Rightarrow (\lambda a)\wedge b= \lambda(a\wedge b)$. 
>   Come conseguenza $a\wedge a = (0,0,0),\quad \lambda a\wedge a=(0,0,0)$. Allora se $a$ e $b$ sono paralleli, $a\wedge b=(0,0,0)$
>3) $a\wedge b=0\Rightarrow a$ e $b$ sono paralleli.
>4) Se $a,b,c\in \mathbb{R}^{3}\Rightarrow (a\wedge b)\cdot c =(b\wedge c)\cdot a=(c\wedge a)\cdot b$

Esercizi a pag 2 argomento 5b

>[!def] Superficie parametrica
>Sia $A\subseteq \mathbb{R}^{2}$ aperto e [[Insieme connesso e disconnesso|connesso]] [[Spazio metrico limitato e totalmente limitato|limitato]].
>Denotiamo con $K=\bar A$.
>Una funzione $\varphi:K\to \mathbb{R}^{3}$ si dice superficie parametrica se gode delle seguenti proprietà:
>1) $\varphi$ è di classe [[Classi di funzioni#^08c68a|$C^{1}(A)$]]
>2) $\varphi$ è iniettiva su $A$.
>3) $\varphi$ è [[Continuità funzioni - spazi metrici|continua]] su $K$.
> 
> Il sostegno della superficie è l'immagine di $K$ attraverso $\varphi$. $(\varphi(K))$

^92d1dd

>[!def] Superficie parametrica regolare
>Una [[#^92d1dd|superficie parametrica]] si dice regolare se vale$$||\frac{\partial\varphi}{\partial x}\wedge\frac{\partial\varphi}{\partial y}||\not = 0\qquad \mbox{su tutto A}$$

^89fd73


>[!def] Area di una superficie regolare
>Si definisce l'area di una superficie regolare $\varphi:K\to \mathbb{R}^{3}$ come 
>$$\int_{K}||\frac{\partial \varphi}{\partial x} \land\frac{\partial \varphi}{\partial y}||dxdy=A(\varphi)$$

Ha fatto un'altro calcolo della superficie lo scianna il 24/05, scrivere
esempi a pag 4 argomento5b

>[!clm] Piano tangente
> Sia $\varphi:K=\bar A\to \mathbb{R}^{3}$ una superficie [[#^89fd73|regolare]].
>Prendiamo un punto $(x_{0},y_{0})\in A$ e consideriamo un rettangolo $[x_{0}-\delta,x_{0}+\delta]\times[y_{0}-\eta,y_{0}+\eta]$ che sia tutto contenuto in $A$.
>Sarà allora vero che i segmenti $[x_{0}-\delta, x_{0}+\delta]\times \{y_{0}\}$ e $\{x_{0}\} \times [y_{0}-\eta, y_{0}+\eta]$ sono contenuti in $A$.
>![[Superfici-piano1.excalidraw]]
>Considero $\varphi$ ristretta ai due segmenti
>$\gamma(t):=\varphi(t,y_{0})$ con $t\in[x_{0}-\delta, x_{0}+\delta]$
>$\sigma(s):=\varphi(x_{0},s)$ con $s\in [y_{0}-\eta,y_{0}+\eta]$
>Entrambe queste [[Curve]] hanno sostegno sul [[Curve#^1549a8|sostegno]] di $\varphi$.
>Inoltre possiamo calcolare
>$$\gamma^{'}=\frac{d}{dt}\varphi(x,y_{0})=\frac{\partial \varphi}{\partial x}(x,y_{0})$$
>$$\sigma^{'}=\frac{d}{ds}\varphi(x_{0},y)=\frac{\partial \varphi}{\partial y}(x_{0},y)$$
>Sappiamo che $\gamma^{'}(x_{0})$ è tangente a $\gamma$ nel punto $\varphi(x_{0},y_{0})$ e $\sigma^{'}(y_{0})$ è tangente a $\sigma$ nel punto $\varphi(x_{0},y_{0})$ ([[Curve#^ba243d]]) 
>
>Allora possiamo dire che $\gamma^{'}(x_{0})$ e $\sigma^{'}(y_{0})$ sono tangenti alla superficie in $\varphi(x_{0},y_{0})$.
>Allora $\frac{\partial \varphi}{\partial x}(x_{0},y_{0})$ e $\frac{\partial \varphi}{\partial y}(x_{0},y_{0})$  sono vettori tangenti alla superficie nel punto $\varphi(x_{0},y_{0})$.
>
>Se $\varphi$ è [[#^89fd73|regolare]], allora $\frac{\partial\varphi}{\partial x}(x_{0},y_{0})\wedge\frac{\partial\varphi}{\partial y}(x_{0},y_{0})$ non è il vettore nullo, allora $\varphi(x_{0},y_{0})$ è [[Ortogonale ad un insieme di vettori|ortogonale]] alla superficie.
>
>Possiamo allora dire che i vettori $\frac{\partial \varphi}{\partial x}(x_{0},y_0)$ e $\frac{\partial \varphi}{\partial y}(x_{0},y_0)$ identificano il piano tangente alla superficie nel punto $\varphi(x_{0},y_{0})$.
>Se $\forall(t,s)\in \mathbb{R}^{2}$ pongo
>$$\prod(t,s)=\varphi(x_{0},y_{0})+t\frac{\partial \varphi}{\partial x}(x_{0},y_{0})+s\frac{\partial \varphi}{\partial y}(x_{0},y_{0})$$
>$\prod:\mathbb{R}^{2}\to \mathbb{R}^{3}$ è una mappa(superficie) che ha come sostegno il piano passante per $\varphi(x_{0},y_{0})$ e contenente le rette parametriche
>$$r(t)=\varphi(x_{0},y_{0})+t\frac{\partial \varphi}{\partial x}(x_{0},y_{0})$$
>$$q(s)=\varphi(x_{0},y_{0})+s\frac{\partial \varphi}{\partial y}(x_{0},y_{0})$$
>






