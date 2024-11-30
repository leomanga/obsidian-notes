In ingresso ad un [[Sistemi lineari tempoinvarianti]] mettiamo $$u(t)=M\cos(\omega t+\phi)$$
$M$ è l’ampiezza, $\omega$ la pulsazione e $\phi$ la fase.
==Immaginiamo la fase nulla.==

Come ipotesi abbiamo che tutti i poli di $G(s)$ ([[Funzione di trasferimento]]) abbiano parte reale negativa, quindi da [[Modi di un sistema dinamico lineare#Caratteristiche di convergenza dei modi]], tutti i modi saranno convergenti.

Intanto avremo che la [[Trasformata di Laplace]] di $u(t)$ sarà
$$U(s)=M\frac{s}{s^{2}+\omega^2}$$
Il quale ha come poli parte reale nulla e parte immaginaria.

Avremo allora che $Y_{f}(s)=G(s)\cdot U(s)$ sarà una funzione con poli tutti negativi tranne due poli coniugati immaginari.
Facendo un po’ di calcoli si trova che 
$$y_{f}(t)=\frac{M}{2}G(j\omega)e^{j\omega t}+\frac{M}{2}G(j\omega)e^{-j\omega t}+y_{t}(t)$$
dove $y_{t}(t)$ viene chiamata **RISPOSTA DI REGIME TRANSITORIO**, che è relativa ai modi con i poli negativi, quindi per $t\to \infty$, $y_{t}(t)\to \infty$.
Sfruttando la scrittura esponenziale del [[Campo dei numeri complessi]] scriviamo
$$G(j\omega)=|G(j\omega)|e^{j\measuredangle G(j\omega)}$$
(con $\measuredangle$ si intende la fase di $G(j\omega)$)
Allora, facendo un po’ di calcoli possiamo scrivere che 

>[!prp] Risposta di regime permanente
>In generale, dato $u(t)=M\cos(\omega t+\phi)$ ed una [[Funzione di trasferimento]] con tutti i poli negativi, avremo come [[Risposta forzata]]
>$$
y_{f}(t)=M|G(j\omega)|\cos(\omega t+\measuredangle G(jw)+\phi)+y_{t}(t)
>$$
>La risposta forzata in questo caso prende il nome di **RISPOSTA DI REGIME PERMANENTE** ed è caratterizzata da una amplificazione o da una attenuazione dell’ampiezza $M$ dal modulo di $G(j\omega)$ e da uno sfasamento $\measuredangle G(jw)$.
>La risposta di regime transitorio $y_{t}(t)$ tenderà a 0 per $t\to \infty$.

per trovare $y_{t}$ si usa che è la parte rimanente dalla scomposizione in fratti semplici. Dato che la risposta viene da $$\frac{Q(s)}{D(s)}+\frac{R_{2}}{s-j\omega}+\frac{\overline{R_{2}}}{s+j\omega}$$
Avremo che $$y(t)=\mathcal{L}^{-1}[\frac{Q(s)}{D(s)}]$$
Dove $Q$ e $D$ sono i resti dalla scomposizione in fratti semplici.
# Altri casi
Abbiamo avuto come ipotesi che $G(s)$ avesse poli a parte reale negativa.
- Se ha almeno un polo maggiore di 0, avremo che $y_{p}(t)$ sarà divergente.
- Se ha un polo in 0, allora $y_{t}$ tenderà ad una costante e $y_{p}$ tenderà ad una sinusoide con media non nulla.
- Se contiene i poli immaginari $\pm j\alpha$, con $\alpha\not = 0$, allora $y_{t}$ conterrà i modi $\cos$ e $\sin$. Questo fenomeno si chiama **BATTIMENTO**. In base ad $\alpha$, è possibile che $y_{p}$ si annulli.
- Se contiene i poli immaginari $\pm j\omega$, allora i conti fatti non sono più veri dato che abbiamo molteplicità 2. Avremo che la [[Risposta forzata]] conterrà i modi $t\cos$ e $t\sin$. Questo fenomeno si chiama **RISONANZA**.




