---
aliases:
  - IO
---
Rappresenta una o più equazioni differenziali che mettono in relazione le [[variabili di ingresso]] e le [[variabili di uscita]] e le loro derivate.
Si intende sia per [[Sistemi SISO]] che per [[Sistemi MIMO]].

$$h(u(t),\dot{u}(t), \ddot{u}(t),\ldots,u^{(m)}(t),y(t),\ldots,y^{(p)}(t),t)=0$$

$u$ sono le variabili di ingresso
$y$ sono le variabili di uscita

>[!prp] Rappresentazione nei sistemi [[Sistemi lineari tempoinvarianti|LTI]]
>$$\begin{split}&y^{n}(t)+a_{n-1}y^{(n-1)}+\ldots+a_{1}\dot{y}(t)+a_{0}y(t)=\\
>& =b_{m}^{(m)}+b_{m-1}u^{(m-1)}+\ldots+b_{1}\dot{u}(t)+b_{0}u(t)
>\end{split}$$

^2ade95

>[!prp] Trasformata di Laplace
>$$Y(s)=\underbrace{\frac{c_{n-1}s^{n-1}+c_{n-2}s^{n-2}+\ldots + c_{0}}{s^{n}+a_{n-1s^{n-1}+\ldots+a_1s+a_{0}}}}_{Y_{l}(s),\ risposta\ libera}+\underbrace{\frac{b_{m}s^{m}+b_{m-1}s_{m-1}+\ldots+b_{1}s+b_{0}}{s^{n}+a_{n-1}s^{n-1}+\ldots+a_{1}s+a_{0}}}_{Y_{f(s)},\ risposta\ fissa}U(s)$$
>Dove $c_{i}$ sono combinazioni lineari di $y(0), \dot{y}(0),\ldots,y^{n-1}(0)$
>
>- $Y_{l}(s)$ viene chiamata **risposta libera**, la quale è influenzata solo dai dati iniziali.
>- $Y_{f}(s)$ è la **[[Risposta forzata]]**
>  Infatti $Y_{f}(s)=G(s)\cdot U(s)$ dove $U(s)$ è la trasformata della funzione di ingresso, mentre $G(s)$ viene chiamata **funzione di trasferimento del sistema**.
>  
>  Per la [[Proprietà di un sistema dinamico#^5c80d6|causalità]], $n\ge m$, quindi $G(s)$ è sempre [[Funzioni proprie e strettamente proprie|propria o strettamente propria]].
>  
>[[Trasformata di Laplace]]

^84e975
# Tempo discreto
#TODO 
$$G(z)=\frac{b_{0}z^{m}+b_{1}z^{m-1}+\ldots + b_{m}z^{n-m}}{z^{n}+a_{1}z^{n-1}+\ldots+a_{n}}$$
