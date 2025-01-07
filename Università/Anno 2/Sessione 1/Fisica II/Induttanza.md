---
aliases:
  - Coefficiente di autoinduzione
---
Abbiamo per ipotesi un circuito
- Chiuso e isolato
- Fisso e indeformabile
Le condizioni sono di quasi stazionarietà, la [[Corrente elettrica]] che scorre nel circuito viene ipotizzata costante in tutti i punti del circuito ad ogni tempo $t$. (Nella realtà la corrente impiega del tempo, anche se piccolissimo, a propagarsi nel circuito).

Abbiamo che, dalla [[Campo di induzione magnetica#^39e67d|prima formula di Laplace]],
$$\vec{B}(\vec{r}, t)=\frac{\mu}{4\pi}\oint_{C}\frac{I(\vec{r,}t)d\vec{l}(\vec{r})\times(\vec{r}- \vec{r}^{'})}{|\vec{r}-\vec{r}^{'}|^{3}}$$
Ma dall’ipotesi di quasi stazionarietà, possiamo scrivere
$$\vec{B}(\vec{r}, t)=I(t)\underbrace{\frac{\mu}{4\pi}\oint_{C}\frac{d\vec{l}(\vec{r})\times(\vec{r}- \vec{r}^{'})}{|\vec{r}-\vec{r}^{'}|^{3}}}_{\mbox{}}$$