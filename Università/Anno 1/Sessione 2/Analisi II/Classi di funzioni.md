Queste classi di funzioni sono [[Spazio vettoriale|spazi vettoriali]] ed hanno [[Norma]]. Sono quindi [[Spazi metrici|spazi metrici]]. ^283b88

>[!def] Classe di funzioni $C_{b}(E)$
>Sia $E\subseteq \mathbb{R}^{n}$. Denotiamo con $C_{b}(E)$ l'insieme $$C_{b}(E)=\{f:E\to\mathbb{R}\mbox{ continua su E e limitata}\}$$
>Dotiamo inoltre questo spazio con la norma [[Norma infinito]].

^1b877f

>[!def] Classe di funzioni $C^{1}$
>%%display:classe $C^{1}$%%
>Dato un intervallo $[a,b]$, dico che $f:[a,b]\to\mathbb{R}$ è di classe $C^{1}$ su $[a,b]$ se $f$ è [[Funzione derivabile|derivabile]], $f^{'}(a^{+}):=\lim_{h\to o^{+}}\frac{f(h+a)-f(a)}{h}$, $f^{'}(b^{-}):=\lim_{h\to 0^{-}}\frac{f(b+h)-f(b)}{h}$ e la derivata $f^{'}:[a,b]\to\mathbb{R}$ definita come $$f^{'}(x)=\begin{cases}f^{'}(a^{+})\qquad se\ x=a\\ f^{'}(x)\qquad se\ x\in(a,b)\\f^{'}(b^{-})\qquad se \ x=b\end{cases}$$
> Definisco $C^{1}([a,b])=\{f:[a,b]\to\mathbb{R}$ che sono di classe  $C^{1}$ su $[a,b]\}$
> Dotiamo questo spazio con la norma 
> $$||f||_{C^{1}}:=||f||_{\infty}+||f^{'}||_{\infty}$$
> ---
> ![[Serie di fourier#^3892cb]]

^08c68a

^beec38
>[!def] Classe di funzioni $C^{\infty}$
>%%display:classe $C^{\infty}$%%
>Una funzione è di classe $C^{\infty}$ se $\lim_{n\to \infty}f^{(n)}(x)$ è di classe $C^{1}$.
>

^7dda87

