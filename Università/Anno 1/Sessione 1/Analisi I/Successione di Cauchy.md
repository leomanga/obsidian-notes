---
capitolo: 9
collegamenti: "[[Successioni e limiti infiniti]]"
---
# Caso in $\mathbb{R}$
Una successione reale $a_n$ si dice di Cauchy se
$$\forall \epsilon > 0 \ \ \exists \nu_{\epsilon}\in \mathbb{N}:\forall n \in \mathbb{N}, n > \nu_{\epsilon},\ \ \forall m \in \mathbb{N}, m > \nu_{\epsilon} \ \ \ \ \ |a_{n}- a_{m}|<\epsilon$$

In questa definizione non appare nessun ente esterno, cosa che appariva prima, cioè il limite $\ell$. (Ref: [[Successioni e limiti finiti#Limite finito]])

## Teorema | Successione di Cauchy $\iff$ successione convergente
Sia $a_n$ una successione di numeri reali. Sono equivalenti:
1) $a_n$ è convergente
2) $a_n$ è di Cauchy
#dimostrazione-da-fare Prima implicazione facile, seconda difficile

# Caso generale negli spazi metrici
Sia $(x_n)\subseteq X$ una successione in uno [[Spazi metrici|Spazio metrico]] $(X,d)$.
Allora $x_n$ si dice di Cauchy se:
$$\forall \epsilon>0\ \exists N_\epsilon\in\mathbb{N}:\ \forall n,m\ge N_{\epsilon},d(x_{n},x_{m})\le \epsilon$$
## Lemma | convergente $\Rightarrow$ successione di Cauchy
In qualsiasi spazio metrico, ogni successione $x_n$ convergente è anche di Cauchy.
Il viceversa è vero se e solo se $(X,d)$ è [[Spazio metrico completo|completo]].