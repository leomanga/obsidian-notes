La risposta forzata $y_{f}$ nell’uscita o $x_{f}$ nello stato è la parte del sistema dinamico, influenzata dall’ingresso $u$.

Dopo la [[Trasformata di Laplace]] possiamo dire che $Y_{f}(s) = G(s)\cdot U(s)$ dove $G(s)$ è la [[Funzione di trasferimento]].

# Risposta forzata per i vari ingressi
## Risposta impulsiva
In questo caso abbiamo come ingresso il [[Segnale impulsivo]]. ($u(t)=\delta(t)$)
Allora, dato che $U(s)=1$, avremo $Y_{f}=G(s)$.
Allora $$y_{imp}(t)=\mathcal{L}^{-1}[G(s)]$$
$y_{imp}$ prende il nome di risposta impulsiva e funziona come base per tutti gli altri casi.

## Ingresso generico
Per un ingresso generico avremo che $$y_{f}(t)=\mathcal{L}^{-1}[G(s)\cdot U(s)]=y_{imp}(t)*u(t)$$
dove $*$ rappresenta il [[Prodotto di convoluzione]].
$y_{imp}(t)$, come visto nella [[#Risposta impulsiva]] è l’antitrasformata di $G(s)$.
## Risposta al gradino
In questo caso abbiamo come ingresso il [[Gradino unitario]]. ($u(t)=\mathbb{1}(t)$)
$$Y_{f}(s)=G(s)\cdot U(s)=G(s)\cdot \frac{1}{s}$$
Allora da [[#Ingresso generico]]
$$y_{f}(t)=y_{imp}(t)*\mathbb{1}(t)=\int_{0}^{t}y_{imp}(\tau)d\tau$$
Quindi la **risposta al gradino** è l’integrale della [[#Risposta impulsiva]].

Ci chiediamo cosa succede per $\lim_{t\to \infty}y(t)$.
Vogliamo che questo limite esista finito, e questo vale per i poli a parte reale negativa, tranne al più un solo polo in 0. ([[Modi di un sistema dinamico lineare#Convergenti|(1)]] [^1])
Dato che il polo in 0 viene già “occupato” da $\frac{1}{s}$, vogliamo che **$G(s)$ abbia tutti i poli a parte negativa**.
Allora, da [[Trasformata di Laplace#^f408f6]]
$$\lim_{t\to \infty}y_{f}(t) = \lim_{s\to 0}s\cdot G(s)\cdot \frac{1}{s}=G(0)$$
$G(0)$ prende il nome di **guadagno stazionario del sistema**.




[^1]: Nota che nel link non è citato il polo in 0 dato che con convergenti si intende che tendono a 0. Un solo polo in 0 invece permette di far tendere il limite ad 1, che in questo caso è accettabile.

## Risposta al segnale sinusoidale
[[Teorema della risposta in frequenza]]