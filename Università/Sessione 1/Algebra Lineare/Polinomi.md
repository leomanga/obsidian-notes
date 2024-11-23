---
pagina: 23
collegamenti:
  - "[[Monomi]]"
---
# Definizione
Un polinomio è una somma di [[Monomi]].
- Un polinomio è omogeneo se tutti i monomi che lo compongono hanno lo stesso grado
- Il grado di un polinomio è il massimo grado dei monomi.
- Generico polinomio di grado $n$
$$a_0+a_1x_1+a_2x_2^2+\ldots+a_nx_n^n$$
# Riducibilità di un polinomio
Sia $\mathbb{K}[x]=\{a_0+a_1x_1+a_2x_2^2+\ldots+a_nx_n^{n}:a_{i}\in\mathbb{K},n\in\mathbb{N}\}$l'insieme di tutti i polinomi a coefficienti in $\mathbb{K}$ nella variabile $x$.
Un polinomio $P(x)\in \mathbb{K}[x]$ si dice che è RIDUCIBILE in $\mathbb{K}$ se è possibile scrivere $P(x)$ come prodotto di polinomi a coefficienti in $\mathbb{K}$ di grado maggiore di $0$.
- es: $x^2+5x+6=(x+3)(x+2)$

# Radice o zero di un polinomio
Sia $P(X)\in\mathbb{K}[x]$
$a\in\mathbb{K}$ Si dice RADICE O ZERO del polinomio $P(x)$ se e solo se $(x-a\mid P(x))$(ovvero se $x-a$ divide $P(x)$)
Cioè $P(x)=(x-a)\cdot Q(x)$
### Molteplicità algebrica
La molteplicità algebrica è il massimo numero naturale tale che $(x-a)^m|P(x)$

# Corollario 1
Se $\varphi(x)=\sum_{i=0}^{n}a_{i}x^{i}$ e $\psi(x)=(x-b)$
Allora per trovare il resto della divisione di $\varphi(x)$ per $\psi(x)$ basta calcolare $\varphi(b)$
#dimostrazione-da-fare 

# Teorema fondamentale dell'algebra
Ogni polinomio in una variabile a coefficienti in $\mathbb{C}$ di grado $n$ ammette $n$ zeri contati con la propria molteplicità algebrica

# Corollario 2
Se $\varphi(x)\in \mathbb{C}[x]$ allora $\varphi(x)=prod_{i=1}^{r}(x-b_{i})^{m_{i}}$ dove $m_i$ è la molteplicità algebrica di $b_{i}$
$deg(\varphi(x))=\sum_{i=1}^{r}m_{i}$

- se $deg(\varphi(x))$ è dispari allora ammette almeno una radice reale