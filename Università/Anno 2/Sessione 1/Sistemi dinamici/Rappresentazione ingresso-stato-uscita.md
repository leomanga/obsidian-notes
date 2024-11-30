---
aliases:
  - ISO
collegamenti:
---
Rappresenta una o più equazioni differenziali che mettono in relazione le [[variabili di ingresso]], le [[variabili di stato]] le [[variabili di uscita]].

$$\begin{cases}
 \dot{x}(t)=f(x(t),u(t),t)\\
 y(t)=g(x(t),u(t),t)
\end{cases}\qquad
\begin{split}
&f:\mathbb{R}^{n}\times\mathbb{R}^{m}\times\mathbb{R}\to \mathbb{R}^{n}\\
&g:\mathbb{R}^{n}\times \mathbb{R}^{m}\times \mathbb{R}\to \mathbb{R}^{p}
\end{split}
$$
>[!N.B.]
>$n$ numero di stati, $m$ numero di ingressi, $p$ numero di uscite.
>$u$ sono le [[variabili di ingresso]]
$x$ sono le [[variabili di stato]]
$y$ sono le [[variabili di uscita]]

>[!prp] Rappresentazione nei sistemi [[Sistemi lineari tempoinvarianti|LTI]]
>$$\begin{cases}\dot{x}(t)=A\cdot x(t)+B\cdot u(t)\\
>y(t)=C\cdot x(t)+D\cdot u(t)
>\end{cases}\qquad
>\begin{split}
>A:\mathbb{R}^{n\times n}\quad B:\mathbb{R}^{n\times m}\\
>C:\mathbb{R}^{p\times n}\quad D: \mathbb{R}^{p\times m}
>\end{split}
>$$

>[!prp] Trasformata di Laplace
>$$X(s)=\underbrace{(sI-A)^{-1}x(0)}_{X_{l},\ risposta\ libera\ nello\ stato}+\underbrace{(sI-A)^{-1}BU(S)}_{Y_{f},\ risposta\ forzata\ nello\ stato}$$
>$$Y(s)=CX(s)+DU(s)=\underbrace{C(sI-A)^{-1}x(0)}_{Y_{l},\ risposta\ libera}+\underbrace{[C(sI-A)^{-1}B+D]U(s)}_{Y_{f},\ risposta\ forzata}$$
>- $X_{l}$ e $Y_{l}$ sono le **risposte libere** nello stato e nell’uscita, le quali sono influenzate solo dai dati iniziali.
>- $X_{f}$ e $Y_{f}$ sono le **[[Risposta forzata|risposte forzate]]** nello stato e nell’uscita.
>  $Y_{f}=G(s)\cdot U(s)$, dove $U(s)$ è la trasformata della funzione di ingresso, mentre $G(s)=C(sI-A)^{-1}B+D$ viene chiamata **funzione di trasferimento del sistema**. 
>  Grazie a $G(s)$ si passa facilmente alla rappresentazione [[Rappresentazione ingresso-uscita|IO]]].
>