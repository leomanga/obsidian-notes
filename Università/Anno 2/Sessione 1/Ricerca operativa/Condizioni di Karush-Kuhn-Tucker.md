---
aliases:
  - KKT
---
Considerando un problema di [[Ottimizzazione vincolata]]:
$$\begin{split}\min f(x)\\x\in X\subset \mathbb{R}^{n}\end{split}$$
dove $X=\{x:h(x)=0, g(x)\ge 0\}$, in cui $h$ e $g$ sono vettori di funzioni di $x\in \mathbb{R}^{n}$.
In [[Ottimizzazione vincolata]] abbiamo visto che se $f$, $g$ e $h$ hanno derivate parziali continue in $x^{*}$, se $x^{*}$ è un punto di minimo locale ed è un punto [[Ottimizzazione vincolata#^020857|regolare]], esiste un vettore $\lambda^{*}$ tale che valgono le seguenti condizioni del primo ordine (Condizioni di Karush-Kuhn-Tucker):
$$\begin{split}
\nabla_{x}L(x^{*},\lambda^{*})&=0\\ h_{i}(x^{*})&=0\quad i=1,\ldots,m\\
g_{j}(x^{*})&\ge 0\quad j=m+1,\ldots,m+p\\ 
\lambda^{*}_{j}&\ge 0\quad j=m+1,\ldots,m+p\\
\lambda_{j}^{*}g_{j}(x^{*})&=0\quad j=m+1,\ldots,m+p
\end{split}$$
dove $L$ è la funzione lagrangiana definita per i casi di [[Programmazione non lineare]]:
$$L(x,\lambda)=f(x)-\sum_{i=1 }^{m}\lambda_{i}h_{i}(x)-\sum_{j=m+1}^{m+p}\lambda_{j}g_{j}(x)$$

Se un punto $\bar x$ non è [[Ottimizzazione vincolata#^020857|regolare]], allora non si riesce a verificare la lagrangiana $L(\bar x, \lambda)$, quindi non si può applicare ciò che abbiamo visto sopra.

Denotiamo con $\mathcal{K}$ l’insieme dei punti KKT, ovvero quei punti di minimi locale secondo le condizioni di Karush-Kuhn-Tucker.

>[!def] Complementarietà stretta
>Dato un problema [[PNL]], un punto di minimo locale $x^{*}$, e un vettore $\lambda^{*}$ che soddisfa le condizioni KKT, vale la condizione di complementarietà stretta se, per ciascuna disequazione attiva in $x^{*}$, si ha $\lambda_{j}^{*}>0$
>
>(Se per le $g$ vale per forza che $\lambda_{j}>0$, non per forza vale per le $f$)
>Se siamo in questa condizione, allora $\lambda^{*}$ è unico

