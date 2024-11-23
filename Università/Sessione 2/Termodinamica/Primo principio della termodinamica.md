# Caso di un sistema chiuso
- [[Sistema termodinamico#Definizione sistema chiuso]]

>[!def] I principio della termodinamica - sistema chiuso
Il primo principio della termodinamica si rappresenta come [[Principio di conservazione dell'energia]], in assenza di variazioni di [[Energia cinetica]] ed [[Energia potenziale della forza peso]], con [[Scambi di energia]] nella forma di [[Calore]] e [[Lavoro]].
>$$\Delta U = W+Q$$

## Casi
Possiamo prendere come riferimento diverse casistiche di un sistema chiuso:
- nel caso di un [[Sistema termodinamico#Definizione sistema isolato|sistema isolato]], allora $W=Q=0$, potendo allora affermare che $\Delta U = 0$.
- nel caso di trasformazioni cicliche, lo stato del sistema coincide con quello finale. Si avrà coincidenza allora dell' [[Energia interna]] iniziale del ciclo $(U_{i})$ e dell'[[Energia interna]] finale del ciclo $(U_f)$. 
  Possiamo allora affermare che $\Delta U =U_{f}-U_{i}\Rightarrow Q=-W$
- Nel caso di trasformazioni [[Sistema termodinamico#Definizione sistema adiabatico|adiabatiche]], essendo il calore scambiato nullo $(Q=0)$, si può affermare che $\Delta U=W$.
# Applicazione nei gas

>  Collegamenti
> [[Lavoro]] ($W$)
> [[Calore]] ($Q$)
> [[Energia interna]] ($U$)
> [[Volume]]($V$)
> [[Pressione]]($p$)
> [[Temperatura]]($T$)
> [[Gas perfetti]]

Il primo principio della termodinamica ha grande applicazione nei sistemi gassosi.
Spesso si rappresenta la sostanza gassosa come [[Gas perfetti|gas perfetto]], in riferimento alle relazioni che legano le variabili $p,V, T$ ([[Gas perfetti#Legge di Boyle e equazione fondamentale dei gas perfetti]]).
## Caso di una trasformazione adiabatica di compressione
Ad esempio, nel caso di un gas perfetto che subisce una trasformazione adiabatica di compressione ($Q=0,\Delta V<0$), si ha 
$$
\Delta U = W, dU=\delta W
$$
Essendo $\delta W = -p\cdot dV$ ([[Lavoro#^6902eb]]), ma anche $p\cdot V = f(T)$ ([[Gas perfetti#Dilatazione termica equazione dei gas perfetti]]) e, dato che $\Delta V<0$, si avrà uno scambio di lavoro che viene compiuto sul sistema, deducendo quindi un incremento dell'energia interna $(\Delta U>0)$.
Essendo $W=f(p,V)=f(T)$, avremo un corrispondente incremento della temperatura.
## Caso di una trasformazione isobara
Nel caso di una trasformazione isobara ($\Delta p=0$) di un gas perfetto, si avranno generalmente valori non nulli del calore trasmesso e della variazione di energia interna.
Da [[Lavoro#^6902eb]] e [[Lavoro#^4706bb]], potremo definire il lavoro trasmesso come
$$
\delta W = -p\cdot dV \Rightarrow W=-p\cdot(V_{f}-V_{i})
$$
Essendo $V_{f}$ e $V_{i}$ il volume del sistema allo stato finale ed iniziale della trasformazione.
## Caso di una trasformazione isocora 
Nel caso di una trasformazione isocora ($\Delta V=0$) di una gas perfetto si avrà uno scambio di lavoro nullo, essendo $\delta W =-p\cdot dV$ e quindi 
$$
\Delta U = Q
$$
Si deduce che nel caso di cessione di calore al sistema, si avrà un incremento di energia interna del sistema e quindi anche un incremento della [[Temperatura]] ($T$).
Sulla base dell'[[Gas perfetti#Legge di Boyle e equazione fondamentale dei gas perfetti|equazione dei gas perfetti]], [[Gas perfetti#^dd36f9]], possiamo trovare che
$$
p=( \frac{n\cdot R_{u}}{V})\cdot T= cost\cdot T
$$
Questo implica che un sistema gassoso sottoposto a scambio di calore verso l'interno, subisca un incremento di temperatura e di pressione.
## Caso di una trasformazione isoterma
Nel caso di una trasformazione isoterma $(\Delta T=0)$ di un gas perfetto, si ha la condizione caratteristica di trasformazione per cui, dall'[[Gas perfetti#Legge di Boyle e equazione fondamentale dei gas perfetti|equazione dei gas perfetti]], [[Gas perfetti#^dd36f9]], troviamo che
$$
p\cdot V=n\cdot R_{u}\cdot T=cost
$$

^22a57b

Per via sperimentale, però, è stato assunto che $U=f(T)$ (esperimenti di Joule), allora si ha, dato che $T$ è costante si ha
$$
\Delta U =0
$$
e pertanto 
$$
W+Q=0\Rightarrow W=-Q
$$
Il lavoro scambiato si può calcolare da [[Lavoro#^4706bb]] e [[#^22a57b]],
$$
W = \int_{V_{i}}^{V_{f}}p\cdot dV=-\int_{V_{i}}^{V_{f}}\frac{n\cdot R_{u}\cdot T}{V}
dV=-n\cdot R_{u}\cdot T \int_{V_{i}}^{V_{f}}\frac{dv}{V}$$
$$W= -n\cdot R_{u}\cdot T\cdot\ln(\frac{V_{f}}{V_{i}})=n\cdot R_{u}\cdot T\cdot \ln(\frac{V_{i}}{V_{f}})$$

