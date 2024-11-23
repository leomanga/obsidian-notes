---
pagina: 11
aliases:
  - completo
---
# Definizione | Spazio metrico completo
Lo spazio metrico $(X,d)$ si dice completo se ogni [[Successione di Cauchy#Caso generale negli spazi metrici|successione di Cauchy]] risulta convergente.
### Osservazione
Nei reali ogni [[Successione di Cauchy#Caso generale negli spazi metrici|successione di Cauchy]] è convergente, allora $\mathbb{R}$ è completo.
### Esempio
$\mathbb{Q}\subseteq \mathbb{R}$ e considero $\mathbb{Q}$ come spazio metrico.
Allora $\mathbb{Q}$ non è completo, dato che basta prendere una successione di numeri razionali $q_n$ tale che $q_{n}\to\sqrt 2$.
Il limite non esiste in $\mathbb{Q}$, mentre esiste in $\mathbb{R}$.
# Lemma 1![[Successione di Cauchy#Lemma convergente $ Rightarrow$ successione di Cauchy]]
# Lemma 2| successione convergente $\Rightarrow$ le sottosuccessioni convergono
Supponiamo $(X,d)$ [[Spazi metrici|spazio metrico]] e supponiamo $(x_n)\subseteq X$ [[Successione di Cauchy#Caso generale negli spazi metrici|successione di Cauchy]].  
Supponiamo che $\exists (x_{n_{k}})$ convergente a qualche $x\in X$.
Allora tutta la successione $x_{n}$ converge a $x$.
#dimostrazione-da-fare 
# Corollario | completo $\iff$ chiuso
Sia $(X,d)$ [[Spazi metrici|spazio metrico]] [[Spazio metrico completo|completo]] e sia $E\subseteq X$.
Allora lo spazio $(E,d)$ è completo se e solo se è [[Chiusura di un insieme - spazi metrici#Definizione insieme chiuso|chiuso]].
![[Dimostrazione corollario pag 12.jpg]]
