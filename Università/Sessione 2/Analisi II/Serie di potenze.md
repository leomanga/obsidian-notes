---
collegamenti:
  - "[[Serie di funzioni]]"
---
Una serie di potenze è una particolare [[Serie di funzioni]]
$$\sum_{n=0}^{+\infty}a_{n}(y-y_{0})^{n}$$dove $y_{0}\in \mathbb{R}$ fissato e quindi $f_{n}(y)=a_{n}(y-y_{0})^{n}$.
$y_{0}$ prende il nome di ==centro della serie di potenze==.
Con il cambio di variabile $x=y-y_{0}\Rightarrow\sum_{n=0}^{+\infty}a_{n}x^{n}$ e $f_{n}(x)=a_{n}x^{n}$.
$a_{n}\in \mathbb{R}$ è una successione qualsiasi.

>[!remark] 
>Una serie di potenze $\sum_{n=0}^{+\infty}a_{n}x^{n}$ converge sempre per $x=0$, ma può anche non convergere per nessun altro valore di $x\in \mathbb{R}$.

>[!thm] 
>Supponiamo $\sum_{n=0}^{+\infty}a_{n}x^{n}$ converga per $x=y$. 
>Allora $\sum_{n=0}^{+\infty}a_{n}x^{n}$ converge $\forall x\in(-|y|,|y|)$.
>
>---
>Dimostrazione argomento 4b pg 7.

>[!rmk]
>Se $\sum_{n=0}^{+\infty}a_{n}y^{n}$ non converge $\forall x:|x| > |y|\Rightarrow\sum_{n=0}^{+\infty}a_{n}x^{n}$ non converge.

>[!def] Raggio di convergenza
>Definiamo il raggio di convergenza di una serie di potenze come
>$$R:=\sup\{ |x|:x\in \mathbb{R},\sum_{n=0}^{+\infty}a_{n}x^{n}\mbox{ converge}\}$$
>Se ad esempio $\sum_{n=0}^{+\infty}<+\infty\ \forall x\in \mathbb{R}$, allora $R=+\infty$.
>

^81d774

>[!prp] 
>Se $\sum_{n=0}^{+\infty}a_{n}x^{n}$ ha [[#^81d774|raggio di convergenza]] $R>0\Rightarrow\sum_{n=0}^{+\infty}a_{n}x^{n}$ converge $\forall x:|x|<R$ e non converge $\forall x:|x| > R$.

>[!rmk]
>Se $R=|x|$ può accadere che la serie converga come che non converga. Dipende. Questo è dovuto dal fatto che $R$ è un estremo superiore e non un massimo.

>[!thm]
>Supponiamo che $\sum_{n=0}^{+\infty}a_{n}x^{n}$ abbia raggio di convergenza $R>0$.
>Allora la funzione $f(x)= \sum_{n=0}^{+\infty}a_{n}x^{n}$ è [[Derivate - spazi metrici|derivabile]] in $(-R,R)$ e la derivata coincide con la serie $f^{'}(x)=\sum_{n=0}^{+\infty}na_{n}x^{n-1}$.
>In particolare $f^{'}(x)$ ha lo stesso raggio di convergenza $R>0$.
>---
>Dimostrazione a pag 108

>[!corollary]
>Supponiamo $f(x)=\sum_{n=0}^{+\infty}a_{n}x^{n}$ abbia raggio di convergenza $R>0$.
>Per ogni $k>0$ si ha che $f$ è derivabile $k$-volte su $(-R,R)$ e tale derivata coincide con la serie delle derivate $$\sum_{n=0}^{+\infty}\left(\frac{d^{k}}{dx^{k}}\right)a_{n}x^{n}=\sum_{n=k}^{+\infty}\frac{n!}{(n-k)!}a_{n}x^{n-k}$$

>[!corollary]
>Si ha $f(x)=a_{n}x^{n}$, con raggio di convergenza $R>0$.
>Allora $f(x)$ è di [[Classi di funzioni#^7dda87|classe $C^{\infty}$]].

>[!thm] Teorema della radice totale
>Sia $\sum_{n=0}^{+\infty}a_{n}x^{n}$ una serie di potenze per la quale esiste il limite $$\lim_{n\to+\infty}\sqrt{|a_{n}|}=:L$$
>Allora:
>1) Se $L=+\infty$, la serie $\sum_{n=0}^{+\infty}a_{n}x^{n}$ converge solo per $x=0 (R=0)$
>2) Se $L=0$, la serie converge $\forall x\in \mathbb{R}(R=+\infty)$
>3) Se $L\in(0,+\infty)\Rightarrow R=\frac{1}{L}$
>---
>$R$ è il [[#^81d774]].
>Dimostrazione a pagina 110




