Consideriamo un problema con soli vincoli di uguaglianza
$$
\begin{split}\min f(x)\\h(x)=0\end{split}
$$

^a46f2a

Cerchiamo di definire un problema non vincolato
$$\begin{split}\min F(x)\\ x\in \mathbb{R}^{n}\end{split}$$
Lo scopo è quello di creare una funzione $F(x)$ per cui è presente un termine che sparisce se i vincoli [[#^a46f2a]] sono soddisfatti, sennò porta un contributo positivo alla funzione.

Dato $y\in \mathbb{R}^{m}$, sia $p(y)$ una funzione (detta funzione di penalità), tale che $p(y)=0$ se $y=0$ e $p(y)>0$ per $y\not=0$.

Porremo allora $F(x)=f(x)+\rho p(h(x))$, dove $\rho>0$ è un coefficiente opportuno.
Si presuppone che $F(x)$ sia [[Università/Anno 1/Sessione 2/Analisi II/Derivate - spazi metrici#Definizione funzione differenziabile|differenziabile]] nei punti in cui $h(x)=0$. 
Di solito si sceglie $p(y)=y^{T}y$ così da avere
$$F(x)=f(x)+\rho \sum_{i=0}^{m} h_{i}(x)^2$$
Avremo allora l’algoritmo
```
Si fissa un punto iniziale xs qualsiasi; 
k := 0;
while(xs non soddisfa le condizioni di KKT){
	k := k + 1;
	partendo da xs, calcola xk = arg min{f(x) + ρ[k]*sum(h(x)^2});
	xs = x[k]
}
```
