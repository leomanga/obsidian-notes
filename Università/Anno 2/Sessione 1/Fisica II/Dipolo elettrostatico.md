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
Chiamiamo $\vec{P} = Q\cdot \vec{\delta}$ **momento di dipolo**.
Allora $$V(P)=k_{e}\cdot \vec{P}\vec{r}\cdot \frac{1}{r^3}$$
Possiamo inoltre calcolare il momento meccanico come 
$$\vec{M}=\vec{P}\times\vec{E}$$
Se le due cariche opposte non sono uguali, la forza risultante di un dipolo su un campo elettrostatico è
$$\vec{R}=(\vec{P}\cdot \nabla)\vec{E}$$
