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
$$\sigma_{p}(\vec{r})=P(\vec{r})\cdot \hat n$$
$$\rho_{p}(\vec{r})=-\sigma\cdot \vec{P}(\vec{r})$$
dove $\vec{P}$ è il [[Vettore polarizzazione]] e $P$ il suo modulo. Mentre $\hat n$ rappresenta il versore normale alla superficie (diretto verso l’esterno).

Il [[Potenziale elettrostatico]] dovuto alle cariche diventerà
$$V_{p}(\vec{r})=k_{e}\oint_{S}\frac{\sigma_{p}(\vec{r})}{|\vec{r}- \vec{r}^{'}|}ds^{'}+k_{e}\iiint_{V}\frac{\rho_{p}(\vec{r})}{|\vec{r}-\vec{r}^{'}|}dv^{'}$$
Il [[Campo elettrostatico]] diventerà
$$\vec{E}_{p}(\vec{r})=k_{e}\oint_{S}\frac{\sigma_{p}(\vec{r})}{|\vec{r}- \vec{r}^{'}|^{3}}ds^{'}+k_{e}\iiint_{V}\frac{\rho_{p}(\vec{r})}{|\vec{r}-\vec{r}^{'}|^{3}}dv^{'}$$

Scrivere suscettività dielettrica pag 19 slides.