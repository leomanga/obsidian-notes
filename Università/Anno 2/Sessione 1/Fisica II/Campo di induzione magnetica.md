![[Magnetostatica nel vuoto#^b6258f]]

Per trovare $\vec{B}(\vec{r})$ basta integrare.

>[!prp]
>$$\nabla\times \vec{B}(\vec{r})=\vec{J}(\vec{r})$$
>dove $\vec{J}$ è la [[Densità di corrente elettrica]]
# Legge della circuitazione di Ampere

Ho un filo infinito, e un cammino in un piano ortogonale al filo.
Voglio calcolare
$$\int_{C}^{D}\vec{B}(\vec{r})\cdot d\vec{l}$$
Da [[Magnetostatica nel vuoto#Filo infinito Legge di Biot-Savart]] so che $\vec{B}(\rho)=\frac{\mu_{0}}{2\pi}\frac{I}{\rho}\hat \phi$
Allora $$\vec{B}(\rho)d\vec{l}=\frac{\mu_{0}}{2\pi}\frac{I}{\rho}\hat \phi\cdot(d\rho\hat{\rho}+\rho d\phi\hat\phi)=\frac{\mu_{0}}{2\pi}Id\phi$$
Allora, non essendoci dipendenza da $\rho$
$$\int_{C}^{D}\vec{B}(\vec{r})d\vec{l}=\int_{\phi_{C}}^{\phi_{D}}\frac{\mu_{0}}{2\pi}Id\phi = \frac{\mu_{0}}{2\pi}I(\phi_{D}-\phi_{C})$$
Se come percorso facessi $D\to C$, allora $\phi_{D} =2\pi+\phi_{C}$
Allora se il filo è dentro la circuitazione 
$$\oint \vec{B}(\vec{r})d\vec{l}=\pm\mu_{0}$$
Se il filo è fuori alla circuitazione
$$\oint \vec{B}(\vec{r})d\vec{l}=\begin{cases}\mu_{0}\sum_{i=1}^{n}(\pm I_{i})\\0\end{cases}$$



