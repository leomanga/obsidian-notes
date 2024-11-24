
>[!def] Successione di funzioni
>%%display: Successione di funzioni%%
>Una successione di funzioni è una famiglia di funzioni$$f_n:E\to\mathbb{R}^{k},k\in\mathbb{N},E\subseteq \mathbb{R}$$

^64f0c7

>[!def] Convergenza puntuale successione di funzioni
>Sia $(f_{n})_{n \in\mathbb{N}}$ una [[#^64f0c7]].
>Diciamo che $f_{n}$ converge puntualmente ad una funzione $f:E\to \mathbb{R}^{k}$ se $$\forall x\in E,\mbox{ la successione numerica } f_{n}(x)\in\mathbb{R}^{k}\mbox{ converge a } f(x)\in\mathbb{R}^{k}$$
>$$\forall x\in E, \forall \epsilon>0, \exists n_\epsilon\in\mathbb{N}:||f_{n}(x)-f(x)||\le\epsilon,\ \forall n\ge n_{\epsilon}$$
>---
>Guarda esempio su appunti pg 84

^5a5aaf

>[!def] Convergenza uniforme successione di funzioni
>Diremo che $f_{n}$ converge a $f$ uniformemente se 
>$$ \forall \epsilon>0, \exists n_\epsilon\in\mathbb{N}:||f_{n}(x)-f(x)||\le\epsilon,\ \forall n\ge n_{\epsilon},\ \forall x\in E$$
>---
>Guarda esempio su appunti pg 86

^5ebe85

![[Norma infinito]]

>[!thm] Funzione uniformemente convergente implica puntualmente convergente
>Siano $f_{n}:E\to\mathbb{R}^{k}$ funzioni assegnate e sia $f:E\to\mathbb{R}^{k}$
>$$f_{n}\to f\mbox{ uniformemente }\Rightarrow f_{n}\to f \mbox{ puntualmente}$$

>[!thm] Se la norma infinito = 0, allora $f_n$ converge uniformemente
>Siano $f_{n}:E\to\mathbb{R}^{k}$ funzioni assegnate e sia $f:E\to\mathbb{R}^{k}$
>$$||f_{n}-f||_{\infty}=0\iff f_{n}\to f\mbox{ uniformemente}$$
>---
>Dimostrazione a pg 87

>[!def]
>Sia $V =\{f:E\to\mathbb{R}^{k}:f\mbox{ limitata}\}$
>Allora $V$ è uno [[Spazio vettoriale|spazio vettoriale]].

>[!thm] Se $f_{n}$ converge uniformemente, allora $f$ è continua
>Siano $f_{n}:E\to\mathbb{R}$ [[Continuità funzioni - spazi metrici#Definizione Continua in un insieme|funzioni continue]] su $E$ tali che $f_{n}\to f:E\to\mathbb{R}\mbox{ uniformemente}$. Allora $f$ è continua.
>---
> Dimostrazione pg 90

>[!thm] Funzione [[Insieme misurabile secondo Peano Jordan]] e uniformemente convergente. Allora $f$ è integrabile
>Se $f_{n}:E\to\mathbb{R}$, con $E\subseteq R$ [[Rettangolo]] ed $E$ [[Insieme misurabile secondo Peano Jordan]].
>Supponiamo $f_{n}$ integrabile su $E$ e $f_{n}\to f$ uniformemente. Allora $f$ è integrabile su $E$.
>Inoltre $$\int_{E}f_{n}dx\to\int_{E}f dx$$
>---
>Dimostrazione pg 91

>[!lemma] 
>Sia $E\subseteq R$ un insieme [[Insieme misurabile secondo Peano Jordan]], allora $f:E\to \mathbb{R}$ è integrabile $\iff \forall \epsilon>0\ \exists g,h:E\to\mathbb{R}\mbox{ integrabili}$ tali che $\int h -\int g \le \epsilon$ e $g(x)\le f(x)\le h(x)\ \forall x\in E$
>
>---
>Dimostrazione pag 91

>[!prp]
>Siano $f_{n}:E\to \mathbb{R}$ funzioni [[Limiti finiti di una funzione in un punto#Definizione 12.0.15 Funzione limitata|limitate]] e $f_{n}\to f:E\to \mathbb{R}$ uniformemente.
>Allora anche $f$ è limitata e $||f_{n}||_{\infty}<+\infty$.
>Vale anche il viceversa.
>
>---
>Dimostrazione pag 94

![[Classi di funzioni#^1b877f]]

![[Classi di funzioni#^beec38]]

>[!thm] Lo spazio $C_{b}(E)$ è completo
>Lo [[Spazio vettoriale]] [[Norma|normato]] $(C_{b}(E),||\cdot||_{\infty})$ (vedi [[Classi di funzioni#^283b88]]) è uno [[Spazio metrico completo]]
>---
>Dimostrazione a pag 97

>[!thm] Lo spazio $C^{1}$ è completo
>Lo [Spazio vettoriale](app://obsidian.md/Spazio%20vettoriale) [normato](app://obsidian.md/Norma)  $(C^{1}(E),||\cdot||_{C^{1}})$ (vedi [Classi di funzioni > ^283b88](app://obsidian.md/Classi%20di%20funzioni#^283b88) è uno [Spazio metrico completo](app://obsidian.md/Spazio%20metrico%20completo)
>---
>Dimostrazione pag 99

>[!thm] 
>Sia $[a,b]\subseteq \mathbb{R}$ e siano $f_{n}:[a,b]\to \mathbb{R}$ funzioni di [[Classi di funzioni#^beec38]] tali che $f_{n}\to f:[a,b]\to \mathbb{R}$ [[#^5ebe85|uniformemente]] e $f^{'}_{n}\to g:[a,b]\to \mathbb{R}$ [[#^5ebe85|uniformemente]].
>Allora si ha $g\in C^{1}([a,b])$ e $f^{'}=g$.
>---
>Dimostrazione pag 98















