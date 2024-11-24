---
pagina: 257
collegamenti:
  - "[[Kernel di una funzione lineare|Kernel]]"
---
# Proposizione 1
Sia $\varphi:V\to W$ [[Trasformazione lineare|funzione lineare]]
Sia $\mathcal{Y}$ [[Sottospazio lineare|sottospazio lineare]] di $W$.
Allora $\varphi^{-1}(\mathcal{Y})$ è un sottospazio lineare di $V$.
#dimostrazione-da-fare 

# Proposizione 2 | Iniettività
$$\varphi\mbox{ iniettiva}\iff null(\varphi)=0$$
#dimostrazione-da-fare 
# Proposizione 3
Sia $\varphi:V\to W$
$$\forall Y\mbox{ sottospazio lineare di W}, ker(\varphi)\subseteq\varphi^{-1}(Y)$$
# Proposizione 4
Sia $\varphi:V\to W$
Sia $b \in W$
- $B \not \in W, \varphi^{-1}(b) = \varnothing$
- $B \in W \Rightarrow \varphi^{-1}(b)= p + ker(\varphi), \varphi(p) = b$
$dim(\varphi^{-1}(b))= null(\varphi)$

# Proposizione 5
Sia $\varphi:V\to W$ [[Trasformazione lineare|funzione lineare]].
Sia $A$ [[Sottospazio lineare|sottospazio lineare]] di $V$.
Allora $\varphi(A)$ è sottospazio lineare di $W$ e 
$$dim(\varphi(A))=dim(A)-dim(A\cap ker(\varphi))$$
#dimostrazione-da-fare [[Teorema di nullità + rango]]   

# Proposizione 6
Sia $\varphi:V\to W$ [[Trasformazione lineare|funzione lineare]].
Sia $S$ un [[Sottospazio affine|sottospazio affine]] di $V$.
$S = P+S_{0}$, $S_0$ [[Sottospazio lineare|sottospazio lineare]] di $V$.
Allora $$\varphi(S)=\varphi(P)+\varphi(S_{0})$$
- $\varphi(P)+\varphi(S_{0})$ è un sottospazio affine di $W$.
#dimostrazione-da-fare 
$$dim(\varphi(S))=dim(\varphi(S))-dim(S_{0}\cap ker(\varphi))$$ 
# Proposizione 7
Sia $\varphi:V\to W$ [[Trasformazione lineare|funzione lineare]].
Sia $Y$ [[Sottospazio lineare|sottospazio lineare]] di $W$.
Allora, come abbiamo già visto $\varphi^{-1}(Y)$ è un sottospazio lineare. ([[Proposizioni funzioni lineari#Proposizione 1|QUI]])
$$dim(\varphi^{-1}(Y))= null(\varphi)+dim(Im(\varphi)\cap Y)$$
#dimostrazione-da-fare 

# Proposizione 8
Sia $\varphi:V\to W$ [[Trasformazione lineare|funzione lineare]].
Sia $S$ un [[Sottospazio affine|sottospazio affine]] di $W$.
#dimostrazione-da-fare 
$$\varphi^{-1}(S)=P+\varphi^{-1}(S_{0})$$
e $$dim(\varphi^{-1}(S))=dim(\varphi^{-1}(S_{0}))=null(\varphi)+dim(S_{0}\cap Im(\varphi))$$