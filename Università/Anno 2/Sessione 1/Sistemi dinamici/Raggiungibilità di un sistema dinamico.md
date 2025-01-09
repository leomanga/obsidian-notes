---

---
Notazioni:
In questo documento $T$ viene usata come numero, quindi $A^{T}$ è una matrice elevata alla $T$. Per il simbolo del trasposto si usa $'$.

--- 

>[!def] Raggiungibilità in un sistema dinamico a tempo discreto
>Uno stato $\bar x \in \mathbb{R}^{n}$ si dice raggiungibile in $k$ passi (dallo stato zero) se, assumendo $x(0)=0$, esiste una sequenza di passi $u(0),u(1),\ldots,u(k-1)$ tale che $x(k)=\bar x$.

## Studio della raggiungibilità | problema del controllo
Dato un sistema [[Sistemi lineari tempoinvarianti|LTI]] a tempo discreto
$$\begin{cases}
x(k+1)=Ax(k)+Bu(k)\\ 
y(k)=Cx(k)+Du(k)\\
x(0)=x_{ini}
\end{cases}$$
Noi cerchiamo per un certo $T$, $x(T)=x_{fin}$. 
Lo scopo è quello di determinare, se possibile, la sequenza di ingressi $u(0),u(1),\ldots,u(T-1)$ tale da portare lo stato da $x_{ini}$ a $x_{fin}$.
Da [[Analisi modale nello spazio degli stati per sistemi a tempo discreto]] abbiamo che
$$x(k)=x_{l}(k)+x_{f}(k)=A^{k}x(0)+\sum_{i=0}^{k-1}A^{k-1-i}Bu(i)$$

Possiamo imporre $$A^{T}x_{ini}+\sum_{i=0}^{T-1}A^{T-1-i}Bu(t)=x_{fin}$$
Riscrivendo in forma matriciale abbiamo
$$
\underbrace{\begin{bmatrix}
B&&AB&&A^{2}B\ \cdots \ A^{T-1}B
\end{bmatrix}}_{\mathcal{R}_{T}}
\begin{bmatrix}
u(T-1) \\ u(T-2) \\ \vdots  \\ u(0)
\end{bmatrix}=x_{fin}-A^{T}x_{ini}
$$

^9e9296

dove $x\in \mathbb{R}^{n}$, $u\in \mathbb{R}^{m}$ e $\mathcal{R}_{T}\in \mathbb{R}^{n\times Tm}$ e viene definita

>[!def] Matrice di raggiungibilità in $T$ passi
>La matrice di raggiungibilità è la matrice $\mathcal{R}_{T}\in \mathbb{R}^{n\times Tm}$
>$$\mathcal{R}_{T}=\begin{bmatrix}
B&&AB&&A^{2}B\ \cdots \ A^{T-1}B
\end{bmatrix}$$

^e41c75

Dal [[Teorema di Rouchè-Capelli]], il problema ammette soluzione se e solo se 
$$x_{fin}-A^{T}x_{ini}\in Im(\mathcal{R}_{T})$$
(Se non appartenesse all’immagine, la matrice completa avrebbe un rango maggiore di quella incompleta e il sistema non sarebbe risolubile)

>[!def] Stato raggiungibile in $k$ passi
>Uno stato $\bar x\in \mathbb{R}^{n}$ si dice raggiungibile in $k$ passi (dallo stato zero) se, assumendo $x(0)=0$, esiste una sequenza di ingressui $u(0), u(1),\ldots,u(k-1)$ tale che $x(k)=\bar x$.

^f26ad0

>[!prp] Raggiungibilità di uno stato
>Lo stato $\bar x$ è [[#^f26ad0|raggiungibile in $k$ passi]]  se e solo se $\bar x\in Im(\mathcal{R}_{k})$ dove $\mathcal{R}_{k}$ è la [[#^e41c75|matrice di raggiungibilità in $k$ passi]].

Definiamo il sottospazio
>[!def] Insieme degli stati raggiungibili in $k$ passi
$$X_{k}^{\mathcal{R}}=Im(\mathcal{R}_{k})$$

Quindi il sottospazio raggiungibile in un passo sarà 
$$X_{1}^{\mathcal{R}}=Im(R_{1})=Im(B)$$quello raggiungibile in due passi sarà
$$X_{2}^{\mathcal{R}}=Im(R_{2})=Im\begin{bmatrix}B&AB\end{bmatrix}\supseteq X_{1}^{\mathcal{R}}$$
quello raggiungibile in tre passi sarà
$$X_{3}^{\mathcal{R}}=Im(R_{3})=Im\begin{bmatrix}B&AB&A^{2}B\end{bmatrix}\supseteq X_{2}^{\mathcal{R}}$$
e così via.
Avremo quindi in generale che 
$$X_{1}^{\mathcal{R}}\subseteq X_{2}^{\mathcal{R}}\subseteq X_{3}^{\mathcal{R}}\subseteq\ldots X_{k}^{\mathcal{R}}\subseteq X_{k+1}^{\mathcal{R}}\subseteq \ldots$$

>[!def] Sistema completamente raggiungibile
>Im sistema si dice completamente raggiungibile se $$\exists k:X_{k}^{\mathcal{R}}=\mathbb{R}^{n}$$
>ovvero $$rank(\mathcal{R}_{k})=n$$
>dove $n$ è il numero di stati.

^04bbfd

Enunciando

>[!thm] Teorema di Cayley-Hamilton
>Data $A\in \mathbb{R}^{n\times n}$, sia $$p(\lambda)=\det(\lambda I-A)=\lambda^{n}+\alpha_{n-1}\lambda^{n-1}+\ldots +\alpha_{0}$$
>Allora $$A^{n}+\alpha_{n-1}A^{n-1}+\ldots+\alpha_{0}I=0$$

Pag 107 per spieazione #da-finire 

>[!prp]
>L’insieme degli stati raggiungibili in un qualunque numero di passi coincide con $$X_{n}^{\mathcal{R}}=Im(\mathcal{R}_{n})$$

>[!def] Matrice di raggiungibilità del sistema
>$$\mathcal{R}:=\mathcal{R}_{n}$$ si dice matrice di raggiungibilità del sistema.

>[!def] Sottospazio raggiungibile del sistema
>$$X^{R}:=Im (\mathcal{R})$$
>si dice sottospazio raggiungibile del sistema.

# Calcolo della sequenza di ingressi
Consideriamo l’equazione [[#^9e9296]]
$$\mathcal{R}_{T}\cdot\underbrace{\begin{bmatrix}u(T-1)\\u(T-2)\\\vdots\\u(0)\end{bmatrix}}_{\mathcal{U}}=\underbrace{x_{fin}-A^{T}\cdot x_{in}}_{v}\iff\mathcal{R}_{T}\cdot U_{T}=v$$
dove $\mathcal{R}_{T}\in \mathbb{R}^{n\times Tm}$, $U_{T}\in \mathbb{R}^{mT\times 1}$ e $v\in \mathbb{R}^{n\times 1}$
Consideriamo diversi casi
- $m=1$ e $T=n$ ($1$ ingresso e $T$ passi). Avremo $\mathcal{R}\in \mathbb{R}^{n\times n}$. Se $rank(\mathbb{R}_{n})=n$ allora il sistema è [[#^04bbfd|completamente raggiungibile]] ed esiste un unica soluzione.$$\mathcal{U}=\mathbb{R}_{n}^{-1}v$$
- il caso generale $mT>n$ . Avremo che se il sistema è [[#^04bbfd|completamente raggiungibile]], allora si hanno $\infty^{mT-n}$ soluzioni.
Studiando il caso generale avremo
#da-finire pag 109
Chiamando $\bar{\mathcal{U}}$ una soluzione particolare,

$$
\bar{\mathcal{U}}=\mathcal{R}_{T}'({R}_{T}{R}_{T}')^{-1}v
$$

^f9ca0f

# Problema del controllo a minima energia
Dovrebbe essere ![[#^f9ca0f]]
#da-finire pag 110

[[Decomposizione di raggiungibilità]]
[[Problema del controllo]]