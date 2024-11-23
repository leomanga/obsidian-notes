---
pagina: 19
---
# Definizione | derivata parziale
Consideriamo una funzione $f:\mathbb{R}^{n}\to \mathbb{R}$ e prendiamo $x=(x_{1},x_{2},\ldots,x_{n})$ in $\mathbb{R}^{n}$.
Definisco la derivata parziale in $x$ rispetto a $x_{i}$ il limite del rapporto incrementale.
$$\frac{\partial f}{\partial x_{i}}(x)=\lim_{h\to0}\frac{f(x+he_{i})-f(x)}{h}$$
dove $e_{i}=(0,0,\ldots,\underbrace{1}_{i-esima\ coordinata},0,0)$ 

---
Consideriamo una funzione $f:\mathbb{R}^{n}\to \mathbb{R}^{k}$ e prendiamo $x=(x_{1},x_{2},\ldots,x_{n})$ in $\mathbb{R}^{n}$.
La derivata parziale è definita ancora come
$$\frac{\partial f}{\partial x_{i}}(x)=\lim_{h\to0}\frac{f(x+he_{i})-f(x)}{h}$$
Il rapporto incrementale però rappresenterà un vettore in $\mathbb{R}^{k}$ e non più uno scalare.
Dato che $f(x)=(f_{1}(x),f_{2}(x),\ldots,f_{k}(x)$, 
$$\frac{\partial f}{\partial x_{i}}=
\begin{bmatrix}
\frac{\partial f_{1}}{\partial x_{i}} \\
\frac{\partial f_{2}}{\partial x_{i}} \\
\vdots \\
\frac{\partial f_{k}}{\partial x_{i}}
\end{bmatrix}$$
# Definizione | funzione derivabile
$f:\mathbb{R}^{n}\to \mathbb{R}$ si dice derivabile se ammette tutte le sue [[Derivate - spazi metrici#Definizione derivata parziale|derivate parziali]].
# Definizione | gradiente
Si dice gradiente di $f:\mathbb{R}^{n}\to \mathbb{R}$, il vettore 
$$\nabla f=\left(\frac{\partial f}{\partial x_1},\frac{\partial f}{\partial x_1},\ldots, \frac{\partial f}{\partial x_1}\right)$$
# Osservazione
Non in tutti gli spazi metrici vale il seguente teorema: [[Derivate#Una funzione derivabile è continua|derivabile->continua]].
# Definizione | derivata direzionale
Nel caso delle derivate parziali, mi avvicinavo al punto percorrendo una retta, è possibile però calcolare le derivate anche muovendomi con una retta obliqua.
Sia $f:\mathbb{R}^{n}\to \mathbb{R},x\in\mathbb{R}^{n}$ e $v$ un vettore di $\mathbb{R}^{n},v\not=(0,0,\ldots,0)$
Allora definisco la derivata di $f$ in direzione $v$ nel punto $x$ come il limite, se esiste finito, di
 $$\frac{\partial f}{\partial v}(x)=\lim_{h\to0}\frac{f(x+hv)-f(x)}{h}$$
# Definizione | funzione differenziabile
Sia $f:\mathbb{R}^{n}\to\mathbb{R}$ e sia $\bar x\in \mathbb{R}^{n}.$ Supponiamo $f$ risulti derivabile in $\bar x$.
Allora $f$ si dice differenziabile in $\bar x$ se 
$$\lim_{x\to \bar x}\frac{f(x)-f(\bar x)-\nabla f(\bar x)\cdot(x-\bar x)}{||x-\bar x||}=0$$
###### Osservazione
$$\nabla f(x)\cdot(x-\bar x)=
\sum_{i=1}^{n}\frac{\partial f}{\partial x_{i}}(\bar x)\cdot(x_{i}-\bar x_{i})$$
___
Nel caso in cui $f:\mathbb{R}^{n}\to\mathbb{R}^{k}$, se $\bar x\in \mathbb{R}^{n}$ e $f$ è derivabile in $\bar x$.
Si dice che $f$ è differenziabile in $\bar x$ se $$\lim_{x\to\bar x}\frac{||f(x)-f(\bar x)-\nabla f(\bar x)\cdot(x-\bar x)||}{||x-\bar x||}=0$$
# Teorema 1
Sia $f:\mathbb{R}^{n}\to\mathbb{R}^{k}$. Supponiamo $f$ sia [[Derivate - spazi metrici#Definizione funzione differenziabile|differenziabile]] in $\bar x\in\mathbb{R}^{n}.$ Allora si ha
(a) $f$ è continua in $\bar x$
(b) $\forall v$ vettore di $\mathbb{R}^{n}, ||v||\not = 0$ si ha $\frac{\partial f}{\partial v}(\bar x)=\nabla f(\bar x) \cdot v$
#dimostrazione-da-fare [[Disuguaglianza di Cauchy-Schwartz]]
# Teorema del differenziale totale
Sia $f:A\subseteq\mathbb{R}^{n}\to\mathbb{R}$ e sia $\bar x\in \mathbb{R}^{n}$.
Supponiamo che la funzione $f$ sia derivabile in una [[Palla]] $B_{\delta}(\bar x)\subseteq A$ e che le derivate parziali $\frac{\partial f}{\partial x_i}$ risultino continue in $\bar x$.
Allora $f$ è [[Derivate - spazi metrici#Definizione funzione differenziabile|differenziabile]] in $\bar x$.
#dimostrazione-da-fare 
# Derivate successive
> [!def] Derivata Seconda
> Sia $f: A\subset\mathbb{R}^{n}\to \mathbb{R}^{k}$ e supponiamo che esista, per qualche $j\in\{1,\ldots,n\}$, la [[Derivate - spazi metrici#Definizione derivata parziale|derivata parziale]] $\frac{\partial f}{\partial_{x_{j}}}$ in un punto $\bar{x}\in A$.
> Sia $i\in\{1,\ldots,n\}$, diremo che $f$ ammette derivata seconda rispetto a $x_{i}$ e $x_{j}$ in $\bar{x}$ se $\frac{\partial f}{\partial x_{j}}$ ammette derivata parziale rispetto a $x_{i}$ in $\bar{x}$. In tal caso scriveremo
> $$
 \frac{\partial^{2}f}{\partial x_{j}\partial x_{i}}(\bar{x})=\frac{\partial}{\partial x_{i}}\left(\frac{\partial f}{\partial x_{j}}\right)\bar{x}=\lim_{h\to 0}\frac{\frac{\partial f}{\partial x_{j}}(\bar{x}+he_{i})-\frac{\partial f}{\partial x_{j}}(\bar{x})}{h}$$

^5c2d78

>[!def] Matrice hessiana
>Nel caso in cui $f:A\to \mathbb{R}$ ammetta in $\bar {x}$ tutte le derivate parziali seconde $\frac{\partial^{2}f}{\partial x_{j}\partial x_{i}}(\bar{x})$ per ogni $i,j\in\{1,\ldots,n\}$, diremo che $f$ è derivabile due volte in $\bar{x}$. In tal caso definiamo l'**Hessiano** di $f$ in $\bar{x}$ la matrice $\nabla^{2}f(\bar{x})$ contenente tutte le derivate parziali seconde di $f$ in $\bar x$, ovvero
>$$
\nabla^2 f(x) = 
\begin{bmatrix}
\frac{\partial^2 f}{\partial x_1^2} & \frac{\partial^2 f}{\partial x_1 \partial x_2} & \ldots & \frac{\partial^2 f}{\partial x_1 \partial x_n} \\
\frac{\partial^2 f}{\partial x_2 \partial x_1} & \frac{\partial^2 f}{\partial x_2^2} & \ldots & \frac{\partial^2 f}{\partial x_2 \partial x_n} \\
\vdots  & \vdots  &  \ddots &  \vdots \\
\frac{\partial^2 f}{\partial x_n \partial x_1} & \frac{\partial^2 f}{\partial x_n \partial x_2} & \ldots & \frac{\partial^2 f}{\partial x_n^2}
\end{bmatrix}$$
> Nel caso in cui $f:A\to \mathbb{R}^{k}$, l'Hessiano sarà un tensore $k\times n\times n$

> [!thm] Teorema di Shwartz
> Sia $f:A\to \mathbb{R}$ con $A\subseteq \mathbb{R}^{n}$ e supponiamo $f$ ammetta [[#^5c2d78|derivate seconde miste]] $$\frac{\partial^{2}f}{\partial x_{i}\partial x_{j}}$ e $\frac{\partial^{2}f}{\partial x_{j}\partial x_{i}}$$ e $\frac{\partial^{2}f}{\partial x_{j}\partial x_{i}}$ per alcuni indici $i\not = j$. Supponiamo che tali derivate siano continue in $\bar x \in A$, allora
> $$
> \frac{\partial^{2}f}{\partial x_{i}\partial x_{j}}(\bar x)= \frac{\partial^{2}f}{\partial x_{j}\partial x_{i}}(\bar x)$$

#dimostrazione-da-fare Il teorema si dimostra nel caso in cui $\mathbb{R}^{n}= \mathbb{R}^{2}$, dato che è poi estendibile al caso generale.
> [!def] Classi di funzioni
> Una funzione $f:A\to \mathbb{R}^{k}$ si dice di classe $C^{0}$ se è continua su $A$. In tal caso scriveremo $f\in C^{0}(A;\mathbb{R}^{k})$ dove $C^{0}(A;\mathbb{R}^{k})$ è l'insieme di tutte le funzioni continue da $A$ in $\mathbb{R}^{k}$.
> Sia $m\in \mathbb{N}\ge 1$. Diremo che $f:A\to \mathbb{R}^{K}$ è di classe $C^{m}$ se $f$ ammette tutte le derivate di ordine $m$ ed esse risultano continue su $A$ e scriveremo $f\in C^{m}(A; \mathbb{R}^{k})$.
> Diremo che $f\in C^{+\infty}(A;\mathbb{R}^{k})$ se ammette tutte le derivate di qualsiasi ordine $m\ge 1$ ed esse risultano continue su $A$.
> >Osservazione
> >Se $f\in C^{m}(A; \mathbb{R}^{k})\Rightarrow f$ è anche di classe $C^{m-1}(A;\mathbb{R}^{k}), m\ge 1$, come conseguenza del [[#Teorema del differenziale totale]]. In generale tutte le derivate di ordine $m^{'}\le m$ sono [[Continuità funzioni - spazi metrici#Definizione Continua in un insieme|continue]].
> 







