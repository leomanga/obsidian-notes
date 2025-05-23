>[!def] Insieme dei vincoli attivi
>Data una regione $X=\{x:h(x)=0, g(x)\ge 0\}$ e un punto $x\in X$, l’ **insieme dei vincoli attivi** in $x$ è costituito da tutti i vincoli soddisfatti in $x$ dall’uguaglianza, ossia
>$$I_{a}(x)=\{i=1,\ldots,m\}\cup\{j:m+1\le j\le m+p, g_{j}(x)=0\}$$

^5325c3

![[Matrice Jacobiana]]

^2dcc57

^7f57d1
>[!thm]
>Date due funzioni $f(x)$ e $h_{1}(x)$, se in un punto $x$ si ha che $\nabla f(x)$ e $\nabla{h_1}(x)$ non sono paralleli, allora esiste un vettore $\bar d$ che soddisfa 
>$$\nabla h_{1}(x)^{T}d = 0\mbox{ e}\ \nabla{f(x)}^{T}d < 0$$
>(Se entrambi non sono paralleli, $x$ non è un punto di minimo, anche se rispetta il vincolo)

![[Massimi e minimi di funzioni su curve o superfici#^ffc5a3]]

>[!prp] Caso di una disequazione
>Nel caso di una disequazione $g_{1}(\bar{x})\ge 0$, supponendo $\nabla g_{1}(\bar x)\not = 0$, per essere al minimo, vogliamo che per il punto $\bar x$, $\nabla f(\bar {x})^{T}d \ge 0$.(se non lo fosse avremmo una [[Direzione di discesa]] negativa).
>Se ci spostiamo leggermente da $\bar{x}$, dalla [[Formula di Taylor]] in più dimensioni avremo $0\le g_{1}(\bar {x} +d )\simeq g_{1}(\bar x)+\nabla g_{1}(\bar x)^{T}d$.
>Allora per essere ammissibile, $\bar x$ deve rispettare $$g_{1}(\bar x)+\nabla g_{1}(\bar x)^{T}d\ge 0$$
>- Caso 1: $\bar x$ interno a $X$ insieme dei vincoli
> Se $\bar x$ è interno a $X$, allora $g_{1}(\bar x)>0$, quindi il vincolo non è attivo in $\bar x$. Allora si verifica sempre l’equazione sopra per qualunque vettore $d$ piccolo in norma tale che $\bar x+d$ sia ancora nella regione ammissibile.
>  Allora in questo caso, non esisterà una direzione di discesa ammissibile per $\nabla f(\bar x)=0$
>  - Caso 2: $\bar x$ nella frontiera di $X$
>    In questo caso avremo un vincolo attivo $g_{1}(\bar x)=0$
>    Allora avremo che $\nabla g_{1}(\bar x)^{T}d\ge 0$.
>    
>    Per risolvere il nostro problema, possiamo qua fare uso dei [[Massimi e minimi di funzioni su curve o superfici#^ffc5a3|moltiplicatori di Lagrange]]. Per unificare i due casi vogliamo che $$\begin{split}&\nabla_{x}L(x^{*}.\lambda_{1}^{*}=0)\quad \mbox{per qualche}\ \lambda_{1}^{*}\ge 0\\&\lambda_{1}^{*}g_{1}(x^{*})=0\end{split}$$ In questo caso il segno del $\lambda$ fa la differenza.(guarda appunti prof per interpretazione geometrica)
>    

>[!def] Condizione di qualificazione dei vincoli attivi
>Data una regione ammissibile $X=\{x:h(x)=0, g(x)\ge 0\}$, un punto ammissibile $x$, e il corrispondente insieme di [[#^5325c3|vincoli attivi]] $I_{a}(x)$, si dice che i vincoli attivi soddisfano la condizione di qualificazione in $x$ se i loro gradienti, calcolati in $x$, sono [[Dipendenza lineare|linearmente indipendenti]].

^6a428a

>[!def ] Punto regolare
>Un punto $x$ per il quale vale la [[#^6a428a|condizione di qualificazione]] dei vincoli attivi prende il nome di punto regolare.
>Se un punto è regolare, nessuno dei gradienti dei vincoli attivi si può annullare.

^020857

Si possono riassumere tutte queste condizioni in [[Condizioni di Karush-Kuhn-Tucker]]
![[Condizioni di Karush-Kuhn-Tucker]]

>[!thm]
>Sia $x^{*}$ un minimo locale e valga la [[#^6a428a|condizione di qualificazione dei vincoli attivi]] in $x^{*}$. Allora, per ogni vettore $\lambda^{*}$ tale da soddisfare, con $x^{*}$, le [[Condizioni di Karush-Kuhn-Tucker]] si ha che
>$$s^{T}\nabla^{2}_{xx}L(x^{*},\lambda^{*})s\ge 0 \quad \forall s:J(x^*)s=0$$
>con $J(x^{*})$ si è indicata [[Ottimizzazione vincolata#^7f57d1|matrice jacobiana]] dei [[#^5325c3|vincoli attivi]] in $x^{*}$, calcolata in $x^*$.
>
>(L’Hessiana del lagrangiano deve essere [[Matrice definita positiva|semidefinita positiva]] sullo spazio nullo della matrice jacobiana dei vincoli attivi in $x^{*}$)

Scrivere sensibilità alle variazioni dei parametri

>[!thm]
> Dato un problema di ottimizzazione vincolata, se le funzioni $h_{i}(x)=a_{i}^{T}+b_{i}$ sono lineari e tutte le $-g_{j}$ sono convesse, allora la regione ammissibile $X$ è convessa.

^a41736

