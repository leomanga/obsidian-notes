>[!def] Distribuzione di probabilità
>Una distribuzione di probabilità è una funzione che prende in ingresso una variabile scalare($\mathbb{x}$) e si basa su una [[Variabili aleatorie|variabile aleatoria]]($x$).
>$$F_{x}(\mathbb{x}):= P\{s:x(s)\le \mathbb{x}\}=P\{x \le \mathbb{x} \}$$

>[!prp] Distribuzione di probabilità come integrale
> Dalla definizione della [[Densità di probabilità]] abbiamo allora che
> $$F_{x}(\mathbb{x})=\int_{-\infty}^{+\infty}f(x)dx$$

>[!example] Lancio del dado
>$S=\{1,2,3,4,5,6\}$
>$x=\begin{cases}1\mbox{ se } s=1\\2\mbox{ se } s=2\\3\mbox{ se } s=3\\4\mbox{ se } s=4\\5\mbox{ se } s=5\\6\mbox{ se } s=6\end{cases}$

```functionplot
---
title: Distribuzione di probabilità lancio del dado
xLabel: numero estratto
yLabel: probabilità
bounds: [-1,8,0,1.5]
disableZoom: false
grid: true
---
F(x) = x < 1 ? 0 :  (x<2 ? 1/6 : (x<3 ? 2/6 : ( x<4 ?3/6 : (x<5 ? 4/6 : ( x< 6 ? 5/6 : 1)))))
```
# Proprietà
1) $\lim_{\mathbb{x}\to \infty}F_{x}(\mathbb{x})=1$
   $\lim_{\mathbb{x}\to -\infty}F_{x}(\mathbb{x})=0$
2) Se $\mathbb{x}_{1}< \mathbb{x}_{2}\quad F_{x}(\mathbb{x}_{1})\le  F_{x}(\mathbb{x}_{2})$, quindi $F_{x}$ è [[Funzioni monotone#Funzione monotona|monotona crescente]]. ^8b45c0
3) $P\{x>\mathbb{x}\}=1-P\{x\le \mathbb{x}\}\}=1-F_{x}(\mathbb{x})$
4) $F_{x}(\mathbb{x}^{+})=F_{x}(\mathbb{x})$, quindi $F_{x}$ è [[Funzioni continue|continua]] a destra.
5) $P\{\mathbb{x}_{1}\le x\le \mathbb{x}_{2}\} = F_{x}(\mathbb{x}_{2})- F_{x}(\mathbb{x}_{1})$
6) $P\{x=\mathbb{x}\}=F_{x}(\mathbb{x}^{+})- F_{x}(\mathbb{x}^{-})$

>[!prp]
>Dalle proprietà possiamo dire che le zone a maggior pendenza sono le zone a maggior [[Probabilità|probabilità]].

