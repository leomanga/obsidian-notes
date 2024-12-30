Il campo elettrostatico è un [[Campo vettoriale]], esiste a prescindere dalla presenza di cariche nello spazio. (Stesso concetto del campo gravitazionale)
Solo alla presenza di una carica si può notare il campo agire come forza elettrostatica([[Elettrostatica#^e120e4|Legge di Culomb]]).

$$
\vec{E}(\vec{r})=\frac{\vec{F_{q}}(\vec{r})}{q}=\frac{k_{\epsilon}Q}{||\vec{r}||^{2}}\vec{r}\quad [\frac{N}{c}][\frac{V}{m}]
$$

^d97f39

Dove $$\vec{F}_{q}=\frac{k_{\epsilon}Qq}{||\vec{r}||^{2}}\cdot \vec{r}\quad [N]$$ ^94c531

($Q$ è una carica grande, mentre $q$ è una carica piccola. La usiamo per pensare l’effetto che potrebbe avere il campo in essa.)

Nel caso di $n$ punti:
$$\vec{E}(\vec{r})=\sum_{i=1}^{n}E_{i}(\vec{r})=k_{\epsilon}\frac{\vec{q}_{1}}{||\vec{r}-\vec{r}_{i}||^3}(r-r_{i})\quad [\frac{N}{c}]$$

>[!prp] Utilizzo della carica elettrica puntiforme
>Se la [[Carica elettrica]] è molto piccola, si può usare il concetto di [[Carica elettrica#^59669a|carica elettrica puntiforme]] $q = \rho(\vec{r})\cdot dv$
>$$\vec{E}(\vec{r})=\iiint_{V}\frac{\rho(\vec{r^{'}})dv}{||\vec{r}-\vec{r^{'}}||^{3}}(\vec{r}-\vec{r^{'}})$$


>[!prp] Utilizzo della carica elettrica lineare
>Se la [[Carica elettrica]] è molto piccola, si può usare il concetto di [[Carica elettrica#^59669a|carica elettrica puntiforme]] $q = \rho(\vec{r})\cdot ds$
>$$\vec{E}(\vec{r})=\iint_{S}\frac{\sigma(\vec{r})ds}{||\vec{r}-\vec{r^{'}}||}(\vec{r}-\vec{r^{'}})$$


>[!prp] Utilizzo della carica elettrica superficiale
>Se la [[Carica elettrica]] è molto piccola, si può usare il concetto di [[Carica elettrica#^59669a|carica elettrica puntiforme]] $q = \lambda(\vec{r})\cdot dl$
>$$\vec{E}(\vec{r})=\int_{L}\frac{\lambda(\vec{r})dl}{||\vec{r}-\vec{r^{'}}||}(\vec{r}-\vec{r^{'}})$$

[[Casi notevoli campi elettrostatici]]

[[Densità volumetrica di carica elettrica#Proprietà]]

[[Potenziale elettrostatico#^334d2b]]

>[!thm] Rotore del campo elettrostatico sempre nullo
>Dato che la circuitazione($\oint_{S}\vec{R}(\vec{r})\cdot dl$) è sempre nulla(\*), allora dal [[Teorema di Stokes]] si ha che 
>$$\nabla\times\vec{E}(\vec{r})=0$$
>(\*): Viene dal fatto che con quell’integrale si sta calcolando una differenza [[Potenziale elettrostatico]] partendo da un punto e finendo nello stesso. Dato che il potenziale non si preoccupa del percorso, si ha che la differenza di potenziale deve essere 0.

