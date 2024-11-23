>[!def] Serie di funzioni
>Una serie di funzioni è una sommatoria $$\sum_{n=0}^{+\infty}f_{n}(x)$$
>dove $f_{n}:E\to \mathbb{R}$.
>Possiamo vedere la serie come limite delle somme parziali
>$$S_{n}(x)=\sum_{i=0}^{n}f_{i}(x)$$

>[!def] Convergenza puntuale serie di funzioni
>Diremo che $\sum_{n=0}^{+\infty}f_{n}(x)$ converge puntualmente ed $f:E\to \mathbb{R}$ se $S_{n}(x)\to f(x)$ [[Successioni di funzioni#^5a5aaf|puntualmente]] quando $n\to+\infty\ \forall x\in E$.
>

^6cf475

>[!def] Convergenza uniforme serie di funzioni
>Diremo che $\sum_{n=0}^{+\infty}f_{n}(x)$ converge uniformemente ad $f:E\to\mathbb{R}$ se $S_{n}\to f(x)$ [[Successioni di funzioni#^5ebe85|uniformemente]] quando $n\to+\infty\ \forall x\in E$.

^993d10

>[!def] Convergenza totale serie di funzioni
>Diremo che $\sum_{n=0}^{+\infty}f_{n}(x)$ converge totalmente ad $f$ se $\sum_{n=0}^{+\infty}||f_{n}||_{\infty}$ è convergente 
>($\iff \sum_{n=0}^{+\infty}||f_{n}||_{\infty}<+\infty$)

^98ab3e

^fd6458
> [!remark]
> Se $\sum_{n=0}^{+\infty}f_{n}(x)$ [[#^fd6458|converge totalmente]], allora $\sum_{n=0}^{+\infty}f_{n}(x)$ [[#^993d10|converge uniformemente]], e quindi [[#^6cf475|converge puntualmente]].
> Infatti se $\sum_{n=0}^{+\infty}||f_{n}||_{\infty} < +\infty\Rightarrow$ la successione di somme parziali $S_{n}(x)$ converge uniformemente ad $f(x)=\sum_{n=0}^{+\infty}f_{n}(x)$.
> ---
> Guarda dimostrazione in argomento 4b pag 2

>[!thm] Funzione che converge totalmente è integrabile
>Siano $f_{n}:E\to\mathbb{R}$ [[Integrabile secondo Rienmann - spazi metrici|Inegrabili]] e limitate, dove $E$ è un [[Insieme misurabile secondo Peano Jordan]]. Supponiamo che $\sum_{n=0}^{+\infty}f_{n}(x)$ [[#^98ab3e|converga totalmente]].
>Allora $f(x):=\sum_{n=0}^{+\infty}f_{n}(x)$ è integrabile su $E$ e $$\int_{E}f(x)dx=\sum_{n=0}^{+\infty}\int_{E}f_{n}(x)dx$$
>---
>dimostrazione in argomento 4b pag 4 

>[!thm] 
>Supponiamo $f_{n}:[a,b]\to\mathbb{R}, f_{n}\in C^{1}([a,b])$ ([[Classi di funzioni#^beec38]]) e supponiamo che $\sum_{n=0}^{+\infty}f_{n}(x)$ e $\sum_{n=0}^{+\infty}f^{'}_{n}(x)$ converge [[#^993d10|uniformemente]] ad $f$ e $g$ rispettivamente. 
>Allora $$f=\sum_{n=0}^{+\infty}f_{n}(x)\in C^{1}([a,b])$$ e $$f^{'}=g=\sum_{n=0}^{+\infty}f^{'}_{n}$$
>---
>dimostrazione in argomento 4b pag 5

![[Serie di potenze]]



