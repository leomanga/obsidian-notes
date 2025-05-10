---
aliases:
  - Trasformata do Steinmetz
  - Antitrasformata di Strinmetz
---
La rappresentazione fasoriale consiste in, data una funzione sinusoidale $e(t)$, rappresentarla nella forma
$$\bar E=E_Me^{j\varphi}$$
ovvero manteniamo l’informazione della fase e dell’ampiezza ma "ci dimentichiamo" della pulsazione della sinusoide.

Ad ogni sinusoide corrisponde un fasore $\bar E$ e quindi un punto del piano complesso inteso come piano dei fasori.

Assegnato $\bar E$ e $\omega$, possiamo associare la sua sinusoide con
$$e(t)=Re[\bar E e^{j\omega t}]$$
Le due relazioni ottenute sono una coppia di trasformata e antitrasformata, dette trasformata e antitrasformata di Strinmetz.

# Proprietà
- Unicità: Siano $e_1(t)$ e $e_2(t)$ due sinusoidi a pulsazione $\omega$, si ha allora necessariamente $e_1(t)=e_{2}(t)\ \forall t$ se e solo se $\bar E_{1}=\bar E_{2}$
- Linearità: Siano $e_{1}(t)$ e $e_2(t)$ due sinusoidi a pulsazione $\omega$ e $a,b\in \mathbb{R}$. Allora $ae_1(t)+be2_{2}(t)$ è una sinusoide a pulsazione $\omega$ con fasore $a\bar E_{1}+b\bar E_{2}$
- Regola di derivazione: Sia $e(t)$ una sinusoide a pulsazione $\omega$ con fasore $\bar E$; allora $\frac{d}{dt} e(t)$ è ancora una sinusoide a pulsazione $\omega$ con fasore $j\omega \bar E$. (Un’operazione differenziale nel dominio del tempo si traduce in una moltiplicazione nel dominio dei fasori)

