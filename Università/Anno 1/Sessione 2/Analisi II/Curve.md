>[!def] Curva in $\mathbb{R}^{n}$
>Una curva in $\mathbb{R}^{n}$ è una funzione $\gamma:[a,b]\to \mathbb{R}^{n}$ di classe 
>[[Classi di funzioni#^08c68a|$C^{1}$]]$([a,b])$.


>[!def] Curva regolare
>Diremo che $\gamma:[a,b]\to \mathbb{R}^{n}$ è regolare se $\gamma \in$ [[Classi di funzioni#^08c68a|$C^{1}$]]$([a,b])$ e $\gamma^{'}(t)\not = 0\ \forall t\in[a,b]$.

^85a74f

>[!def] Curva regolare a tratti
>Diremo che $\gamma:[a,b]\to \mathbb{R}^{n}$ è una curva regolare a tratti se $$\exists  a = t_{0}< t_{1}< t_{2}< \ldots < t_{k}= b$$ tali che $\gamma$ è [[#^85a74f|regolare]] su $[t_{i}, t_{i+1}]\ \forall i = 0, \ldots, k-1$ e $\gamma$ è continua su $[a,b]$.

>[!def] Sostegno
>$\gamma([a,b])$ prende il nome di sostegno di $\gamma$

^1549a8

>[!Prp] Vettore tangente a $\gamma$
>Se $\gamma$ è [[#^85a74f|regolare]], $\gamma^{'}(t)$ rappresenta il vettore tangente a $\gamma$ nel punto $\gamma(t)$.
>Posso in particolare definire $$r(s)=\gamma(t)+s\gamma^{'}(t),\quad s\in \mathbb{R}$$
>risulterà che $r(s)$ è una retta in forma [[Rappresentazione cartesiana e parametrica spazi affini#Rappresentazione parametrica|parametrica]], ed è tangente al [[#^1549a8|sostegno]] di $\gamma$ nel punto $\gamma(t)$.
>Inoltre $$r^{'}(s)=\frac{d}{ds}(\gamma(t)+s\gamma^{'}(t))=\gamma ^{'}(t)$$

^ba243d

>[!axiom]
>Notare che una curva definita come $$\gamma(t)=(t,f(t))$$
>dove $f:[a,b]\to \mathbb{R}$ una funzione di [[Classi di funzioni#^08c68a]]$([a,b])$, allora $\gamma$ è [[#^85a74f|regolare]], dato che $\gamma^{'}\not =0\ \forall t\in[a,b]$.
>

>[!lemma]
>Sia $\gamma:[a,b]\to \mathbb{R}^{2}$ una curva regolare.
>Allora $\forall t \in (a,b)\ \exists$ un intorno $I$ di $t$, $I\subseteq (a,b)$ tale che il sostegno di $\gamma$ sull'intervallo $I$ coincide con il grafico di una funzione $f$ della variabile $x$ oppure con il grafico di una funzione $g$ di $y$.
>---
>Dimostrazione a pag 7 argomento 5a

>[!lemma]
>Per quanto osservato prima, se $\gamma = (x,f(x))$, allora $\gamma^{'}(x)$ coincide col vettore tangente a $\gamma$ nel punto $r(x)$.
>Se $\gamma$ è [[#^85a74f|regolare]], allora $\forall t\in (a,b)\ \exists I$ intorno di $t$ tale che $\gamma:I\to \mathbb{R}^{2}$ è della forma $(x,f(x))$ oppure $(g(y),y)$
>$$\Rightarrow \gamma^{'}(t)\mbox{ coincide con la  tangente a }\gamma \mbox{ nel punto }\gamma(t)$$

>[!def] Curve equivalenti
>Siano $\gamma:[a,b]\to \mathbb{R}^{n}$ e $\sigma:[a,d]\to \mathbb{R}^{n}$ due curve.
>Diremo che $\gamma$ e $\sigma$ siano equivalenti se
>$$\begin{split}&\exists\ p:[a,b]\to [c,d]\mbox{ di classe }C^{1}([a,b]) \mbox{ e bigettiva}\\
>&\mbox{tale che }p^{'}(t)\not = 0\ \forall t\in(a,b)\ e\ \gamma(t)=\sigma(p(t))\ \forall t\in [a,b]\end{split}$$
>La $p:[a,b]\to[c,d]$ può essere vista come un cambio di variabile (oppure come riparametrizzazione di $\gamma$).

^971be9

>[!rmk]
>$\gamma:[a,b]\to \mathbb{R}^{n}$ è una curva parametrica perché dipende dal parametro $t$.
>Esempio
>$$\{x^{2}+y^{2}=1\}=\mbox{circonferenza di raggio 1 centrato nell'origine}$$
>$\gamma:[0,2\pi]\to \mathbb{R}^{2}, \gamma(t)=(\cos t, \sin t)$
>$\gamma$ è una curva parametrica il cui sostegno $\{x^{2}+y^{2}=1\}$

>[!def] Versore tangente a $\gamma$ nel punto $\gamma(t)$
>Sia $\gamma:[a,b]\to \mathbb{R}^{n}$ una curva [[#^85a74f|regolare]], allora definisco
>$$\tau_{\gamma}(t)=\frac{\gamma^{'}(t)}{||\gamma^{'}(t)||}\ \forall t\in(a,b)$$

^25200e

>[!lemma]
>$\tau$ è il versore [[#^25200e|tangente]] a $\gamma$ nel punto $\gamma(t)$.
>Se $\gamma$ è [[#^85a74f|regolare]] ed è [[#^971be9|equivalente]] a $\sigma$ allora
>$(i)$ Se $p:[a,b]\to[c,d]$ è crescente $\Rightarrow \tau_{\gamma}(t)=\tau_{\sigma}(p(t))$ $\forall t\in(a,b)$
>$(ii)$ Se $p:[a,b]\to[c,d]$ è decrescente $\Rightarrow \tau_{\gamma}(t)=-\tau_{\sigma}(p(t))$ $\forall t\in(a,b)$
>---
>Dimostrazione a pag 10 argomento 5a

>[!def] Lunghezza di una curva
>Sia $\gamma:[a,b]\to \mathbb{R}^{n}$ una curva [[#^85a74f|regolare]].
>Allora la lunghezza di $\gamma$ è il valore
>$$L(\gamma)=\int_{a}^{b}||\gamma^{'}(t)||dt$$

>[!prp]
>Sia $\gamma:[a,b]\to \mathbb{R}^{n}$ una curva [[#^85a74f|regolare]], allora
>$$L(\gamma) =\int_{a}^{b}||\gamma^{'}(t)||dt\ge||\gamma(b)-\gamma(a)||$$
>$\gamma(b)$ è il punto finale della curva
>$\gamma(a)$ è il punto iniziale della curva
>---
>Dimostrazione pag 12 argomento 5a

>[!rmk] 
>Se $\gamma(b)-\gamma(a)=\int_{a}^{b}\gamma^{'}(t)dt$, la proposizione precedente è equivalente a $$||\int_{a}^{b}\gamma^{'}(t)dt||\le \int_{a}^{b}||\gamma^{'}(t)||$$

>[!lemma]
	>Sia $\gamma:[a,b]\to \mathbb{R}^{n}$ e $\sigma:[c,d]\to \mathbb{R}^{n}$ con $\gamma$ e $\sigma$ [[#^971be9|equivalenti]]
>$$\Rightarrow L(\gamma)=L(\sigma)$$
>---
>Dimostrazione a pag 14 argomento 5a

>[!def] Spezzata
>Sia $\gamma:[a,b]\to \mathbb{R}^{n}$ una curva [[#^85a74f|regolare]].
>Sia $t_{0}=a<t_{1}<t_{2}<\ldots < t_{k}=b$ una partizione di $[a,b]$.
>Definiamo la spezzata $\sigma$ di vertici $\gamma(t_{i})$ la curva definita come$$\sigma(t)=\gamma(t_{i})+\frac{(t-t_{i})}{t_{i+1}-t_{i}}(\gamma(t_{i+1})-\gamma(t_i))$$
>se $t\in [t_{i},t_{i+1}]\ \forall i=0,\ldots,{k-1}$.
>Quella appena scritta è una parametrizzazione del segmento $\overline{\gamma_{t_{i}}\gamma(t_{i+1})}$ $\iff$ è una curva che dipende dal parametro $t\in[t_{i},t_{i+1}]$ e ha come [[#^1549a8|sostegno]] $\overline{\gamma(t_{i})\gamma(t_{i+1})}$.

>[!thm]
>Sia $\gamma:[a,b]\to \mathbb{R}^{n}$ una curva [[#^85a74f|regolare]] se $\sigma$ è una qualsiasi spezzata di estremi $\gamma(t_{0}), \gamma (t_{1}), \ldots, \gamma(t_{k})$, allora $L(\gamma)\ge L(\sigma)$.
>Inoltre $L(\gamma)=\sup_{\sigma\in \sum} L (\sigma)$ dove $$\sum=\{\mbox{tutte le possibili spezzate costruite su } \gamma\}$$
>$\iff$ l'estremo superiore è fatto su tutte le spezzate $\sigma$ che posso costruire a partire da $\gamma$. $\sigma$ dipende dalla partizione $a=t_{0}<t_{1}<\ldots<t_{k}=b$
>$\iff$ data una partizione $t_{0}<t_{1}<\ldots<t_{k}$ ho automaticamente una spezzata, quindi$$\sup_{\sigma\in\sum}L(\sigma)=\sup\{L(\sigma):t_{0}<t_{1}<\ldots<t_{k}\mbox{ è una partizione di }[a,b]\}$$
>$$L(\sigma)=\sum_{i=0}^{k-1}\int_{t_{i}}^{t_{i+1}}||\sigma^{'}(t)||dt$$
>>[!rmk]
>>La lunghezza di una curva regolare a tratti è la somma delle lunghezze delle curve sui vari tratti.
>---
>Dimostrazione a pag 18 argomento 5a, usa il teorema qua sotto

>[!lemma]
>Sia $v:[\alpha,\beta]\to \mathbb{R}^{n}$ continua.
>Sia $\tau\in (\alpha,\beta)$ fissato.
>Allora$$||\int_{\alpha}^{\beta}v(t)dt||\ge\int_{\alpha}^{\beta}||v(t)dt||-2\int_{\alpha}^{\beta}||v(t)-v(\tau)||dt$$
>---
>Questa la diamo per buona






 







