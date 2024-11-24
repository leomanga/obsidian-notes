---
collegamenti:
  - "[[Calore]]"
  - "[[Scambi di energia]]"
---
L'irraggiamento termico è un fenomeno fisico in cui le superfici a temperature finite emettono energia come onde elettromagnetiche. 
Questo fenomeno coinvolge tutte le sostanze, ma solitamente viene studiato per applicazioni legate alle trasmissioni fra corpi solidi.
L'irraggiamento, a differenza della [[Conduzione termica]] e della [[Convezione termica]], avviene anche in assenza di mezzi materiali di trasporto, risultando più efficiente in assenza di materia(nel vuoto).

>[!def] Costante di Stefan-Boltzmann
>$$\sigma=5,67\cdot10^{-8}\qquad \left[\frac{W}{m^{2}\cdot K^{4}}\right]$$

^c7ada7

>[!def] Potenza emissiva
>La potenza emissiva, definita dalla legge di Stefan-Boltzmann, è la quantità di energia per unità di superficie che un corpo può emettere
>$$\dot{e}_{max}=\sigma\cdot(T_{s} )^{4}\qquad \left[\frac{W}{m^{2}}\right]$$
>$T_{s}$ è la temperatura superficiale del corpo
>$\sigma$ è la [[#^c7ada7]]
^a2be17

>[!def] Corpo nero o corpo radiatore
>%%display:corpo nero%%
>Se un corpo emette un flusso di energia $\dot E$ pari a $\dot{E}_{max}$, allora si tratta per definizione di un corpo radiatore o corpo nero.
>Dove $\dot{E}_{max}$ è la [[#^a2be17]] per una superficie.

^bfc749

Nel caso reale, per una determinata temperatura superficiale $T_{s}$, un corpo emette un flusso di energia per irraggiamento pari a
>[!def] Flusso di energia per irraggiamento
>$$\dot{E}=\epsilon\cdot\sigma\cdot A\cdot(T_{S})^{4}\qquad [W]$$
>$\epsilon$ è un coefficiente tra $0$ e $1$ un funzione della distanza dalle condizioni del corpo nero ([[#^a2be17]])
>$\sigma$ è la [[#^c7ada7]]
>$A$ è la superficie del corpo
>$T_{S}$ è la temperatura superficiale del corpo

^03359a

>[!def] Flusso di energia per irraggiamento per unità di superficie
>$$\dot{e}=\epsilon\cdot\sigma \cdot(T_{S})^{4}\qquad[\frac{W}{m^{2}}]$$
>$\epsilon$ è un coefficiente tra $0$ e $1$ in funzione della distanza e dalle condizioni del corpo nero ([[#^a2be17]])
>$\sigma$ è la [[#^c7ada7]]
>$T_{S}$ è la temperatura superficiale del corpo

Oltre al fenomeno di emissione delle radiazioni elettromagnetiche, su un sistema insistono anche fenomeni di assorbimento di radiazioni emesse da altri sistemi.

Indichiamo con $\dot{G}$ e $\dot{g}$ i [[#^03359a|flussi di energia]] assoluti e specifici da cui viene investito un sistema, e con $\dot{G}_{ass}$ e $\dot{g}_{ass}$  il flusso di radiazione che il corpo assorbe. Si può affermare che 
$$\dot{G}_{ass}=\alpha\cdot\dot{G}$$
>[!def] Coefficiente di assorbimento
>$$\alpha$$

^81fc66

Indicando con $T_{0}$ la temperatura del sistema radiante che consideriamo un [[#^bfc749]] che determina il flusso di energia $\dot{G}$, se ne deduce, da [[#^a2be17]] che
$$\dot{G}_{ass}=\alpha\cdot\sigma\cdot A\cdot (T_{0})^{4}$$
Si possono quindi esprimere i due flussi di energia specifici, uno assorbito ($\dot{g}_{ass}$) e l'altro emesso dal sistema ($\dot{e}$).
Vediamo che $\dot{g}_{ass}$ è pari al coefficiente di assorbimento $\alpha$ per l'irraggiamento specifico
 $$\dot{g}_{ass}=\alpha\cdot\dot{g}=\alpha\cdot\sigma\cdot(T_{0})^{4}$$
 $$\dot{e}=\epsilon\cdot\sigma\cdot(T_{S})^{4}$$
Il coefficiente $\alpha$ dipende sia dalla superficie che dalla natura della radiazione.

>[!def] Flusso netto di energia per irraggiamento
>$$\dot{q}=\dot{g}_{ass}-\dot{e}=\alpha\cdot\sigma\cdot(T_{0})^{4}-\epsilon\cdot\sigma\cdot(T_{S})^{4}$$
>$\alpha$ è il [[#^81fc66]]
>$\sigma$ è la [[#^c7ada7]]
>$T_{0}$ è la temperatura del [[#^bfc749]], che trasmette radiazioni
>$\epsilon$ è un coefficiente tra $0$ e $1$ in funzione della distanza e dalle condizioni del [[#^corpo nero]] ([[#^a2be17]])
>$T_S$ è la temperatura superficiale del corpo

![[Irraggiamento.png]]