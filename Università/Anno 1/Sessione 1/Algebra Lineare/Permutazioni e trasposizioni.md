---
pagina: 278
---
# Definizione | Permutazione
La permutazione di $n$ elementi è una funzione invertibile $\sigma:\{1,\ldots,n\}\to \{1,\ldots,n\}$
$$\left(\begin{split}
&1\ 2\ 3\ \ldots\ n\\
&3\ 1\ 2\ \ldots\ n
\end{split}\right)\quad 
\begin{split}
&\sigma(1)=3\\
&\sigma(2)=1\\
&\sigma(3)=2\\
&\ldots
\end{split}$$

# Definizione | Trasposizione
Una trasposizione $\tau$, è una [[Permutazioni e trasposizioni#Definizione Permutazione|permutazione]] che scambia $i$ con $j$ e fissa tutti gli altri elementi
$$\tau_{1,4}=\left(\begin{split}
&1\ 2\ 3\ 4\\
&4\ 2\ 3\ 1
\end{split}\right)$$

# Definizione | Gruppo simmetrico
L'insieme di tutte le [[Permutazioni e trasposizioni#Definizione Permutazione|permutazioni]] di $n$ elementi forma un gruppo chiamato GRUPPO SIMMETRICO($Sym(n)$).
$$|Sym(n)|=n!$$
# Definizione | Ciclo di lunghezza m
Sia $\sigma$ una [[Permutazioni e trasposizioni#Definizione Permutazione|permutazione]] $\sigma \not = Id$
Se $\exists m\in \mathbb{N}\setminus \{0\}$ tale che $\sigma^{m}=Id$ e $\sigma^{m-1}\not = Id$, si indica con CICLO DI LUNGHEZZA (o ordine) $m$.

# Teorema 1
1) Ogni [[Permutazioni e trasposizioni#Definizione Permutazione|permutazione]] è prodotto(cioè composizione) di [[Permutazioni e trasposizioni#Definizione Ciclo di lunghezza m|cicli]] disgiunti.
2) Ogni ciclo di lunghezza $k$ è prodotto di $k-1$ trasposizioni.

# Corollario
Una permutazione è pari (e si indica con $+$) se è prodotto di un numero pari di trasposizioni
Una permutazione è dispari (e si indica con $-$) se è prodotto di un numero dispari di trasposizioni
# Definizione | segno di una permutazione
Sia $Sym(n)$ l'insieme di tutte le [[Permutazioni e trasposizioni#Definizione Permutazione|permutazioni]] di $n$ elementi
$$\forall \sigma\in Sym(n),\ \underbrace{Sgn}_{segno}(\sigma)=\begin{cases}
+\mbox{ se }\sigma\mbox{ è pari}\\
-\mbox{ se }\sigma\mbox{ è dispari}

\end{cases}$$