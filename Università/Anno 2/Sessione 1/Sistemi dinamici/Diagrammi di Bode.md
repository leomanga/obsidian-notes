Studiamo i [[Sistemi a tempo continuo]] [[Sistemi lineari tempoinvarianti|LTI]].
Lo scopo dei diagrammi di Bode è quello di rappresentare
- La [[Teorema della risposta in frequenza#^a625cb|risposta di regime permanente]] tramite il modulo e la fase di $G(j\omega)$, riuscendo a capire come reagisce il sistema ad un ingresso sinusoidale.
- I segnali periodici con la [[Serie di fourier]]
$$f(t)=f(t+\underbrace{T}_{periodo})\ \forall t\Rightarrow f(t)=\sum_{k=-\infty}^{\infty}F_{k}e^{j}\frac{2\pi}{T}k$$
- I segnali generici tramite la [[Trasformata di Fourier]]$$f(t)=\frac{1}{2\pi}\int_{-\infty}^{+\infty}F(j\omega)e^{j\omega t}d\omega$$
  Se esiste la [[Trasformata di Laplace]] di $f(t)$, allora $F(j\omega)=F(s)$ per $s=j\omega$.
- Se $G(j\omega)$ è razionale fratta, allora conoscere $|G(j\omega)|$ e $\measuredangle G(j\omega)$ equivale a conoscere $G(s)$.
## Proprietà
- $|G(j\omega)|$ è una **funzione pari**. $|G(-j\omega)=|\overline{G(j\omega)}|=|G(j\omega)|$. 
- $\measuredangle G(j\omega)$ è una **funzione dispari**. $\measuredangle G(-j\omega)=\measuredangle \overline{G(j\omega)}=-\measuredangle G(j\omega)$
Sarà sufficiente disegnare le funzioni per $\omega \ge 0$

## Diagrammi
Per disegnare il modulo usiamo
- come ascissa la scala $\log_{10}\omega$
- come ordinata la scala $20\log_{10}|G(j\omega)|=|G(j\omega)|_{dB}$

Per disegnare la fase usiamo
- come ascissa la scala $\log_{10}\omega$
- come ordinata i gradi

Ogni intervallo fra $10^i$ e $10^{i+1}$ è detto **decade**.
Da notare che per $\omega=0$, avremo che $\log_{10}\omega=-\infty$, ovvero dove dovrebbe essere il [[Gradino unitario]].
## Forma di Bode
![[Forma di Bode]]

Se abbiamo $a,b\in \mathbb{C}$
Dato che
$$\log|a\cdot b|=\log|a|+\log|b|$$
e da [[Campo dei numeri complessi#Proprietà dell’argomento o fase|proprietà fase]]
![[Campo dei numeri complessi#^fa4be1]]

Avendo quindi scritto la [[Forma di Bode]] come prodotto di pezzi, posso tracciare i moduli e le fasi di ogni pezzo e poi sommarli.

