>[!prp] Trasformata Zeta
>Sia $f(k)$ un segnale a tempo discreto tale che $f(k)=0\quad \forall k <0$ e $\exists M>0,\rho_{0}\in \mathbb{R}, \rho_{0}>0$ e $k_{0}\in \mathbb{N}$ tali che 
>$$|f(k)|<M\rho_{0}^{k}\quad \forall k\ge k_{0}$$
>Si definisce allora la trasformata Zeta di $f(k)$ la funzione $F(z):\mathbb{C}\to \mathbb{C}$
>$$F(z)=\sum_{k=0}^{+\infty}f(k)z^{-k}=\mathcal{Z}[F(z)]$$

Le ipotesi sono necessarie per far convergere la [[Serie numeriche|serie]].
# Proprietà
1) Linearità
2) Trasformata dei segnali con ritardo $\frac{1}{z^{\Delta}}$
3) Moltiplicazione per esponenziale $\frac{z}{z-\rho}$
4) Moltiplicazione per $k$, $-z\frac{d}{dz}F(z)$→ si può vedere come un anticipazione teoricamente

---

>[!thm] Teorema del valore finale
>$$\lim_{k\to \infty}f(k)\mbox{ esiste finito} \Rightarrow\lim_{k\to \infty}f(k)=\lim_{z\to1}(z-1)F(z)$$
>(Esiste finito se $F(z)$ ha poli interni al cerchio unitario tranne al più un polo in $z=1$)


