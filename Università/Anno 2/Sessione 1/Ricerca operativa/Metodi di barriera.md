Consideriamo un problema con soli vincoli di disuguaglianza
$$
\begin{split}\min f(x)\\g(x)\ge0\end{split}
$$

^91625d

Indichiamo con $X$ l’interno della regione ammissibile, ovvero
$$INT(X)=\{x\in \mathbb{R}^{n}:g(x)>0\}$$
Ipotizziamo chiaramente che $INT(X)$ sia non vuota.
Una funzione barriera per l’insieme ammissibile del problema [[#^91625d]], è una funzione $v(x)$ continua in $INT(X)$ tale che $v(x)\to \infty$ man mano che $x$ si avvicina alla frontiera di $X$. 
Dovremo minimizzare allora la funzione $$F(X,\epsilon)=f(x)+\epsilon v(x)$$
Lo scopo è quello di impedire ad un punto che si trova in $INT(X)$ di uscire dalla regione ammissibile. Più grande è $\epsilon$, più l’effetto barriera è maggiore.
Come funzione barriera $v(x)$ viene usata
$$v(x)=-\sum_{i=m+1}^{m+p}\log(g_{i}(x))$$
Avremo allora l’algoritmo

```
Si fissa un punto iniziale xs ∈ INT(X); 
k := 0;
while(xs non soddisfa le condizioni di KKT){
	k := k + 1;
	partendo da xs, calcola xk = arg min{f(x)+ ϵ[k]*v(x)};
	xs = x[k]
}
```