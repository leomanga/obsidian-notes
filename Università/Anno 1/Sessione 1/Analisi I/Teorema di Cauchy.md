---
collegamenti:
  - "[[Derivate]]"
capitolo: 17
---
# Teorema
Se $f$ e $g$ sono due funzioni reali definite in un intervallo chiuso e limitato $[a,b]$ e derivabili in ogni punto di $[a,b]$, allora esiste almeno un punto $c\in(a,b)$ tale che
$$f^{'}(c)(g(b)-g(a))=g^{'}(c)(f(b)-f(a))$$
#dimostrazione 
Poniamo
$$F(x):=f(x)(g(b)-g(a))-g(x)(f(b)-f(a))$$
La funzione $F$ è derivabile in $[a,b]$, e $F(a) = F(b)$ (basta provare a calcolare).
Applichiamo il [[Teorema di Rolle]] alla funzione $F$ e si ottiene che esiste $c\in(a,b)$ tale che $F^{'}(c)=0$, quindi i due estremi devono essere uguali.

