---
pagina: 230
aliases:
  - funzione lineare
  - trasformazione lineare
  - Funzione lineare
---
# Definizione
Siano $V$ e $W$ [[Spazio vettoriale]] su $\mathbb{K}$.
Sia $\varphi:V\to W$ una funzione tale che 
1) $\varphi(x+y)=\varphi(x)+\varphi(y)\qquad \forall x,y\in V$
2) $\varphi(\lambda x)=\lambda \varphi(x)\quad \forall x \in V,\forall \lambda \in \mathbb{K}$
Allora $\varphi$ è una trasformazione lineare.
- Possiamo scrivere equivalentemente
$$\varphi(\lambda x+\mu y)=\lambda\varphi(x)+\mu\varphi(y)\quad\forall x,y\in V, \forall \lambda,\mu\in \mathbb{K}$$
# Conseguenze
1) $\varphi(0_{V})= 0_W$
2) $\varphi(\sum_{i=1}^na_ix_i)=\sum_{i=1}^na_i\varphi(x_i)$
3) Se $V=W$ allora $\varphi(0)=0$
# Endomorfismo
Se $\varphi:V\to W$ è lineare e $V=W$ si dice ENDOMORFISMO.

# Esempi di trasformazioni lineari
1) Gli [[Isomorfismo|isomorfismi]] e gli automorfismi(che sono invertibili)
2) La [[Rotazione]] attorno all'origine.
3) Se $V=A\oplus B$, la [[Proiezione di A lungo B]] 
4) Il [[Simmetrico di un punto#Definizione 2 Simmetrico di un punto rispetto ad un iperpiano|simmetrico rispetto ad un iperpiano]]
5) L'[[Omotetia di ragione a]].
# Proposizione 1
Sia $\varphi:V\to W$ una funzione lineare.
Sia $\mathbb{X}\subseteq V$
Allora $\varphi(L(\mathbb{X}))=L(\varphi(\mathbb{X}))$
#dimostrazione-da-fare 
- Se $A$ è [[Sottospazio lineare|sottospazio lineare]] di $V$, allora $\varphi(A)$ è un sottospazio lineare di $W$.
- $\varphi(V)=Im(\varphi)$ è un sottospazio lineare di $W$.

# Definizione | Rango
Il rango di $\varphi$, funzione lineare, è definito come la [[Dimensione|dimensione]] dell'immagine di $\varphi$
$$rank(\varphi)= dim(Im(\varphi))$$
- $rank(\varphi)\le dim(codom(\varphi))$

# Proposizione 2
$\varphi:V\to W$ funzione lineare.
Se $S = P+S_{0}$ [[Sottospazio affine|sottospazio affine]] di $V$.
- Se $S$ è spazio affine di $V$, allora $\varphi(S)$ è un sottospazio affine di $W$.

# Teorema di esistenza e unicità
Siano $V$ e $W$ [[Spazio vettoriale|spazio vettoriale|spazi vettoriali]] su $\mathbb{K}$.
Sia $E=(E_1,E_2,\ldots,E_n)$ [[Base]] di $V$. ([[Dimensione|dim]]$(V)=n$).
Sia $B=(B_1,B_2,\ldots,B_n)$ insieme ordinato di vettori di $W$ tale che abbia stessa [[Cardinalità]] di $E$.
- Allora $\exists !$ funzione lineare $\varphi:V\to W$ tale che $\varphi(E_i)=B_{i}\quad\forall i = 1,\ldots,n$

# Proposizione 3
Se $\varphi:V\to W$ funzione lineare
Allora $rank(\varphi)\le dim(V)$ e $rank(\varphi)\le dim(W)$
Allora $rank(\varphi \le min\{dim(V),dim(W)\}.)$

# Proposizione 4 | matrice rappresentativa di $\varphi$ rispetto alle basi E ed F
Sia $\varphi:V_{n}\to W_m$ una funzione lineare
$V_n,W_m$ [[Spazio vettoriale|spazio vettoriali]] su $\mathbb{K}$.
$E = (E_1,E_2,\ldots,E_n)$
$F=(F_1,F_2,\ldots,F_m)$
Allora $\varphi(E_i)=\sum_{J=1}^{m}a_{ji}F_j$
$$\left(\begin{split}
&a_{11}\quad a_{12}\quad\ldots\quad a_1n\\
&a_{21}\quad a_{22}\quad\ldots\quad a_2n\\
&\ldots\\
&a_{m1}\quad a_{m2}\quad\ldots\quad a_mn
\end{split}\right)=\mu_{E,F}(\varphi)
$$
è la matrice rappresentativa di $\varphi$ rispetto alle basi E ed F.
- Il numero di righe è uguale alla [[Dimensione|dimensione]] del codominio di $V_n$, cioè la [[Dimensione|dimensione]] di $W_m$.

Guarda appunti per altro

# Proprietà | Suriettività
$\varphi:V\to W$ funzione lineare, $dim(V)<\infty, dim(W)<\infty$
1) $\varphi$ suriettiva $\iff Im(\varphi) = W\iff rank(\varphi)=dim(W)$
2) $\varphi$ suriettiva $\Rightarrow dim(V)\ge dim(W)$
- Se $dim(V) < dim(W)$ allora non è suriettiva.

# Proprietà | Iniettività
$\varphi:V\to W$ funzione lineare
$\varphi$ iniettiva $\iff rank(\varphi)=dim(V)$
$\varphi$ iniettiva $\Rightarrow dim(V)\le dim(W)$
- Se $dim(V)>dim(W)$ allora non è iniettiva.

# Proprietà | Invertibilità
$dim(V)=dim(W)<\infty$
$\varphi$ è surriettiva $\iff \varphi$ iniettiva $\Rightarrow$ $\varphi$ è invertibile
(Basta che $\varphi$ sia suriettiva o iniettiva per verificare l'invertibilità)