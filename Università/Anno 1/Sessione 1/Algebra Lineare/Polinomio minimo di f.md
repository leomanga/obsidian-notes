---
pagina: 291
aliases:
  - Polinomio di Hamilton Cayley
collegamenti:
  - "[[Polinomio caratteristico]]"
  - "[[Matrice di Jordan o Forma di Jordan]]"
---
# Definizione
Sia $\varphi:V\to V$ [[Trasformazione lineare#Endomorfismo|endomorfismo]]
Il polinomio minimo di $\varphi$ ($P_{min}(\varphi)$) (detto anche polinomio di Hamilton Cayley) è il polinomio monico(il termine di grado massimo è 1) di grado minimo che si annulla in $\varphi$.
Cioè se $g(t)$ è un polinomio tale che $g(\varphi)=0$ allora $P_{min}| g(t)$

$P_{min}(\varphi)=\prod_{ai}(t-a_i)^{h_{i}}$ dove $a_{i}$ sono gli [[Autovettori - autovalori - autospazi|autovalori]] di $\varphi$ e $h_{i}$ è la massima grandezza dei blocchi di Jordan dell'autovalore $a_{i}$

$P_{min}(\varphi)|\underbrace{P_{car}(\varphi)}_{polinomio\ caratteristico}$
# Proposizione
[[Proprietà e definizioni matrici#^a469d1]]
