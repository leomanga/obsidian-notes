---
aliases:
  - Materiali dielettrici
---
Fra i materiali isolanti troviamo le plastiche, il vetro e l’ambra.
Questi materiali sono formati da atomi con un’elevata energia di legame, la quale non permette agli elettroni di muoversi liberamente.
Rimane comunque la possibilità di “strappare” elettroni grazie a forze molto intense come lo strofinio o campi molto intensi. Strappando elettroni si avrà l’effetto di lasciare [[Carica elettrica|cariche]] positive localizzate.

# Polarizzazione per deformazione
In un materiale dielettrico, in presenza si un campo elettrico, si avrà una deformazione di ogni atomo parallelamente al campo esterno ([[Polarizzazione per deformazione]]).
In questo caso il valor medio del momento di dipolo sarà diverso da zero.

# Sostanza formata da molecole polari, polarizzazione per orientamento
Una sostanza dielettrica formata da molecole polari, in assenza di campi elettrici non produce nessun effetto elettrostatico macroscopico, dato che il valor medio del momento di dipolo è nullo. (Questo è dovuto dal fatto che le molecole sono orientate in modo casuale)

Nel caso in cui la sostanza viene sottoposta all’effetto di un campo, le molecole tenderanno ad orientarsi parallelamente al campo e la sostanza sarà **polarizzata per orientamento**.

# Vettore di polarizzazione, potenziale e campo elettrico in un dielettrico
In un dielettrico polarizzato, il [[Vettore polarizzazione]] è diverso da 0 in ogni punto.
Allora nel dielettrico si presenterà una densità di carica $\vec{\rho}_{p}$ volumetrica ed una superficiale $\vec{\sigma_{p}}$.

![[Pasted image 20241212124120.png]]

Avremo
$$
\sigma_{p}(\vec{r})=P(\vec{r})\cdot \hat n
$$

^78e72d

$$
\rho_{p}(\vec{r})=-\nabla\cdot \vec{P}(\vec{r})
$$

^6a35b4

dove $\vec{P}$ è il [[Vettore polarizzazione]] e $P$ il suo modulo. Mentre $\hat n$ rappresenta il versore normale alla superficie (diretto verso l’esterno).

Il [[Potenziale elettrostatico]] dovuto alle cariche diventerà
$$V_{p}(\vec{r})=k_{e}\oint_{S}\frac{\sigma_{p}(\vec{r})}{|\vec{r}- \vec{r}^{'}|}ds^{'}+k_{e}\iiint_{V}\frac{\rho_{p}(\vec{r})}{|\vec{r}-\vec{r}^{'}|}dv^{'}$$
Il [[Campo elettrostatico]] diventerà
$$\vec{E}_{p}(\vec{r})=k_{e}\oint_{S}\frac{\sigma_{p}(\vec{r})}{|\vec{r}- \vec{r}^{'}|^{3}}ds^{'}+k_{e}\iiint_{V}\frac{\rho_{p}(\vec{r})}{|\vec{r}-\vec{r}^{'}|^{3}}dv^{'}$$

Scrivere suscettività dielettrica pag 19 slides. #da-finire
# Gauss nei dielettrici
Se ipotizziamo di avere un [[Materiali conduttori|conduttore]] con una carica $Q_{f}$ distribuita sulla sua superficie all’interno di un dielettrico, possiamo racchiudere il tutto con una superficie di Gauss.

Avremo allora dal [[Teorema di Gauss]] in forma differenziale che $$\nabla \cdot \epsilon_{0}\vec{E}(\vec{r})= \rho_{f}(\vec{r}) +\rho_{p}(\vec{r})$$
Da [[#^6a35b4]], possiamo scrivere 
$$\nabla\cdot [\epsilon_{0}\vec{E}(\vec{r})+\vec{P}(\vec{r})]=\rho_{f}(\vec{r})$$
Definendo l’[[Induzione elettrica]] $\vec{D}(\vec{r})=\epsilon_{0}\vec{E}(\vec{r})+\vec{P}(\vec{r})$, possiamo scrivere che $\nabla\cdot \vec{D}(\vec{r}))=\rho_{f}(\vec{r})$
Integrando ora sul volume $V$ racchiuso dalla superficie di Gauss ed applicando il [[Flusso di un campo vettoriale#^6d04f9|teorema della divergenza]] avremo che
$$Q_{f}=\oint_{S}\vec{D}(\vec{r})\cdot \hat nds=\iiint_{V}\rho_{f}(\vec{r})dv$$
dove $S$ e $V$ sono le misure della superficie di Gauss.

