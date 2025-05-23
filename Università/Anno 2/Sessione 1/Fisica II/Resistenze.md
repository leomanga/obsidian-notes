![[Legge di Ohm]]


Possiamo vedere che, in caso di [[Corrente stazionaria]], in un [[Materiali conduttori|conduttore]] metallico, dato che $$\vec{J}=\sigma\cdot \vec{E}$$
dove $\sigma$ è la [[Densità di corrente elettrica#^c5f9e4|conducibilità elettrica]] e $\vec{E}$ il [[Campo elettrostatico]] locale.
Inoltre $\Delta V = |E|\cdot l$ ($l$ è la distanza fra le due sezioni).
Allora potremo scrivere
$$I = |\vec{J}|S=\sigma |\vec{E}|S=\sigma S \frac{\Delta V}{l}$$
Allora $$\Delta V = \frac{1}{\sigma}\frac{l}{S}I=\frac{\rho\cdot l}{S}I$$
dove 
$$
\rho = \frac{1}{\sigma}\quad [\frac{V}{A}\cdot m]
$$

^1a2c4e

prende il nome di **resistività**.
E possiamo definire
>[!def] Resistenza in un [[Materiali conduttori|conduttore]] metallico
>$$R = \frac{1}{\sigma}\frac{l}{S}=\frac{\rho\cdot l}{S}\quad [\ohm]$$
>dove $\sigma$ è la [[Densità di corrente elettrica#^c5f9e4|conducibilità elettrica]], $l$ è la distanza fra le due sezioni a diverso [[Potenziale elettrostatico|potenziale]], $S$ la superficie delle sezioni del materiale e $\rho$ è la resistività [[#^1a2c4e]]


>[!prp] Legge di Joule
Sappiamo che la [[Potenza]], da [[Corrente elettrica#^9163ff|link]] può essere calcolata come 
$$P= (V_{A}-V_{B})I=RI^{2}=\frac{(\Delta V)^{2}}{R}\quad [W]$$
> La potenza generata viene dissipata attraverso calore e questo fenomeno prende il nome di **effetto Joule**.

^2b0c5c

# Parte di elettrotecnica
Parliamo di resistori ideali. Ogni resistore ideale è passivo se e solo se $R\ge 0$. Nella realtà lo è sempre, quindi le resistenze sono sempre bipoli passivi. Questo è dato da [[#^2b0c5c]] in cui si vede che la potenza è sempre positiva se $R\ge 0$ e da [[Bipolo#^bc5df0]] si trae la conclusione.
#TODO Trasformazione triangolo-stella

## Regime sinusoidale
Supponiamo $i(t)=I_{M}\cos(\omega t+\phi_{i})$, allora dalla legge di Ohm
$$v(t)=V_M\cos(\omega t+\phi_v)=Ri(t)=RI_{M}\cos(\omega t+\phi_{i})$$
Allora $$V_M=RI_{M},\quad \phi_v=\phi_i$$

>[!def] Relazione costitutiva nel dominio dei fasori
>[[Fasori]]
>$$\bar V = R\bar I$$
>
>![[Resistenza-fasori.excalidraw]]




