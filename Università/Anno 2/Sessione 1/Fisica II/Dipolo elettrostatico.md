![[Dipolo elettrostatico.excalidraw]]

Vogliamo calcolare il [[Potenziale elettrostatico]] di questa configurazione
$$V(P)=V^{+}(P)+V^{-}(P)$$
dove $V^{+}$ e $V^{-}$ sono il potenziale della carica positiva e di quella negativa.

Avremo allora
$$V^{+}(P)=k_{e}\frac{Q}{|\vec{r^{+}}-\frac{\delta}{2}\hat{z}|}$$$$V^{-}(P)=-k_{e}\frac{Q}{|\vec{r^{-}}-\frac{\delta}{2}\hat{z}|}$$
Adesso dal [[Teorema di Carnot]]
$$|\vec{r^{+}}|=\sqrt{r^{2}+ \frac{\delta^{2}}{4}-r\delta\cos{\theta}}=r^{2}\sqrt{1+\frac{\delta^2}{4r^{2}}-\frac{\delta}{r}\cos{\theta}}$$
$$|\vec{r^{-}}|=r^{2}\sqrt{q+\frac{\delta^2}{4r^2}+\frac{\delta}{r}\cos{\theta}}$$
Facendo un po’ di approssimazioni, immaginando $r>> \delta$, otteniamo
$$V(P)\simeq\frac{k_{e}Q\delta\cos{\theta}}{r^{2}}$$
Chiamiamo 
>[!def] Momento di dipolo
>$$\vec{p} = Q\cdot \vec{\delta}$$
>Successivamente abbiamo visto anche che $\vec{p}=\alpha\cdot \vec{E}_{l}$ dove $\alpha$ è la polarizzabilità di ogni elemento e $\vec{E}_{l}$ è il campo locale che agisce sull’elemento.

^ac2828

Allora 
>[!prp] Potenziale a grandi distanze
>Se la distanza fra le cariche è molto più piccola di quella in un punto $\vec{r}$, si ha
>$$V(P)=k_{e}\cdot \vec{p}\cdot\vec{r}\cdot \frac{1}{r^3}\quad[V]$$
>Dove $\vec{P}$ è il [[#^ac2828|momento di dipolo]]

Possiamo inoltre calcolare il momento meccanico 
>[!prp] Momento meccanico
>
$$\vec{M}=\vec{p}\times\vec{E}\quad [N\cdot m]$$
Dove $\vec{p}$ è il [[#^ac2828|momento di dipolo]] e $\vec{E}$ è il [[Campo elettrostatico]]

Inoltre abbiamo
>[!prp] Forza risultante se le due cariche sono diverse
Se le due cariche opposte non sono uguali, la forza risultante (applicata al baricentro) di un dipolo su un campo elettrostatico è
>
$$\vec{R}=(\vec{p}\cdot \nabla)\vec{E}$$

Possiamo anche calcolare l’energia potenziale
>[!def] Energia potenziale del dipolo
>$$U=-\vec{p}\cdot \vec{E}(r)\quad [J]$$
>Dove $\vec{p}$ è il [[#^ac2828|momento di dipolo]] e $\vec{E}$ è il [[Campo elettrostatico]]

