Dato un polinomio, si vuole calcolare in un punto $x\in \mathbb R$
$$P(x) = \sum_{i=0}^{n}a_{i}x^{i}=a_{0}+x(a_{1}+x(a_{2}+\ldots+x(a_{n-1}+x a_{n}))\ldots)$$
```python
x = PUNTO
a = VETTORE CHE RAPPRESENTA I VALORI DEL POLINOMIO

s = a[n]
for i in range(n):
	s = s*x + a[n-i-1]
```

Algoritmo ottimale, $n$ moltiplicazioni + $n$ addizioni.
Impossibile fare di meglio.