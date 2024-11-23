---
collegamenti:
  - "[[Velocità]]"
  - "[[Capitolo 7 - Cinematica dei moti relativi]]"
aliases:
  - Velocità
---
Da [[Velocità]], sappiamo che la velocità vista dal punto di vista dell'osservatore fisso è
$$\vec{v}=\frac{d\vec{r}}{dt}=\frac{dx_{p}}{dt} \vec{i}+ \frac{dy_{p}}{dt}\vec{j}+ \frac{dz_{p}}{dt} \vec{k}$$
Invece l'osservatore che si muove vedrà il punto materiale muoversi con velocità diversa
$$\vec{v}^{'}=\frac{dx^{'}_{p}}{dt} \vec{i}+ \frac{dy^{'}_{p}}{dt}\vec{j}+ \frac{dz^{'}_{p}}{dt} \vec{k}$$
Molto importante è notare che, dati che per il sistema di riferimento mobile, gli assi del sistema si muovono a loro volta, non possiamo scrivere che $\vec{v}^{'} = \frac{d\vec{r}}{dt}$.

Inoltre la velocità l'origine del sistema di riferimento mobile $0^{'}$ rispetto al sistema fisso è data da
$$
\vec{v}_{0^{'}}=\frac{d\vec{r}_{0^{'}}}{dt}=\frac{dx_{0^{'}}}{dt} \vec{i}+ \frac{dy_{0^{'}}}{dt}\vec{j}+ \frac{dz_{0^{'}}}{dt} \vec{k}
$$

^b8a13a

Possiamo inoltre calcolare 
$$
\frac{d\vec{r^{'}}}{dt}=\vec{v}^{'}+x^{'}_{p}\frac{d \vec{i}^{'}}{dt}+y_{p}^{'}\frac{d \vec{j}^{'}}{dt}+z^{'}_{p}\frac{d \vec{k}^{'}}{dt}
$$

^ae8051

Da notare che $\vec{i}^{'},\vec{j}^{'}, \vec{k}^{'}$ sono versori [[Vettori ortogonali|ortogonali]] e così si mantengono durante il moto.

GUARDA PAG 18-19


>[!def] Velocità angolare
>Dati (guarda pag 18 per vedere come)
>$$\frac{d\vec{i}'}{dt}\cdot \vec{j} = \frac{d\vec{j}'}{dt}\cdot \vec{i} = \omega^{'}_{z} $$
>$$\frac{d\vec{j}'}{dt}\cdot \vec{k} = \frac{d\vec{k}'}{dt}\cdot \vec{j} = \omega^{'}_{x} $$
>$$\frac{d\vec{k}'}{dt}\cdot \vec{i} = \frac{d\vec{i}'}{dt}\cdot \vec{k} = \omega^{'}_{y} $$
>Definiamo il vettore di velocità angolare
>$$\vec{\omega}=\omega^{'}_{x}\vec{i^{'}}+\omega^{'}_{y}\vec{j^{'}}+\omega^{'}_{z}\vec{k^{'}}$$

^eddbc4

>[!prp] Formule di Poisson
>%%display:Formule di Poisson%%
>$$\vec{\omega} \times \vec{i} = \frac{d\vec{i}'}{dt}$$$$\vec{\omega} \times \vec{j} = \frac{d\vec{j}'}{dt}$$$$\vec{\omega} \times \vec{k} = \frac{d\vec{k}'}{dt}$$ 

^c662b4

Da [[#^ae8051]] e con le [[#^c662b4]] possiamo allora scrivere che
$$
\frac{d\vec{r}^{'}}{dt}=\vec{v^{'}}+\vec{\omega}\times\vec{r^{'}}
$$

^c57149

$\vec{v}$ tiene conto di come il punto materiale si muove rispetto al sistema mobile, e viene detta velocità relativa.
$\vec{\omega}\times\vec{r^{'}}$ tiene conto di come il sistema mobile sta ruotando rispetto a quello fisso.

Possiamo inoltre derivare , dalla [[Legge oraria - moti relativi#^90d7fe]] ed utilizzare [[#^b8a13a]] e [[#^c57149]] ![[Legge oraria - moti relativi#^90d7fe]]
Otterremo allora
>[!Def] Velocità nei moti relativi
>%%display:velocità%%
>$$\vec{v}=\vec{v^{'}}+\vec{v_{0}^{'}}+\omega \times\vec{r^{'}}=\vec{v^{'}}+\vec{v_{tr}}$$
>$\vec{v_{tr}}=\vec{v}_{0^{'}}+\omega \times \vec{r^{'}}$ viene detta velocità di trascinamento e tiene conto di come il sistema mobile si muove rispetto a quello fisso

^3c15dd





