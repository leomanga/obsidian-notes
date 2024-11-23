---
pagina: 15
---
# Definizione | pressione esercitata da un fluido
La pressione esercitata da un fluido in quiete su una superficie di area unitaria è pari al rapporto fra la forza normale alla superficie e la superficie.
$$p = \lim_{A\to A^{'}}\frac{F_{n}}{A}\qquad [\frac{N}{m^2}]$$
$A$ è la [[Superficie]] minima per la quale ha senso definire la materia.
$F_{n}$ è la [[Forza]] perpendicolare alla superficie.

- La pressione in un punto non varia al variare del piano che contiene $A^{'}$
### Unità di misura
La pressione, secondo il [[Sistemi di misura#Sistema internazionale|sistema internazionale]] viene misurata in Pascal, $1 [P_{a}]=1 [\frac{N}{m^{2}}]$.
Nel corrente uso, si usa anche l'unità di misura Bar, $1 [bar]=10^{5}[P_{a}]$ oppure l'atmosfera, $1 [atm] = 101.235[P_{a}]$
# Principio di Pascal
Nel caso dei fluidi incomprimibili ideali (liquidi), la pressione si trasmette inalterata in tutte le superfici, questa caratteristica prende il nome di ==isotropia==.
# Strumenti di misura
### Barometro
Permette la misura della pressione rispetto al vuoto, definisce la ==pressione assoluta==.

Consiste in un tubo di vetro chiuso da un lato, avente l'altro lato aperto immerso in un contenitore di liquido (spesso mercurio).
Dopo aver riempito completamente il tubo di mercurio, viene ribaltato immergendo la parte aperta. Appena raggiunto l'equilibrio si avrà un bilanciamento tra il peso della colonna di mercurio di altezza $h$ e sezione $A$ e la forza esercitata dalla pressione atmosferica che si vuole misurare.

### Manometro
Permette la misura della pressione relativa, rispetto alla pressione locale.$$P_{man}=P_{ass}-P_{atm}$$

Consiste in un tubo aperto alla sua sommità e collegato ad un contenitore del fluido del quale si vuole conoscere la pressione.
Basta applicare la [[#Legge di Stevino]], con la quale

### Vacuometro
Permette la misura della depressione relativa rispetto alla pressione atmosferica.$$P_{vac}=P_{atm}-P_{ass}$$
# Variazione di pressione
Facciamo variare la pressione in base all'altezza, e la [[Densità]] $\rho=\rho(z)$.
Pag 17 per la dimostrazione #dimostrazione-da-fare . 
$$\Delta p = g\cdot\int_{z_{2}}^{z_{1}}\rho(z) dz$$
Dove $g$ è l'accelerazione gravitazionale 
# Legge di Stevino
La pressione in un liquido a [[Densità]] costante cresce linearmente con la profondità. 
Possiamo calcolare la variazione di pressione su un volume:
$$\Delta p = g\cdot \rho\cdot\int_{z_{2}}^{z_{1}}dz$$
# Martinetto idraulico
Sfruttando le leggi viste in precedenza, e studiando due cilindri posti in comunicazione idraulica fra loro e definite due sezioni aventi ampiezze diverse, una volta che il sistema si troverà all'equilibrio, le due sezioni si troveranno alla stessa quota e quindi garantiranno che le pressioni $p_{1}=p_{2}$.
Quindi $$\frac{F_{1}}{A_{1}}=\frac{F_{2}}{A_{2}}$$
Allora si deduce che $F_{2}=F_{1}\cdot \frac{A_{2}}{A_{1}}$
Si può allora notare che si può creare un effetto moltiplicativo della forza trasmessa.
