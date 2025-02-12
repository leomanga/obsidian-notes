Il metodo iterativo più semplice
## Ipotesi
- $f(x)$ continua nell’intervallo $[a,b]$
- $f(a)f(b)<0$
Per [[Funzioni continue#Esistenza degli zeri]] avremo almeno una soluzione $\alpha$ di $f(x)=0$ in $(a,b)$

## Procedimento
SI divide ad ogni passo l’intervallo $[a,b]$ a metà e si determina in quale dei due sottointervalli si trova la soluzione

## Algoritmo
Poniamo $a_{0}:= a$, $b_{0}:= b$
Per $i=0,1,\ldots,nmax$ si calcola
$$x_{i}:=\frac{a_{i}+b_{i}}{2}$$
Se $f(x_{i})\cdot f(a_{i})\Rightarrow a_{i+1}:= a_{i},b_{i+1}:= x_{i}$
Altrimenti se $f({x_{i}})\cdot f(b_{i})< 0\Rightarrow a_{i+1}:= x_{i},b_{i+1}:= b_{i}$
Altrimenti se $f(x_{i})=0\Rightarrow x_{i}= \alpha$

Il procedimento viene arrestato se per un indice $i$ risulta
$|f(x_{i})| \le toll$ oppure $|a_{i}-b_{i}|\le toll$

## Convergenza
Il metodo della bisezione converge globalmente alla soluzione.
La convergenza però è lenta