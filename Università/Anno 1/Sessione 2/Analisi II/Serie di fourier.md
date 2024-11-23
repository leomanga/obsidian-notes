---
collegamenti:
  - "[[Serie di funzioni]]"
---
>[!def] Serie di fourier
>Una serie di fourier è una [[Serie di funzioni]] della forma
>$$\frac{a_{0}}{2}+\sum_{k\ge 1}a_{k}\cos (kx)+b_{k}\sin(kx)$$
>Se $f$ è una funzione data $f:[-\pi,\pi]\to \mathbb{R}$
>Possiamo trovare i coefficienti $a_{0},a_{k},b_{k}, k\ge 1$ tali che $$f(x)=\frac{a_{0}}{2}+\sum_{k\ge 1}a_{k}\cos (kx)+b_{k}\sin(kx)$$

>[!def] Funzione continua a tratti
>%%display : funzione continua a tratti%%
>Dato un intervallo $[a,b]$, diremo che $f:[a,b]\to \mathbb{R}$ è continua a tratti se $\exists$ una partizione di $[a,b]$, $t_{0}=a<t_{1}<t_{2}<\ldots<t_{k}=b$ tali che $f$ è continua su $(t_{i-1},t_{i})\ \forall i =1,\ldots,n$.

^72d75b
>[!def] Funzione $C^{1}$ a tratti
>%%display:funzione $C^{1}$ a tratti%%
>Diremo che $f:[a,b]\to \mathbb{R}$ è $C^{1}$ a tratti se $\forall i=1,2,\ldots,n$, la funzione $f$ è di classe  [[Classi di funzioni#^08c68a|$C^1$]]$((t_{i-1},t_{i}))$ e inoltre esistono i limiti
>$$\lim_{x\to t_{i-1}}f(x)=f(t_{i-1}^{+})\in \mathbb{R},\ \ \lim_{x\to t_{i}}f(x)=f(t_{i}^{-})\in \mathbb{R}$$
>Devono esistere anche i limiti dei rapporti incrementali
>$$f^{'}(t_{i}^{-})=\lim_{h\to 0}\frac{f(t_{i}+h)-f(t_{i}^{-})}{h}\in \mathbb{R},\ \ f^{'}(t_{i-1}^{+})=\lim_{h\to 0^{+}}\frac{f(t_{i-1}+h)-f(t_{i-1}^{+})}{h}\in \mathbb{R}$$
>Infine $f^{'}:[t_{i-1},t_{i}]\to \mathbb{R}$ deve essere [[Continuità funzioni - spazi metrici|continua]].
^3892cb

>[!def] Funzione periodica
> $f:\mathbb{R}\to \mathbb{R}$ si dice periodica se $$\exists T>0: f(x)=f(x+T)\ \forall x\in \mathbb{R}$$ $T$ si chiama periodo.
> Se $f:\mathbb{R}\to \mathbb{R}$ è periodica di periodo $T>0$, posso definire $\widehat f:\mathbb{R}\to \mathbb{R}=f(\frac{xT}{2\pi})$ e $f$ risulterà periodica di periodo $2\pi$.
> Se $f:[-\pi,\pi]\to \mathbb{R}$, possiamo definire la sua estensione periodica di periodo $2\pi$ come $\bar f(x)=\widehat f(x-2k\pi)\mbox{ se } x\in[-\pi+2k\pi,\pi+2k\pi]\ \forall k\in \mathbb{Z}$.   

^88ecc8

> [!lemma]
>Le funzioni su $[-\pi,\pi]$ $$e_{0}=1,\ \ e_{k}=\cos(kx),\ \ e_{-k}=\sin(kx)$$
>con $k\ge 1$ soddisfano le seguenti proprietà
>$$\begin{split}&\int_{-\pi}^{\pi}e_{k}^{2}dx=\pi\mbox{ se } k\in \mathbb{Z}, k\not = 0\\
>&\int_{-\pi}^{\pi}e_{0}^{2}dx=2\pi\\
>&\int_{-\pi}^{\pi}e_{k}e_{j}dx=0\mbox{ se }k\not = j\\
>&\int_{-\pi}^{\pi}e_{k}dx=\begin{cases}2\pi\ k=0\\0 k\not = 0, k\in \mathbb{Z}\end{cases}
>\end{split}$$

^744fba

> [!proposition]
>Supponiamo $$f(x)=\frac{a_{0}}{2}+\sum_{k\ge 1}a_{k}\cos (kx)+b_{k}\sin(kx)$$
>Allora $$\begin{split}&\int_{-\pi}^{\pi}f(x)\cos(hx)dx=\\
>&=\int_{-\pi}^{\pi}\frac{a_{0}}{2}\cos(hx)+\sum_{k\ge 1}\left(\int_{-\pi}^{\pi}a_{k}\cos(kx)\cos(hx)+\int_{-\pi}^{+\pi}b_{k}\sin(kx)\cos(hx)\right)=\\
>&=\pi a_{h}\end{split}$$
>Si ottiene questo risultato da [[#^744fba]]
>In modo analogo avremo che 
>$$\int_{-\pi}^{\pi}f(x)\sin(hx)=\pi b_{h}$$

^6143e3

>[!prp] Coefficienti di fourier
>Da [[#^6143e3]], se la serie di Fourier converge ad $f(x)$, allora i coefficienti $a_{0},a_{k},b_{k}$ devono soddisfare
>$$\begin{split}& \frac{1}{\pi}\int_{-\pi}^{\pi}f(x)\cos(kx)=a_{k}\ \forall k\ge 1\\
>&\frac{1}{\pi}\int_{-\pi}^{\pi}f(x)\sin(kx)=b_{k}\ \forall k\ge 1\\
>& \frac{1}{\pi}\int_{-\pi}^{\pi}f(x)dx=a_{0}\end{split}$$

> [!lemma]
>$$\frac{1}{2}+\cos {t}+\cos{2t}+\ldots+\cos{nt}=\frac{\sin((n+\frac{1}{2})t)}{2\sin{\frac{t}{2}}}$$
>
>---
>[[Dimostrazione per induzione]] a pag 5 appunti argomento4c

>[!prp] Disuguaglianza di Bessel
>Supponiamo $f:[-\pi,\pi]\to\mathbb{R}$ funzione limitata ed [[Integrabile secondo Rienmann - spazi metrici|Integrabile secondo RIenmann]].
>Se $a_{0},a_{k},b_{k}$ sono i coefficienti di Fourier, si ha$$\frac{a_{0}^{2}}{2}+\sum_{k\ge 1}\left(a_{k}^{2}+b_{k}^{2}\right)\le \frac{1}{\pi}\int_{-\pi}^{\pi}|f(x)|^{2}dx$$
>
>---
>dimostrazione pagina 6 argomento 4c
>
>>[!nota] Identità di Parseval
>>Se $f\in C^{1}$ ed è $2\pi$-[[#^88ecc8|periodica]] su $\mathbb{R}$ vale l'uguaglianza

^0bb00e

> [!theorem]
>Sia $f:[-\pi,\pi]\to \mathbb{R}$ una [[#^88ecc8]] limitata.
>Allora la serie di Fourier $$\frac{a_{0}}{2}+\sum_{k\ge 1}\left(a_{k}\cos kx+ b_{k}\sin kx\right)$$
>converge puntualmente a $$\frac{f(x^{+})+f(x^{-})}{2}$$
>dove $f(x^{+})=\lim_{\bar x\to x^{+}}f(\bar x)$ e $f(x^{-})=\lim_{\bar x\to x^{-}}f(\bar x)$
>>[!nota] 
>>Se $f(x)$ è continua in $\bar x$
>>
>>$$\Rightarrow S_{n}(\bar x)\to \frac{f(\bar x^{+})+f(\bar x^{-})}{2}=f(\bar x)$$
>> Se $\bar x$ è un punto di salto
>> $$\Rightarrow S_{n}(\bar x)\to \frac{f(\bar x^{+})+f(\bar x^{-})}{2}\mbox{(può non coincidere con } f(\bar x) )$$
>---
>Dimostrazione a pagina 11 argomento 4c

>[!thm]
>Sia $f : \mathbb{R}\to \mathbb{R}$ di [[Classi di funzioni#^08c68a]] e $2\pi$-[[#^88ecc8|periodica]].
>$$S_{n}\to f \mbox{ totalmente su }[-\pi,\pi]$$
>---
>[[Serie di funzioni#^98ab3e]]
>Dimostrazione pag 17 argomento4c





 

