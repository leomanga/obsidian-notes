---
collegamenti:
  - "[[Teorema fondamentale del calcolo integrale#Definizione 19.2.3 Primitiva]]"
---
# Definizione
Si dice integrazione indefinita, l'operazione che consiste nel calcolo delle primitive di una funzione continua. Si indica con
 $$\int f(x)dx$$
# Integrazione per decomposizione
Se possiamo scrivere la funzione $f$ come somma di due funzioni $f_{1}$ e $f_2$, allora la primitiva di $f$ sarà uguale ala primitiva di $f_1$ + la primitiva di $f_2$.
$$\int[f_1(x)+f_2(x)]dx=\int f_{1(x)}dx+\int f_{2}dx=g_1+g_2+c$$
# Integrazione per parti
#dimostrazioni 
Dato che per [[Derivate#Derivata del prodotto]]
$$(fg)^{'}=f^{'}g+fg^{'}$$
integrando da entrambi i lati
$$\int_{a}^{b}(f(x)g(x))^{'}dx=\int_{a}^{b} f^{'}(x)g(x)dx+\int_{a}^{b}f(x)g^{'}(x)dx$$
da [[Teorema fondamentale del calcolo integrale#Proposizione 19.2.5 Calcolo di integrali definiti]]
$$f(b)g(b)-f(a)g(a)= \int_{a}^{b} f^{'}(x)g(x)dx+\int_{a}^{b}f(x)g^{'}(x)dx$$
oppure
$$\int_{a}^{b}f(x)g^{'}(x)dx= -\int_{a}^{b} f^{'}(x)g(x)dx +f(b)g(b)-f(a)g(a)$$
# Integrazione per sostituzione integrali definiti
Sia $f:I\to\mathbb{R}$ una [[Funzioni continue|funzione continua]]. 
Siano $J$ un intervallo e $\varphi:J\to I$ una funzione [[Derivate#Definizione Derivata di una funzione in un punto|derivabile]] con derivata continua, e $\alpha$ un punto di $J$. Allora
$$\int_{\varphi(\alpha)}^{\varphi(s)}f(x)dx = \int_{\alpha}^{s}f(\varphi(t))\varphi^{'}(t)dt\quad \forall y \in I$$ Inoltre se $\varphi$ è bigettiva e se $a$ è un punto di $I$,
$$\int_{a}^{y}f(x)dx=\int_{\varphi^{-1}(a)}^{\varphi^{-1}(y)}f(\varphi(t))\varphi^{'}(t)dt\quad \forall y\in I$$
		#dimostrazione-da-fare 

# Integrazione sostituzione integrali indefiniti
$$\int h(u(x))u^{'}(x)dx=\left[\int h(u)du\right]_{u=u(x)}$$