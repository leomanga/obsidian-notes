---
collegamenti:
  - "[[Campo dei numeri complessi]]"
---
>[!def] Trasformata di Laplace
>Sia $f(t):\mathbb{R}\to \mathbb{R}$ tale che $f(t)=0\ \forall t<0$ e
>$\exists M>0,\alpha \in \mathbb{R}, t_{0}\ge 0$ tali che 
>$$|f(t)|\le Me^{\alpha t}\quad \forall t\ge t_0$$
>Si definisce allora la trasformata di Laplace la funzione $F(s):\mathbb{C}\to \mathbb{C}$
>$$F(s)=\int_{0}^{\infty}f(t)e^{-st}dt=\mathcal{L}[f(t)]$$

Le ipotesi sono fondamentali perché potrebbe non convergere l’integrale.
Se le ipotesi sono valide, per $\sigma>\alpha$, l’integrale converge sempre, dove $\sigma$ è la parte reale di $s$.

# Proprietà
1) **Linearità**: Dato che l’integrale è un operatore lineare, allora, con $f,g:\mathbb{R}\to \mathbb{R}$ e $\alpha,\beta\in \mathbb{R}$
$$\mathcal{L}[\alpha f(t)+\beta g(t)]=\alpha\mathcal{L}[f(t)]+\beta \mathcal{L}[g(t)]=\alpha F(s)+ \beta G(s)$$
2) **Trasformata dei segnali con [[Operatore di ritardo|ritardo]]**: Con $\Delta >0$
$$g(t)=f(t-\Delta)\cdot \mathbb{1}(t)$$
$$\mathcal{L}[g(t)]=G(s)=F(s)\cdot e^{-\Delta s}$$ ^a6ef22
3) **Moltiplicazione per esponenziale**: (praticamente la cosa inversa della trasformata dei segnali con ritardo)
   $$g(t)=f(t)e^{\alpha t}\cdot \mathbb{1}(t)$$
$$   \mathcal{L}[g(t)]=F(s-\alpha)$$
4) **Moltiplicazione per $t$**:
   $$g(t)=t\cdot f(t)$$$$\mathcal{L}[g(t)]=-\frac{d}{ds}F(s)$$
5) **Trasformata della derivata**:
   $$g(t)=f^{'}(t)\cdot \mathbb{1}(t)$$$$\mathcal{L}[g(t)]=s\cdot F(s)-f(0)$$
6) **Trasformata dell’integrale**:
   $$g(t)=\int_{0}^{t}f(\tau)d\tau\cdot \mathbb{1}(t)$$
   $$\mathcal{L}[g(t)]=\frac{1}{s}F(s)$$
7) **Trasformata del [[Prodotto di convoluzione]]**:
   $$h(t) = f(t) * g(t)$$
   $$\mathcal{L}[h(t)]=F(s)\cdot G(s)$$

---
[[Funzioni proprie e strettamente proprie]]

>[!thm] Teorema del valore finale
>$$\lim_{t\to \infty}f(t)\mbox{ esiste finito}\Rightarrow\lim_{t\to\infty}f(t)=\lim_{s\to 0}sF(s)$$
>

^f408f6

# Trasformate non elementari
[[Segnale rettangolare]]
[[Sinusoide smorzata]]

# Elementi caratteristici della trasformata di un [[Sistemi lineari tempoinvarianti|LTI]]
Nella trasformata di un [[Sistemi lineari tempoinvarianti|LTI]], avremo sempre, nel caso [[Rappresentazione ingresso-uscita#^84e975|IO]]:
$$Y(s)=Y_{l}(s)+Y_{f}(s)$$
$Y_{f}(s)=G(s)\cdot U(t)$