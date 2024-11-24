---
pagina: 10
collegamenti: "[[Chiusura di un insieme]]"
---

[[Spazi metrici#Definizione insieme aperto]] 
[[Spazi metrici#Definizione insieme chiuso]]
# Definizione | insieme aperto
Dato $A\subseteq \mathbb{R}$, si dice aperto se $\forall x\in A \exists\  r>0:B_r(x)\subseteq A$.
$B_r$ è una [[Spazi metrici#Definizione palla|palla]].
# Definizione | insieme chiuso
Dato $C\subseteq\mathbb{R}$, si dice chiuso se $A^C$ è [[Chiusura di un insieme - spazi metrici#Definizione insieme aperto|aperto]]. Dove $A^{C}=\mathbb{R}\setminus A$.
# Corollario
Un insieme $C\subseteq X$ è chiuso $\iff \forall (x_n)\subseteq C:x_{n}\to x$ quando $n\to +\infty$ si ha $x\in C$
# Definizione | Punto di accumulazione
Sia $E\subseteq X$, dove $(X,d)$ è uno [[Spazi metrici|spazio metrico]] e sia $x\in X$.
Diremo che $X$ è un punto di accumulazione per $E$ se $$\forall r>0\ \exists y\in E, y\not=x:y\in E\cap B_r(x)$$
Stessa cosa se è verificata $$\forall n>0\ \exists y_{n}\in B_{\frac{1}{n}}(x)\cap E, y_{n}\not= x$$
### Osservazione 1
Se $x$ è un punto di accumulazione per $E$, non è necessariamente vero che $x$ appartenga ad $E$.
### Osservazione 2
Se $x\in E$ non è detto che $x$ sia di accumulazione per $E$.
Ad esempio $E=N^2$ non ha punti appartenenti ad $E$ che stiano dentro alla pallina di raggio $< 1$.
==IN QUESTO CASO SI PARLA DI PUNTO ISOLATO==
# Definizione | Chiusura
$E\subseteq X$, indicheremo con $\bar E$ la chiusura di $E$ in $X$.
$$\bar E=\bigcap_{C\ chiuso, C\supseteq E} C\Rightarrow \mbox{è chiuso}$$
# Definizione | Parte interna
$E\subseteq X$, indicheremo con $\mathring{E}$ la parte interna di $E$ in $X$.
$$\mathring{E}=\bigcup_{A\ aperto, A\subseteq E}A\Rightarrow\mbox{è aperto}$$
# Lemma 1
Sia $C\subseteq X$ un insieme chiuso e sia $(x_{n})\subseteq C$ [[Limite in un punto - spazi metrici#Definizione successione convergente|convergente]].
Allora $x\in C$.
#dimostrazione-da-fare [[Dimostrazione per assurdo]] pg 8
# Lemma 2
Sia $E\subseteq X$. Allora $x\in \bar E$ se e solo se esiste una successione $(x_n)\subseteq E$ tale che $x_{n}\to x.$
#dimostrazione-da-fare pg 8
# Definizione | Insieme compatto
$(X,d)$ [[Spazi metrici|spazio metrico]].
Sia $K\subseteq X$ insieme non vuoto.
Allora $K$ si dice compatto se vale la seguente proprietà:
Dati $\{A_i\}_{i\in I}$ insiemi aperti tali che $\cup_{i\in I} A_{i}\supseteq K$. 
Allora $\exists I^{'}\subseteq I$ tale che $I^{'}$ è un insieme finito e $K\subseteq \cup_{i\in I^{'}}A_{i}$ 
# Definizione | Insieme compatto per successioni
$K\subseteq X$ si dice compatto per successioni se vale la seguente proprietà:
$$\forall(x_n)\subseteq K\Rightarrow\exists\mbox{ una sottosucessione }(x_{n_{k}})\subseteq K: x_{n_{k}}\to x\in K$$
# Teorema
Sia $(X,d)$ [[Spazi metrici|spazio metrico]].
Allora le seguenti affermazioni sono equivalenti.
$(i)K\subseteq X$ è [[Chiusura di un insieme - spazi metrici#Definizione Insieme compatto|compatto]]
$(ii)K\subseteq X$ [[Chiusura di un insieme - spazi metrici#Definizione Insieme compatto per successioni|compatto per successioni]]
$(iii)K\subseteq X$ [[Spazio metrico completo#Definizione Spazio metrico completo|completo]] o [[Chiusura di un insieme - spazi metrici#Definizione Chiusura|chiuso]][^1]e [[Spazio metrico limitato e totalmente limitato#Definizione Spazio metrico totalmente limitato|totalmente limitato]].

# Proposizione
In $\mathbb{R}^{n}$ che è [[Spazio metrico completo#Definizione Spazio metrico completo|completo]], $K$ è [[Chiusura di un insieme - spazi metrici#Definizione Insieme compatto|compatto]] $\iff$ è [[Chiusura di un insieme - spazi metrici#Definizione Chiusura|chiuso]] e [[Spazio metrico limitato e totalmente limitato#Definizione Spazio metrico limitato|limitato]]. (Dato che è anche totalmente limitato)


[^1]: da [[Spazio metrico completo#Corollario completo $ iff$ chiuso]].
