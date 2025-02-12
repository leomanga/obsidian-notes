I calcolatori non hanno a disposizione un numero finito di bits, solo un sottoinsieme dei numeri reali è rappresentabile in un computer.
Questo sottoinsieme è detto **insieme dei numeri di macchina**.
Rappresentiamo i numeri reali con il sistema posizionale a virgola mobile normalizzata
$$\pm(0.d_1d_2\ldots)\beta^{e}$$
dove $d_{1}\not = 0$ e $e$ l’esponente o la **caratteristica**.
L’insieme dei numeri macchina si rappresenta come
$$F(\beta, t,L,U)$$
in cui $\beta$ è la base, $t$ è la mantissa, $L$ è il minimo esponente e $M$ il massimo esponente.
$$\min F(\beta, t, L ,U)=\pm(0.d_{1}d_{2}\ldots d_{t})\beta^ {L\quad}\max F(\beta, t, L ,U)=\pm(0.d_{1}d_{2}\ldots d_{t})\beta^{U}$$

>[!nota]
>Come detto $d_{1}\not = 0$, quindi in base $2$ necessariamente $d_{1}=1$ che viene chiamato bit fantasma.

Chiaramente se $x\in \mathbb{R}$ necessita per la sua rappresentazione in virgola mobile normalizzata, più di $t$ cifre di mantissa sarà necessaria un’approssimazione per arrotondamento o troncamento.
Rappresentiamo l’approssimazione come
$$\bar x = fl(x)$$
Avremo
>[!def] Approssimazione per troncamento
>$$fl(x)=\pm(0.d_1d_{2}\ldots d_{t})\beta^{e}$$
>

^ca2a1e

>[!def] Approssimazione per arrotondamento
>$$fl(x)=\begin{cases}\pm(0.d_1d_2\ldots d_{t})\quad &dt_{t+1}<\frac{\beta}{2}\\
>\pm(0.d_1d_2\ldots(d_{t}+1)\quad &d_{t+1}>\frac{\beta}{2} \end{cases}$$
>Se $d_{t+1}=\frac{\beta}{2}$ si applica il cosiddetto “round to even”, ovvero si sceglie di rendere $d_{t}$ pari.

^e8c116

L’approssimazione genera certamente errori di rappresentazione:
- Errori di underflow: $e< L$
- Errori di overflow: $e>U$
- Errori di arrotondamento: $L\le e\le U$ ma il numero di cifre è maggiore di $t$

Il numero di cifre che l’elaboratore riserva alla mantissa determina la **precisione** con la quale l’elaboratore lavora.
Studiando la limitazione superiore degli [[Teoria degli errori#^0c317c|errori assoluti]] avremo che 
- Con [[#^ca2a1e|troncamento]] $$|x-fl(x)|<\beta^{e-t}$$
- Con [[#^e8c116|arrotondamento]]
$$|x-fl(x)|\le\frac{1}{2}\beta^{e-t}$$
Studiando la limitazione superiore degli [[Teoria degli errori#^0f475d|errori relativi]] invece avremo
- Con [[#^ca2a1e|troncamento]] $$|\frac{x-fl(x)}{x}|<\beta^{1-t}=\epsilon_{m}\forall x\not=0$$
- Con [[#^e8c116|arrotondamento]]
$$|\frac{x-fl(x)}{x}|<\frac{1}{2}\beta^{1-t}=\frac{1}{2}\epsilon_{m}\forall x\not=0$$

Dove chiamiamo $\epsilon_{m}$ **precisione di macchina**.

>[!def] Precisione di macchina
>$$\epsilon_{m}=\beta^{1-t}$$

^ff68fc


