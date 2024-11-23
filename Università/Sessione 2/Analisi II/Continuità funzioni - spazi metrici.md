# Definizione | Continua in un punto
Sia $(X,d)$ uno  [[Spazi metrici|spazio metrico]] e sia $f:X\to \mathbb{R}$.
($X$ può avere più dimensioni)
Allora $f$ si dice continua in $\bar x$ se vale:
$$\begin{split}\forall \epsilon>0\ \exists \delta_\epsilon>0:|f(\bar x)-f(y)|<\epsilon\ &\forall y:d(\bar x,y)<\delta_\epsilon\\
&\forall y\in B_{\delta}(x)\\
\end{split}$$
$$\begin{split}\iff \forall \mbox{ successione } (x^{m}\subseteq\mathbb{R}^{n}:x^{m}\to x\\\mbox{ per } m\to+\infty\mbox{ si ha }f(x^{m})\to f(x)\end{split}$$
---
Nel caso generale in cui $f:X\subseteq{\mathbb{R}^n}\to\mathbb{R}^{k}$
possiamo dire che $f$ è continua se e solo se
$$\begin{split}\forall \epsilon>0\ \exists \delta_\epsilon>0:||f(\bar x)-f(y)||<\epsilon\ &\forall y:d(\bar x,y)<\delta_\epsilon\\
&\forall y\in B_{\delta}(x)\\
\end{split}$$
$$\begin{split}\iff \forall \mbox{ successione } (x^{m}\subseteq\mathbb{R}^{n}:x^{m}\to x\\\mbox{ per } m\to+\infty\mbox{ si ha }f(x^{m})\to f(x)\end{split}$$
# Definizione | Continua in un insieme
Sia $(X,d)$ uno [[Spazi metrici|spazio metrico]] e sia $f:X\to \mathbb{R}$.
Sia $E\subseteq X$. 
Allora $f$ si dice continua in $E$ se $\forall x\in E$ $f$ è continua in $x$.
In questo caso $\delta$ dipende da $\epsilon$ e da $x$.
# Definizione | Uniformemente continua
$$\forall \epsilon > 0\ \exists \delta>0:|f(x)-f(y)|<\epsilon\ \forall y\in E: d(x,y)<\delta$$
# Esempio 1 | continuità funzione distanza
a pag 17
# Teorema
Sia $(X,d)$ uno [[Spazi metrici|spazio metrico]].
Allora $d:X\times X\to\mathbb{R}$ è continua su $X\times X\iff$ ogni volta che $x^{m}\to x$ e $y^{m}\to y$ si ha $d(x^{m},y^{m})\to d(x,y)$
#dimostrazione-da-fare 
# Funzione continua a tratti
![[Serie di fourier#^72d75b]]
