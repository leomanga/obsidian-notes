---
capitolo: 10
collegamenti: "[[Serie numeriche a termini di segno costante]]"
---
A differenza delle [[Serie numeriche a termini di segno costante]], dove tutto si basava sul concetto di [[Estremo superiore e inferiore]], adesso dobbiamo usare il [[Successioni e limiti infiniti|limite]].
(La successione non è più monotona).
La successione delle somme parziali si indica come sempre.
$$s_{n}:= \sum_{k=1}^{n}a_{k}\ \ \ \ \forall n \in \mathbb{N}$$
Ci possono essere 4 casi:

[^1] la successione è convergente a un numero reale r.
[^2] la successione è divergente verso $+\infty$.
[^3] la successione è divergente verso $-\infty$.
[^4] la successione non ha limite.

### Caso [^1]
La serie converge ad un numero reale $r$
$$\sum_{n=1}^{+\infty}a_{n}= r = \lim_{n\to + \infty} s_n$$
### Caso [^2] 
$$\sum_{n=1}^{+\infty}a_{n}= + \infty$$
### Caso [^3]
$$\sum_{n=1}^{+\infty}a_{n}= - \infty$$
### Caso [^4]
La serie è detta indeterminata, non esiste valore che possiamo associare ad essa.


# Consistenza con il caso delle serie a termini con segno costante
Se tutti gli $a_n$ hanno lo stesso segno, cadiamo in [[Serie numeriche a termini di segno costante]]. Copriamo [^1],[^2],[^3].

# Serie geometrica di ragione reale
[[Serie geometrica di ragione reale]]

# Omogeneità
Con $p \not= 0$
$$\sum_{n=1}^{+\infty}pa_{n}= p \sum_{n=1}^{+\infty}a_{n}$$
# Linearità
Date le due serie **NON INDETERMINATE**
$$\sum_{n=1}^{+\infty}a_{n},\qquad \sum_{n=1}^{+\infty}b_{n}$$
Si ha che
$$\sum_{n=1}^{+\infty}a_{n} + \sum_{n=1}^{+\infty}b_{n} = \sum_{n=1}^{+\infty}(a_{n} + b_n)$$
# Carattere definitivo
Stesso principio di [[Serie numeriche a termini di segno costante#Carattere definitivo]]

# Proposizione 10.0.7
Sia $\sum_{n=1}^{+\infty}a_{n}$ una serie convergente. Allora
$$\lim_{n\to+\infty}a_{n}= 0$$
#dimostrazione 
Per definizione esiste finito il limite s della successione ($s_n$) delle somme parziali della serie. Osserviamo che
$$a_{n}= s_{n}-s_{n-1}$$
Passando al limite si ottiene
$$\lim_{n\to +\infty}a_{n}=\lim_{n\to +\infty}(s_{n}- s_{n-1}) = \lim_{n\to +\infty}(s_{n}) - \lim_{n\to +\infty}s_{n-1} = s-s = 0$$

# La coda di una serie convergente è infinitesima
Sia $\sum_{n=1}^{+\infty} a_n$ una serie convergente. Allora
$$\lim_{N\to+\infty} \sum_{n=N+1}^{+\infty}a_{n}= 0$$
#dimostrazione-da-fare 



