---
collegamenti:
  - "[[Variabili di scambio]]"
---

Il lavoro si calcola come una [[Forza]] per uno spostamento.
	$$\begin{split}W &= p\cdot A=\\&=\vec{F}\cdot \Delta L=\int_{A}^{B}\vec{F}d\vec{s}=\\&=\underbrace{E_{kB}-E_{kA}}_{in\ caso\ ci\ sia\ solo\ questa\ energia}=\\&=\underbrace{E_{pB}-E_{pA}}_{in\ caso\ ci\ sia\ solo\ questa\ energia}\end{split}\qquad[N \cdot m]=[kg\cdot \frac{m^{2}}{s^{2}}]=[J]$$
Dove $N$ sono i [[Forza|Newton]], $m$ i metri e $s$ i [[Tempo|secondi]].
$p$ è la [[Pressione]].
$A$ è una superficie.
$d\vec{s}$ è lo spostamento infinitesimo. $E_{k}$ è l'[[Energia cinetica]]
$J$ sono i Joule.
Al lavoro si associa il concetto di [[Potenza]].

> Lavoro in [[#Meccanica]]
> Lavoro in [[#Termodinamica]]

---
# Meccanica
Il lavoro dipende dalla forza e dal percorso del punto materiale in un determinato intervallo.
Consideriamo lo spostamento infinitesimo $d\vec{s}$.
Si definisce lavoro infinitesimo
$$d W = \vec{F}\cdot d\vec{s}$$
Per la definizione del [[Prodotto scalare]],
$$dW=F\cdot ds\cos\vartheta$$
Dove $\vartheta$ è l'angolo che la forza $\vec{F}$ forma con lo spostamento $d\vec{s}$.

Inoltre studiando il lavoro (pag 10) meccanica, possiamo vedere che $$dW=m\cdot v\cdot dv$$
Dove $m$ è la [[Massa]], $v$ la [[Velocità]] e $dv$ è la variazione di velocità infinitesima.
A questo punto integrando fra due punti troviamo che
$$W=\frac{1}{2}mv_{b}^{2}-\frac{1}{2}mv_{a}^{2}=E_{kb}-E_{ka}$$
Dove $E_{k}$ è l'[[Energia cinetica]]

Inoltre possiamo scrivere 
$$W=-mg(z_{b}-z_{a})=E_{p}$$
Dove $E_{p}$ è l'[[Energia potenziale della forza peso]].
Si noti che se il punto materiale scende verso il basso, il lavoro è positivo, sennò è negativo.

# Termodinamica
In termodinamica si definisce il lavoro applicato su un sistema fluido.
Particolare interesse hanno le trasformazioni termodinamiche applicate ai fluidi comprimibili, e parleremo in questo caso di lavoro di compressione o lavoro di espansione.

## Caso di compressione
Consideriamo una sostanza gassosa contenuta all'interno di un [[Sistema termodinamico]] chiuso e adiabatico.
All'equilibrio sul gas viene esercitata una [[Forza]] 
$$
F = p\cdot A
$$
Se viene effettuata una compressione attraverso trasformazioni quasi statiche fino ad avere uno spostamento infinitesimo del pistone $-dy$, il lavoro $\delta W$ compiuto sul fluido sarà:
$$
\delta W=F\cdot(-dy)=p\cdot A\cdot (-dy)=-p\cdot \underbrace{dV}_{variazione\ negativa}
$$

^6902eb

Prendendo in considerazione un istante iniziale $i$ ed uno finale $f$ di una trasformazione di compressione in cui il sistema assume un [[Volume]] rispettivamente di $V_{i}$ e $V_{f}$, ==il lavoro effettuato complessivamente== su o dal sistema sarà pari a 
$$
W = \int_{i}^{f}\delta W=-\int_{V_{i}}^{V_{f}}p\cdot dV=-\int_{V_{i}}^{V_{f}}p(V)\cdot dV
$$

^4706bb

- [[Potenza]].