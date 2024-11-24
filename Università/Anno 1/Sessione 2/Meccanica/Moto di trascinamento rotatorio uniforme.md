Nel moto di trascinamento rotatorio uniforme l'origine del sistema di riferimento mobile e l'origine di quello fisso sono uguali.
Invece due assi si muovono, in questo caso $x^{'}$ e $y^{'}$, rispetto a $x$ e $y$ con [[Velocità - moti relativi#^eddbc4|velocità angolare]] costante.
![[Moto di trascinamento rotatorio uniforme.png]]

# Posizione
Sappiamo la [[Legge oraria - moti relativi|Posizione]] è data da
![[Legge oraria - moti relativi#^90d7fe]]

Dato che i due sistemi hanno la stessa origine, $\vec{r}_{O^{'}}=0$.
Quindi
>[!def] Posizione del moto di trascinamento rotatorio uniforme
>$$\vec{r}=\vec{r^{'}}$$
>NOTA: Le due rappresentazioni sono diverse nei due sistemi di riferimento.
>$\vec{r}=x_{p}\vec{i}+y_{p}\vec{j}$ e $\vec{r^{'}}=x_{p}^{'}\vec{i^{'}}+y_{p}^{'}\vec{j}^{'}$

# Velocità
Ricordiamo che la [[Velocità - moti relativi|Velocità]] è data da
![[Velocità - moti relativi#^3c15dd]]

Inoltre ricordiamoci le [[Velocità - moti relativi#^c662b4]]
![[Velocità - moti relativi#^c662b4]]

Dato che $\vec{k^{'}}$ è fisso, $\vec{\omega}\times \vec{k^{'}} = \frac{d\vec{k^{'}}}{dt} =  0$, quindi $\vec{\omega}$ è parallelo a $\vec{k^{'}}=\vec{k}$.
Potremo allora scrivere $$\vec{\omega}=\omega\vec{k}$$.

Inoltre, dato che i due sistemi hanno l'origine in comune, $\vec{v}_{O^{'}}=0$, risultando quindi che  
$$
\vec{v}_{tr}=\vec{\omega}\times \vec{r}
$$
Allora possiamo definire la velocità
>[!def] Velocità nel moto di trascinamento rotatorio uniforme
>$$\vec{v} =\vec{v^{'}}+\vec{v}_{tr}=\vec{v^{'}}+\vec{\omega}\times\vec{r}$$

# Accelerazione
Ricordiamo che l'[[Accelerazione - moti relativi|Accelerazione]] è data da
![[Accelerazione - moti relativi#^2f665c]]

Come nel caso della velocità, dato che i due sistemi hanno origine comune, $\vec{a}_{O^{'}}=0$.
Inoltre, essendo il moto rotatorio, uniforme, la [[Velocità - moti relativi#^eddbc4|velocità angolare]] è costante e quindi $\frac{d\vec{\omega}}{dt}=0$.

Avremo quindi
>[!def] Accelerazione nel moto di trascinamento rotatorio uniforme
>$$\vec{a}=\vec{a^{'}}+\vec{\omega}\times(\omega\times \vec{r^{'}})+2\vec{\omega}\times\vec{v^{'}}$$
>Si evidenzia che $\vec{a}_{tr}=\omega\times(\omega\times\vec{r^{'}})=\omega\times(\omega\times\vec{r})$.
>Inoltre l'accelerazione di Coriolis, $\vec{a_{c}}=2\omega\times\vec{v^{'}}$, sarà perpendicolare a $\vec{v^{'}}$. 
>