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

## Come disegnare
Per il termine costante  è facile.
Stessa cosa per il termine monomio, basta sostituire a $\frac{1}{s^{g}}$, $1/(j\omega)^{g}$ e risolvere.
Per il termine binomio dovremo approssimare ed avremo $20\log_{10}(\omega)+20log_{10}|\tau|$ quando $|\omega\tau|>>1$, sennò avremo $20\log_{10}1=0$.
Per la fase #da-finire  pag 92
Termine trinomio #da-finire 

## Procedura
Modulo:
1)  Si parte sempre dal termine $\frac{k_{B}}{s^{g}}$ che corrisponde ad una retta di pendenza $-20g\ dB/dec$ e che passa per il punto $\omega=1$ con modulo $|\cdot|_{dB}=20\log|k_{B}|$
2) Si portano sull’asse delle ascisse i punti di rottura pari a $\frac{1}{|\tau|}$ per i termini binomio e a $\omega_{i}$ per i termini trinomio.
3) Partendo da sinistra, verso destra, in corrispondenza dei punti di rottura, si varia la pendenza di
	- $+20\mu dB/dec$ per ogni zero reale di molteplicità $\mu$
	- $-20\mu dB/dec$ per ogni polo reale di molteplicità $\mu$ 
	- $+40\mu dB/dec$ per ogni coppia di zeri complessi di molteplicità $\mu$
	- $-40\mu dB/dec$ per ogni coppia di poli complessi di molteplicità $\mu$

Fase:
1) Si parte con una semiretta orizzontale da $\omega = 0$, quindi da $\log_{10}\omega=-\infty$ fino al primo punto di rottura, di valore pari a $\begin{cases}-90°\cdot g\quad \mbox{se }k_{B}>0\\ -90°\cdot g-180°\quad \mbox{se }k_{B}<0\end{cases}$
2) Si riportano in ascissa gli stessi punti di rottura del diagramma del modulo.
3) Procedendo da sinistra a destra, in corrispondenza dei punti di rottura, si varia la fase di
	- $+90°\mu$ per ogni zero reale negativo o polo reale positivo di molteplicità $\mu$
	- $-90°\mu$ per ogni zero reale positivo o polo reale negativo di molteplicità $\mu$
	- $+180°\mu$ per ogni coppia di zeri complessi a parte reale negativa o poli complessi a parte reale positiva di molteplicità $\mu$
	- $-180°\mu$ per ogni coppia di zeri complessi a parte reale positiva o poli complessi a parte reale negativa di molteplicità $\mu$
