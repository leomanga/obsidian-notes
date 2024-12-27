![[Magnetostatica nel vuoto#^b6258f]]

Per trovare $\vec{B}(\vec{r})$ basta integrare.

>[!prp]
>$$\nabla\times \vec{B}(\vec{r})=\mu_{0}\cdot\vec{J}(\vec{r})$$
>dove $\vec{J}$ è la [[Densità di corrente elettrica]]
>La dimostrazione è con il [[Teorema di Stokes]]. (guarda appunti 13/12 Ipad vitto).

>[!prp]
>$$\nabla\cdot \vec{B}(\vec{r})=0$$
>
# Legge della circuitazione di Ampere

![[Legge della circuitazione di Ampere.excalidraw]]

Ho un filo infinito, e un cammino in un piano ortogonale al filo.
Voglio calcolare
$$\int_{C}^{D}\vec{B}(\vec{r})\cdot d\vec{l}$$
Da [[Magnetostatica nel vuoto#Filo infinito Legge di Biot-Savart]] so che $\vec{B}(\rho)=\frac{\mu_{0}}{2\pi}\frac{I}{\rho}\hat \phi$
Allora $$\vec{B}(\rho)d\vec{l}=\frac{\mu_{0}}{2\pi}\frac{I}{\rho}\hat \phi\cdot(d\rho\hat{\rho}+\rho d\phi\hat\phi)=\frac{\mu_{0}}{2\pi}Id\phi$$
Allora, non essendoci dipendenza da $\rho$
$$\int_{C}^{D}\vec{B}(\vec{r})d\vec{l}=\int_{\phi_{C}}^{\phi_{D}}\frac{\mu_{0}}{2\pi}Id\phi = \frac{\mu_{0}}{2\pi}I(\phi_{D}-\phi_{C})$$
Se come percorso avessi $C$ e $D$ sovrapposti, quindi facessi un giro completo, allora $\phi_{D} =2\pi+\phi_{C}$
Allora se il filo è dentro la circuitazione 
$$\oint \vec{B}(\vec{r})d\vec{l}=\pm\mu_{0}I$$
Se il filo è fuori alla circuitazione
$$\oint \vec{B}(\vec{r})d\vec{l}=0$$
Dato che non sempre la circuitazione è pari a 0, allora il campo di induzione magnetica non è conservativo.
