---
pagina: 209
---
# Definizione
Sia $V$ [[Spazio euclideo]] con $\mathbb{K} = \mathbb{R}\ o\ \mathbb{C}$
Sia $<.,.>$ prodotto scalare definito su $V$.
$\forall \mathbb{X}\subseteq V$
$\mathbb{X}^\perp:=\{y\in V:y\perp x, \forall x\in \mathbb{X}\}\subseteq V$

# Proposizione
$\mathbb{X}^\perp$ è un [[Sottospazio lineare|sottospazio lineare]] di $V$, $\forall \mathbb{X}\subseteq V$
#dimostrazione-da-fare 

# Esempi
guarda su appunti

# Proprietà
1) $$\mathbb{X}^{\perp} \cap \mathbb{X} \subseteq \{0\}\qquad \forall \mathbb{X}\subseteq V$$
#dimostrazione-da-fare 
2) $$\mathbb{X}^{\perp}=V\iff(\mathbb{X}=\varnothing)\lor(\mathbb{X}=\{0\})$$
#dimostrazione-da-fare 
3) $V^{\perp}=\{0\}$
4) $\mathbb{X}\subseteq \mathbb{Y}\Rightarrow \mathbb{X}^\perp\supseteq \mathbb{Y}^\perp\qquad\forall\mathbb{X},\mathbb{Y}\subseteq V$
#dimostrazione-da-fare  ^7ece09
* Se $dim(V)=n$ allora $L(\mathbb{X}\subseteq L(\mathbb{Y}))\iff\mathbb{X}^{\perp}\supseteq \mathbb{Y}^\perp$
5) $\mathbb{X}^{\perp}=L(\mathbb{X})^{\perp}$ 
#dimostrazione-da-fare 
6) $\mathbb{X}^{\perp}=L(\mathbb{X}^{\perp})$
7) $L(\mathbb{X})\subseteq(\mathbb{X}^{\perp})^{\perp}\qquad \forall \mathbb{X}\subseteq V$
#dimostrazione-da-fare 
- Se $dim(V)=n$ allora $(\mathbb{X}^{\perp})^{\perp}=L(\mathbb{X})$
- $L(\mathbb{X})\subseteq (\mathbb{X}^{\perp})^{\perp}\Rightarrow \mathbb{X}\subset (\mathbb{X}^{\perp})^{\perp}$
8) $(\mathbb{X}\cup\mathbb{Y})^{\perp}=\mathbb{X}^{\perp}\cap \mathbb{Y}^{\perp}\qquad \forall \mathbb{X},\mathbb{Y}\subseteq V$
#dimostrazione 
- $\{A_1,A_2,\ldots,A_m\}=A_{1}^{\perp}\cap A_{2}^{\perp}\cap\ldots\cap A_{m}^{\perp}$
9) $L(\mathbb{X}^{\perp}\cup \mathbb{Y}^{\perp})\subseteq (L(\mathbb{X})\cap L(\mathbb{Y}))^{\perp}\qquad \forall \mathbb{X},\mathbb{Y}\subseteq V$
#dimostrazione-da-fare 
- Se $dim(V)=n$ allora $L(\mathbb{X}^{\perp}\cup \mathbb{Y}^{\perp})=(L(\mathbb{X})\cap L(\mathbb{Y}))^{\perp}$

# Proposizione
 Sia $V$ [[Spazio euclideo]].
 Siano $A$ e $B$ due [[Sottospazio lineare|sottospazi lineari]] di $V$.
 $$\Rightarrow (A+B)^{\perp}= A^{\perp}\cap B^{\perp}$$
 #dimostrazione-da-fare 
# Lemma delle proiezioni
[[Somma diretta]]
Sia $V$ uno [[Spazio euclideo]] di $dim(V) = n$ e $S$ un [[Sottospazio lineare|sottospazio lineare]] di $V$ con $dim(S)=m$
Se esiste una [[Base ortogonale e ortonormale|base ortogonale]] di $S$
Allora $V = S \oplus S^\perp$
#dimostrazione-da-fare 