# Caso 1 - Funzioni con poli singoli
Data una funzione $f(x)$ lineare, si vuole portare nella forma
$$\sum_{i=1}^{n}     \frac{R_{i}}{x+r_{i}}$$
dove $n$ è il numero di radici reali e complesse e $r_{i}$ è la radice i-esima
## Metodo 1
$$R_{i}=\lim_{x\to r}(x-r)\cdot f(x)$$
# Caso 2 - Funzioni con poli multipli
Data una funzione $f(x)$ lineare, si vuole portare nella forma
$$f(x)=\sum_{i=1}^{n}f_{i}(x)$$
$$\mbox{dove }f_{i}(x)=\frac{R_{i,1}}{x-r_{i}}+\frac{R_{i,2}}{(x-r_{i})^{2}}+\ldots+\frac{R_{i,\mu_{i}}}{(x-r_{i})^{\mu_{i}}}$$
## Metodo
$$R_{i,k}=\frac{1}{(\mu_{i}-k)!}\lim_{s\to p_{i}}\frac{d^{\mu_{i}-k}}{ds^{\mu_{i}-k}}[(x-p_{i})^{\mu_{i}}f(x)]$$
Dove $\mu_{i}$ è la molteplicità della radice $i$-esima e $k=1,\ldots,\mu_{i}$ e $i=1,\ldots,n$

# Caso 3 - Funzioni razionali fratte [[Funzioni proprie e strettamente proprie|proprie]]
Si può sempre scrivere una funzione fratta propria del tipo (importante che il polinomio al denominatore sia monico)
$$f(x)=\frac{a_{n}x^{n}+a_{n-1}x^{n-1}+\ldots+a_{0}}{s^{n}+b_{n-1}x^{n-1}+\ldots+b_{0}}$$
come $$a_{n}+\tilde{f(x)}$$
dove $\tilde{f(x)}$ è il risultato della divisione fra il numeratore ed il denominatore. $a_{n}$ è il resto.
$\tilde{f}(x)$ sarà sicuramente una funzione strettamente propria, quindi sarà possibile utilizzare i casi [[#Caso 1 - Funzioni con poli singoli|1]] e [[#Caso 2 - Funzioni con poli multipli|2]].

