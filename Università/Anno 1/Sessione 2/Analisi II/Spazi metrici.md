---
aliases:
  - Spazio metrico
  - spazio metrico
  - spazi metrici
---
# Definizione
Uno spazio metrico è un insieme $X$ in cui è definita una [[Funzione distanza]] $d:X\times X\to[0,+\infty]$ per ogni coppia di punti $x,y\to X$.
Il simbolo $d(x,y)$ denota la distanza fra $x$ e $y$.
La coppia ($X$, d) prende il nome di spazio metrico. 
(Supponiamo sempre $X\not = \varnothing$).
# Osservazione
Se ($X,d$) è uno spazio metrico e $Y\subseteq X,$ con $Y\not = \varnothing$, allora $(Y,d)$ è anch'esso uno spazio metrico.
# Esempi
- $\mathbb{R}$ è uno spazio metrico, $d(x,y)=|x-y|$.
- Da [[Spazi metrici#Osservazione|osservazione]], dato che $\mathbb{Q}\subseteq \mathbb{R}$ è uno spazio metrico, e $d(x,y)=|x-y|$.
- $E\subseteq \mathbb{R}$, allora $(E,d)$ è uno spazio metrico.
- $\mathbb{R}^{n}=\underbrace{\mathbb{R}\times\ldots\times \mathbb{R}}_{n\ volte}$
- ##### Nel caso $\mathbb{R}^2$, $d$ si può calcolare con Pitagora.
$$\underbrace{d_{e}}_{distanza\ euclidea}=(p,q)=\sqrt{(p_1-q_1)^2+(p_2-q_2)^2}=||p-q||$$
	- Possono esserci anche altre nozioni di distanza in $\mathbb{R}^{2}$, per esempio $d_{1}(p,q)=|p_1-q_1|+|p_2-q_2|$.
		 #dimostrazione-da-fare 
	- $d_{\infty}(p,q)=max\{|p_1-q_1|,|p_2-q_2|\}$
		 #dimostrazione-da-fare 
	- La distanza definita con il minimo non è una distanza dato che non verifica le [[Funzione distanza#Proprietà|proprietà]] della distanza.
- ##### In $\mathbb{R}^n$
	- $d_e(p,q)=(\sum_{i=1}^n|p_i-q_i|^2)^{1/2}$ 
	- $d_1(p,q)=\sum_{i=1}^{n}=|p_i-q_i|$
	- $d_\infty(p,q)=\max\{|p_i-q_i|,i=1,\ldots,n\}$
# Proprietà
Dati $x,y,z\in X$
$|d(x,y)-d(z,y)|\le d(x,z)$
#dimostrazione-da-fare 

Nel caso particolare in cui $d(x,y)=||x-y||$ dove $x,y\in\mathbb{R}$ ovvero $d(x,y)=d_e(x,y)$, la proprietà appena dimostrata dice che $\forall x,y,z\in\mathbb{R}$ $| \Vert x-y\Vert-\Vert x-z\Vert|\le||y-z||$

# Definizioni
- [[Palla]]
- [[Disco]]
- [[Chiusura di un insieme - spazi metrici#Definizione insieme aperto|insieme aperto]]
- [[Chiusura di un insieme - spazi metrici#Definizione insieme chiuso|insieme chiuso]]
# Proposizione 1
$\varnothing$ è sia aperto che chiuso. 
È aperto per definizione, mentre è aperto perché $A=\mathbb{R}$ è aperto per la definizione della [[Spazi metrici#Definizione palla|palla]].
Allora $A^C$ ([[Complementare]]) è chiuso, quindi $\varnothing$ è chiuso.
Stessa cosa per $\mathbb{R}$.
# Proposizione 2
$A$ è aperto $\iff$ $A^{c}=X\setminus A$ è chiuso
# Proposizione 3 | L'unione di insiemi aperti è un insieme aperto
Se $A_i$ sono aperti, dove $i\in I, I$ un insieme di indici. 
Allora $\cup_{i\in I}A_i=A$, che è aperto. 
# Proposizione 4| L'intersezione di insiemi chiusi è un insieme chiuso
Se $C_i$ sono insiemi chiusi, $i\in I,I$ un insieme di indici.
Allora $\cap_{i\in I}C_i=C$ è [[Chiusura di un insieme - spazi metrici#Definizione insieme chiuso|chiuso]]|.