---
collegamenti: "[[Sottospazio lineare]]"
---
# Definizione
Sia $V$ spazio vettoriale e $\mathbb{X}$ e $\mathbb{Y}$, due sottoinsiemi di $V$.
$\mathbb{X}$ è equivalente a $\mathbb{Y}$ e si scrive $\mathbb{X} \sim \mathbb{Y}$ se e solo se $L(\mathbb{X}) = L(\mathbb{Y})$.

# Criteri di equivalenza
1) $\mathbb{X}\setminus \{0\} \sim \mathbb{X} \sim \mathbb{X} \cup \{0\}$
2)  $\mathbb{X} \sim (\mathbb{X} \setminus \{y\}) \cup \{ty\}\qquad \forall y\in\mathbb{X}, \forall t\in\mathbb{K}\{0\}$
3) $\mathbb{X} \sim (\mathbb{X} \setminus \{x\}) \cup \{1\cdot x + ty\}\qquad \forall x\in\mathbb{X}, \forall t\in\mathbb{K}\{0\}$
4) $\forall x,y_1,y_2,\ldots,y_m\in\mathbb{X}$, con $x\not=y_1,y_2,\ldots,y_{m\qquad}\forall t_1,t_2,\ldots,t_m\in\mathbb{K}$
$$\mathbb{X}\sim\mathbb{X}\setminus\{x\}\cup\{1\cdot x+t_1y_1+t_2y_2+\ldots+t_my_m\}$$

6) Se $\mathbb{X}$ contiene 2 [[Dipendenza lineare|Vettori proporzionali]] posso toglierne uno
7) SE $\mathbb{X}$ contiene un valore $z$ tale che è [[Combinazione lineare]] di altri vettori di $\mathbb{X}$, posso togliere $z$.

1)-6) -> modifiche elementari
Esempio:
$$\{A\}\sim\{2A\}\sim\{tA\}_{t\in\mathbb{R}\setminus\{0\}}$$
# Definizione 2
Siano $\alpha=(A_1,A_2,\ldots,A_n)$ e $\beta = (B_1,B_2,\ldots,B_m)$ due [[Sequenza di vettori|sequenze di vettori]] di V.
$\alpha$ è equivalente a $\beta$ e si scrive ($\alpha \approx \beta$) se $\{A_1,A_2,\ldots,A_{n}\}\sim \{B_1,B_2,\ldots,B_m\}$, cioè $L(A_1,A_2,\ldots,A_{n})= L(B_1,B_2,\ldots,B_m)$.


