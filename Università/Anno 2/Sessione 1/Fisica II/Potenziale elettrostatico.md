---
aliases:
  - Volt
  - volt
---
# Calcolo del potenziale per carica unitaria
## Calcolo del lavoro
Dato che da [[Campo elettrostatico#^d97f39]],  $\vec{F}_{el}=\vec{E}(\vec{r})\cdot q$, allora essendo $q=1$ abbiamo
$$\vec{F}_{el} = \vec{E}(\vec{r})$$
Allora avremo che il [[Lavoro]] elettrostatico infinitesimo $dL_{el}$ sarà
$$dL_{el}=\vec{F}_{el}\cdot d\vec{l}=\vec{E}(\vec{r})\cdot d\vec{l}$$
Il lavoro fatto da un esterno possiamo esprimerlo come
$$dL_{at}=-d\vec{L}_{el}$$

Il lavoro totale compiuto per portare la carica da un punto $A$ ad un punto $B$ sarà quindi
$$L_{AB}=-\int_{A}^{B}\vec{E}(\vec{r})\cdot d\vec{l}=\int_{B}^{A}\vec{E}(\vec{r})\cdot d\vec{l}$$
dove l’integrale rappresenta l’integrale curvilineo.
Passando in coordinate sferiche possiamo scrivere $d\vec{l}=dr\hat{r}+rd\theta\hat\theta+r\sin(\theta)d\phi\hat\phi$ ([[Coordinate sferiche#^ce13bf]])
Inoltre il campo generato in un punto $\vec{r}$  è $\vec{E}(\vec{r})=\frac{1}{4\pi\epsilon_{0}} \frac{Q}{r^{2}}\hat r$ .
Allora avremo 
$$\begin{split}&dL_{at}=\\&&-\vec{E}(\vec{r})\cdot d\vec{l} =-\vec{E}(\vec{r})\cdot(dr\hat{r}+rd\theta\hat\theta+r\sin(\theta)d\phi\hat\phi)=-E(\vec{r})dr \\&= -\frac{1}{4\pi\epsilon_{0}}\frac{Q}{r^{2}} dr\end{split}
$$
## Il lavoro non dipende dal cammino
Se prendiamo $r_{a}$ ed $r_{b}$ i punti di partenza e di arrivo della carica avremo 
$$
L_{at}=-\int_{r_{a}}^{r_{b}}dL_{at}dr=-\frac{1}{4\pi\epsilon_{0}}Q\int_{r_{a}}^{r_{b}}\frac{1}{r^{2}}dr=\frac{Q}{4\pi\epsilon_{0}}(\frac{1}{r_{b}}- \frac{1}{r_{a} })
$$

^49268c

Allora notiamo che $L_{at}$ non dipende dal percorso, ma solo dai punti iniziali e finali.
**Dal principio dei sovrapposizione degli effetti, ciò vale anche per più cariche**

## Definizione del potenziale elettrostatico
>[!def] Potenziale elettrostatico
>Si definisce il potenziale elettrostatico $V(P)$ come il lavoro tra $P$ ed un punto $P_{0}$ + la costante $V(P_{0})$
>$$V(p)=-\int_{P_{0}}^{P}\vec{E}(\vec{r})\cdot d\vec{l}+ V(P_{0})$$
>Da [[#^49268c]], ipotizzando che $V(P_{0})=0$ (mandando $P_{0}$ ad infinito), avremo
>$$V(\vec{r})=\frac{1}{4\pi\epsilon_{0}}\frac{Q}{r}\quad [\frac{J}{c}]=[V]$$
>Dove $[V]$ sono i Volt

>[!prp] Relazione tra potenziale elettrostatico e [[Campo elettrostatico]]
>$$\vec{E}(\vec{r})=-\nabla V(x,y,z)$$

^334d2b
