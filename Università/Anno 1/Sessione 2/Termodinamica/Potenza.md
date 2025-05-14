---
collegamenti:
  - "[[Lavoro]]"
---
La potenza è la misura della velocità con cui avviene uno scambio di energia  [[Lavoro]].
$$\begin{split}\dot W = P &= \frac{\delta W}{dt}=\frac{W}{\Delta t} =\vec{F}\cdot\frac{d\vec{s}}{dt}=\vec{F}\cdot \vec{v}\quad &\left[\frac{J}{s}\right]\\&=I(V_{A}-V_{B})\quad &[V \cdot A] \end{split}\quad[W]$$
dove $\delta W$ è il [[Lavoro]] in un istante infinitesimo di tempo.
$d\vec{s}$ è lo [[Legge oraria|Spostamento]] infinitesimo e $\vec{v}$ la [[Velocità]].
$J$ sono i Joule, $s$ i secondi e $W$ i Watt. 
$I$ è la [[Corrente elettrica]] e $V_A$ e $V_{B}$ sono i [[Potenziale elettrostatico|potenziali]] di due estremità di un conduttore.

# Potenza nel regime sinusoidale
Parte di elettrotecnica.

Facciamo uso della definizione di [[Valore efficace]]
Data la definizione di potenza istantanea
$$p(t)=v(t)i(t)=V_{M}\cos(\omega t+\phi_v)I_{M}\cos(\omega t+\phi_{i}) W$$ Definiamo la potenza attiva e reattiva, il risultato della media della potenza istantanea.
$$P_{tot}=\frac{1}{T}\int_{0}^{T}v(t)i(t)dt=P_{a}+P_{r}=\frac{1}{2}V_{M}I_{M}=VI \quad [W]$$
dove $P_{a}$ è data dalla parte reale della corrente e della tensione, mentre $P_{r}$ è data dalla parte immaginaria di esse.
$P_r$ per sua natura, nel periodo $T$, è sempre 0, ovvero è una potenza scambiata reversibilmente, non viene dissipata. Ad essa non è associato alcun trasferimento di energia utile al carico.
Viene introdotta a questo punto $Q=\frac{1}{2}V_{M}I_{rM}=VI_{r}=VI\sin(\phi_z)$ la cui unità di misura sarebbe sempre i Watt, ma per convenzione e per distinguerli si userà l’unità VAR.
Viene naturalmente introdotta anche la potenza attiva $P=\frac{1}{2}V_{M}I_{aM}=VI_{a}=VI\cos(\phi_{z)}\ [W]$

Inoltre si definisce la potenza apparente $A$ come
$$A = \frac{1}{2}V_M I_M=\sqrt{P^{2}+Q^{2}}\quad VA$$
La cui unità di misura sono i VA(volt-ampere) per distinguerla.

continua da esressioni potrenza istantanea pag 26 lezione 11 