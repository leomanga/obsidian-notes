---
aliases:
  - vestigal-sideband
---
Questo tipo di modulazione è basato sulla semplificazione del progetto del filtro passa-banda rispetto al caso [[SSB]] che richiede in teoria un filtro ideale.
La modulazione avviene attraverso il seguente processo:

![[Pasted image 20250409180300.png]]

Avremo che, eseguendo le operazioni $$u(t)=[A_{c}m(t)\cos(2\pi f_{c}t)]*h(t)$$$$U(f)=\frac{A_{c}}{2}[M(f-f_{c})+M(f+f_{c})]H(f)$$
Dove appunto $H(f)$ sarà un filtro che estrarrà solo la banda laterale.

![[Filtro per VSB.excalidraw]]

La demodulazione avviene attraverso il seguente modello:

![[Pasted image 20250409180311.png]]

Eseguendo le operazioni avremo che
$$\begin{split}V(f)&=\frac{1}{2}[U(f-f_{c})+U(f+f_{c})]=\\&=\frac{A_{c}}{4}[M(f-2fc)+M(f)]H(f-f_{c})+\frac{A_{c}}{4}[M(f+2fc)+M(f)]H(f+f_{c})\end{split}$$
e a questo punto, dato che LP prende solo frequenze $|f|<W$, i prodotti fa $M(f\pm2f_{c})H(f\pm f_c)$ saranno 0, inoltre in questo range $H$ è costante, quindi:
$$V_{l}(f)=\frac{A_{c}}{4}M(f)[H(f-f_c)+H(f+f_c)]=AM(f)$$
Vediamo quindi che il segnale dopo essere demodulato ha ricevuto una certa distorsione.
Abbiamo detto che $H$ è costante, questo chiaramente nella realtà non è possibile, il filtro però funziona lo stesso, perchè, come possiamo vedere nel disegno, 