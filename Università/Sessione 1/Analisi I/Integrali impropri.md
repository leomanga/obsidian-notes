---
capitolo: 19.7
---
La teoria dell'[[Integrale superiore e inferiore. Funzioni integrabili secondo Rienmann|integrazione secondo Riemann]] è stata svolta sotto due ipotesi sulla funzione $f$ da integrale.
Il dominio di $f$ doveva essere un [[Chiusura di un insieme|intervallo chiuso e limitato]] e la funzione $f$ doveva essere limitata.
Lo scopo adesso è quello di provare ad eliminare queste ipotesi.

# Definizione 19.7.1 | Funzione localmente integrabile
Sia $I\subseteq \mathbb{R}$ un intervallo. Si dice che $f$ è localmente integrabile secondo Riemann in $I$ se $f:I\to\mathbb{R}$ è localmente limitata in $I$, e per ogni $[a,b]\subset I$ si ha che $f$ è integrabile secondo Riemann in $[a,b]$.

# Definizione 19.7.1 | Integrale improprio su in intervallo limitato semiaperto
Sia $f:[a,b)\to\mathbb{R}$ una funzione localmente integrabile in $[a,b)$.
Si dice che $f$ è integrabile in senso improprio o generalizzato su $[a,b)$ se esiste finito
$$\lim_{c\to b^{-}}\int_{a}^{c}f(x)dx$$
Indicheremo con questo simbolo
$$\int_{a}^{b}f(x)dx$$
tale limite.
Cosa simile per $(a,b]$, con $a^{+}$.
# Definizione | Integrale improprio su una semiretta
Sia $f:[a,+\infty)\to\mathbb{R}$ una [[#Definizione 19.7.1 Funzione localmente integrabile|funzione localmente integrabile]]. Si dice che $f$ è integrabile in senso improprio in $[a,+\infty]$ se esiste finito
$$\lim_{c\to+\infty}\int_{a}^{c}f(t)dt$$
Indicheremo questo limite con il simbolo
$$\int^{+\infty}_af(x)dx$$
Cosa simile per $(-\infty,b]$

# Criterio del confronto 1
Siano $f,g:[a,b)\to\mathbb{R}$ due funzioni positive e localmente integrabili in $[a,b)$, tali che $f\le g$. 
Se $g$ è integrabile in senso improprio in $[a,b)$, allora anche $f$ è integrabile in senso improprio in $[a,b)$.
# Criterio del confronto 2
Siano $f,g:[a,+\infty)\to\mathbb{R}$ due funzioni positive e localmente integrabili in $[a,+\infty)$, tali che $f\le g$. 
Se $g$ è integrabile in senso improprio in $[a,+\infty)$, allora anche $f$ è integrabile in senso improprio in $[a,+\infty)$.
# Criterio del confronto asintotico
Siano $f,g:[a,b)\to\mathbb{R}$ due funzioni positive localmente integrabili in $[a,b)$ tali che 
$$\exists\lim_{x\to b^{-}}\frac{f(x)}{g(x)}=L\in[0,+\infty]$$
Allora:
$$\begin{split}&\mbox{se L}<+\infty, \\&g\mbox{ integrabile in senso improprio}\Rightarrow f\mbox{ integrabile in senso improprio}\end{split}$$
- Vuol dire che $g$ converge.
$$\begin{split}&\mbox{se L}>0, \\&g\mbox{ non integrabile in senso improprio}\Rightarrow f\mbox{ non integrabile in senso improprio}\\
&f\mbox{ integrabile in senso improprio}\Rightarrow g\mbox{ integrabile in senso improprio}\end{split}$$
- Vuol dire che $f$ diverge.
$$\begin{split}&\mbox{se }0<L<+\infty, \\&f\mbox{ integrabile in senso improprio}\iff g\mbox{ integrabile in senso improprio}\end{split}$$
# Teorema 19.7.11 | funzione assolutamente integrabile
Sia $f:[a,+\infty]\to\mathbb{R}$ una funzione localmente limitata e localmente integrabile in $[a,+\infty]$. 
Se $|f|$ è integrabile in senso improprio in $[a,+\infty)$ allora anche $f$ è integrabile in senso improprio in $[a,+\infty)$ e si ha
$$\left|\int_{a}^{+\infty}f(x)dx\right|\le\int_{a}^{+\infty}|f(x)|dx$$
# Teorema del confronto
Sia $\varphi:[a,b)\to[0,+\infty)$ con $b\in(a,+\infty]$ una funzione integrabile in senso improprio in $[a,b)$, e supponiamo che $f:[a,b)\to\mathbb{R}$ sia una funzione localmente integrabile in $[a,b)$ tale che
$$|f(x)|\le\varphi(x)\quad \forall x\in [a,b)$$
Allora $f$ è integrabile in senso improprio un $[a,b)$.

# Definizione | Integrale improprio per punto singolare
Sia $f:[a,b]\setminus\{c\}\to\mathbb{R}$ una funzione con $a<c<b$
Supponiamo che $f$ sia localmente limitata e localmente integrabile in $[a,c)$ e in $(c,b]$.
Si dice che $f$ è integrabile in senso improprio in $[a,b]$ se esistono finiti i due limiti
$$\lim_{d\to c^-}\int_a^{d}f(x)dx,\quad\lim_{e\to c^{+}}\int_{e}^{b}f(x)dx$$
E scriveremo questi limiti con il simbolo
$$\int_{a}^{b}f(x)dx$$
la somma dei due limiti.
