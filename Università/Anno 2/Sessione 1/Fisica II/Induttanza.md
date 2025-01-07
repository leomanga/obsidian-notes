---
aliases:
  - Coefficiente di autoinduzione
---
Abbiamo per ipotesi un circuito
- Chiuso e isolato
- Fisso e indeformabile
Le condizioni sono di quasi stazionarietà, la [[Corrente elettrica]] che scorre nel circuito viene ipotizzata costante in tutti i punti del circuito ad ogni tempo $t$. (Nella realtà la corrente impiega del tempo, anche se piccolissimo, a propagarsi nel circuito).
Tutto, inoltre, è immerso in un mezzo materiale lineare, omogeneo e isotropo di [[Magnetostatica nei mezzi materiali#Suscettività e permeabilità magnetica|permeabilità magnetica]] $\mu$.

![[Induttanza.excalidraw]]

Abbiamo che, dalla [[Campo di induzione magnetica#^39e67d|prima formula di Laplace]],
$$\vec{B}(\vec{r}, t)=\frac{\mu}{4\pi}\oint_{C}\frac{I(\vec{r,}t)d\vec{l}(\vec{r})\times(\vec{r}- \vec{r}^{'})}{|\vec{r}-\vec{r}^{'}|^{3}}\quad [T]$$
Ma dall’ipotesi di quasi stazionarietà, possiamo scrivere
$$\vec{B}(\vec{r}, t)=I(t)\underbrace{\frac{\mu}{4\pi}\oint_{C}\frac{d\vec{l}(\vec{r})\times(\vec{r}- \vec{r}^{'})}{|\vec{r}-\vec{r}^{'}|^{3}}}_{\mbox{termine costante}}\quad [T]$$
Se calcoliamo il [[Flusso di un campo vettoriale|flusso]] generato dalla spira, all’interno della spira,
$$\Phi[\vec{B}(\vec{r},t)]=\iint_S{\vec{B}(\vec{r},t)}\cdot\hat{n}\cdot ds=I(t)\underbrace{\frac{\mu}{4\pi}\iint_{S}[\oint_{C}\frac{d\vec{l}(\vec{r})\times(\vec{r}- \vec{r}^{'})}{|\vec{r}-\vec{r}^{'}|^{3}}]\cdot \hat n\cdot ds}_{\mbox{termine costante}=L}$$
Possiamo scrivere allora $$\Phi[\vec{B}(\vec{r},t)]=LI(t)$$
dove $L$ prende il nome di **coefficiente di induzione o induttanza**.
$$L=\frac{\Phi[\vec{B}(\vec{r},t)]}{I}\quad [\frac{Wb}{A}][H]$$
L’unità di misura è in Henry.
Dalla legge di [[Legge di Faraday-Neumann-Lenz]] si autoinduce una [[Generatore di forza elettromotrice#^6d2e46|forza elettromotrice]] 
$$\epsilon_{i}(t)=-L\frac{dI(t)}{dt}$$
# Caso solenoide
![[Solenoide-Induttanza.excalidraw]]

Abbiamo come dato il numero di spire al metro $N [\frac{sp}{m}]$
Tramite [[Magnetostatica nei mezzi materiali#^78a52c]] e dal fatto che avremo $N$ superfici, troviamo che
$$H(t)=NI(t)$$
Allora, da [[Vettore campo magnetico]] e visto che siamo nel vuoto, $$B(t)=\mu_{0}\vec{H}(t)=\mu_{0}NI(t)$$
Calcoliamo il flusso di una spira
$$\Phi_{sp}(t)=\pi a^{2}\mu_{0}NI(t)$$
Essendoci $Nl$ spire nel nostro sistema, avremo che il flusso totale è
$$\Phi_{T}=Nl\Phi_{sp}=\mu_{0}N^{2}\pi a^{2}lI(t)$$
In questo caso allora avremo $$L=\frac{\Phi_{T}(t)}{I(t)}=\mu_{0}N^{2}\pi a^{2}l$$

Ora se colleghiamo il solenoide ad un circuito con una certa resistenza ed un generatore di tensione ($\epsilon$), da [[Legge di Faraday-Neumann-Lenz]] si genera una $\epsilon_{i}=-L\frac{dI(t)}{dt}$, quindi possiamo vedere il solenoide come un generatore messo con i capi al contrario.

Usando la [[Legge di Ohm]] 
$$\epsilon+\epsilon_{i}=RI(t)$$
Otteniamo l’equazione differenziale $$\epsilon=RI(t)+L\frac{dI(t)}{dt}$$
che ha come soluzione $$I(t)=\frac{\epsilon}{R}(1-e^{-\frac{R}{L}t})$$
Avremo quindi che ad infinito il circuito si comporterà come se il solenoide fosse un filo, quindi $I_{\infty}=\frac{\epsilon}{R}$.
Avremo che il circuito avrà questo comportamento dopo $5\tau$, dove $\tau=\frac{L}{R}$.
Se cortocircuitassimo il generatore di tensione, il circuito impiegherebbe sempre $5\tau$ ad avere corrente pari a zero.

Se invece aprissimo un interruttore sul circuito, avremmo una resistenza incredibilmente grande, tau tenderebbe a 0 e verrebbe provocata una scintilla.