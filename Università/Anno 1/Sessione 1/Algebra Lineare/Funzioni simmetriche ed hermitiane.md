---
pagina: 292
aliases:
  - Trasformazioni simmetriche ed hermitiane
---
# Teorema | esistenza funzione lineare
Siano $V$ e $W$ due [[Spazio euclideo|spazi euclidei]] definiti nello stesso [[Campo]] $\mathbb{K}$.
$\varphi:V\to W$ [[Trasformazione lineare|funzione lineare]].
$\underbrace{<.,.>_{V}}_{\mathbb{E}},\underbrace{{<.,.>}_{W}}_{F}$
Allora esiste ed è unica la [[Trasformazione lineare|funzione lineare]]
$$\theta:W\to V\mbox{ tale che} <\varphi(x),y>_{W}=<x,\theta(y)>_{V},\forall x\in V, \forall y \in W$$
### Trasposta di f
 Se $\mathbb{K}=\mathbb{R}$
 $\varphi^{T}:=\theta$ è detta TRASPOSTA di $\varphi$ 
$<\varphi(x),y>_{W}=<x,\varphi^{T}(y)>_{V}$
### Aggiunta di f
Se $\mathbb{K}=\mathbb{C}$
 $\varphi^{*}:= \theta$ è detta AGGIUNTA di $\varphi$
 $<\varphi(x),y>_{W}=<x,\varphi^{*}(y)>_{V}$  
### Proprietà nei Reali
- $I^{T}=I$
- $\varphi^{TT}=\varphi$
- $(a\varphi+b\psi)^{T}=a\varphi^{T}+b\psi^{T}\quad \forall a,b\in \mathbb{R} \varphi\to \varphi^{T}$è una funzione lineare
- $(\psi\circ \varphi)^{T}=\varphi^{T}\circ\psi^{T}$
- $\mu_{E,F}(\varphi^{T})=\mu_{E,F}(\varphi)^{T}$
### Proprietà nei Complessi
- $I^{*}=I$
- $\varphi^{**}=\varphi$
- $(a\varphi+b\psi)^{*}=\bar a\varphi^{*}+\bar b\psi^{*}\quad \forall a,b\in \mathbb{C} \varphi\to \varphi^{*}$è una funzione semi lineare
- $(\psi\circ \varphi)^{*}=\varphi^{*}\circ\psi^{*}$
- $\mu_{E,F}(\varphi^{*})=\mu_{E,F}(\varphi)^{*}$ (Consiste nel fare la trasposta e la coniugata)

# Definizione | funzione simmetrica
Sia $V=W$ [[Spazio euclideo|spazio euclideo]].
$\varphi:V\to W$ [[Trasformazione lineare|funzione lineare]].
$\mathbb{K}=\mathbb{R}$
$\varphi$ è SIMMETRICA se $\varphi=\varphi^{T}$([[Funzioni simmetriche ed hermitiane#Trasposta di f|trasposta]]), cioè
$$<\varphi(x),y>_{V}=<x,\underbrace{\varphi(y)}_{=\varphi^{T}}>_{V}\quad\forall x,y\in V$$
### Definizione matrici | Matrice simmetrica
Se $\varphi$ è simmetrica, allora $\mu_{E,F}(\varphi^{T})=\mu_{E,F}(\varphi)^{T}$, allora $M$ è una matrice simmetrica($a_{ij}=a_{ji},j\not= i$) 

### Teorema spettrale
[[Teorema spettrale]]
# Definizione | funzione hermitiana
Sia $V=W$ [[Spazio euclideo|spazio euclideo]].
$\varphi:V\to W$ [[Trasformazione lineare|funzione lineare]].
$\mathbb{K}=\mathbb{C}$
$\varphi$ è SIMMETRICA se $\varphi=\varphi^{*}$([[Funzioni simmetriche ed hermitiane#Aggiunta di f|aggiunta]], cioè
$$<\varphi(x),y>_{V}=<x,\underbrace{\varphi(y)}_{=\varphi^{*}}>_{V}\quad\forall x,y\in V$$
### Definizione matrici | Matrice hermitiana
Se $\varphi$ è simmetrica, allora $\mu_{E,F}(\varphi^{*})=\mu_{E,F}(\varphi)^{*}= =\mu_{E,F}(\varphi)^{-T}$, allora $M$ è una matrice hermitiana ($a_{ij}=a_{ji},j\not= i$) $\begin{cases} a_{ij}=\bar{a_{ji}},i\not=0\\ a_{ii}=\bar{a_{ii}}\iff(a_{ii}\in\mathbb{R}) \end{cases}$
# Teorema | autovalori di una funzione hermitiana
Gli [[Autovettori - autovalori - autospazi|autovalori]] di una funzione hermitiana sono numeri reali.
#dimostrazione-da-fare 
# Teorema | ortogonalità degli autovettori
Sia $\varphi:V_n(\mathbb{C})\to V_{n}(\mathbb{C})$ una funzione hermitiana.
Siano $a,b$ due [[Autovettori - autovalori - autospazi|autovalori]] di $\varphi$ con $a\not= b$.
Siano $A,B$ [[Autovettori - autovalori - autospazi|autovettori]] di $a$ e $b$ rispettivamente($\varphi(A)=aA,\varphi(B)=bB$.
$$\Rightarrow A\perp B$$
#dimostrazione-da-fare 
# Teorema | f-invarianza di un ortogonale
Sia $\varphi:V_n(\mathbb{C})\to V_{n}(\mathbb{C})$ una funzione hermitiana.
Sia $A$ un [[Sottospazio lineare|sottospazio lineare]] di $V_n(\mathbb{C})$, $\varphi$ è [[f-invariante e fissato da f|f-invariante]].
$$\Rightarrow A^{\perp}\mbox{ è }\varphi\mbox{-invariante}$$
#dimostrazione-da-fare 
# Corollario
Se $\varphi$ è una trasformazione hermitiana e $A$ è un [[Autovettori - autovalori - autospazi|autovettore]] di $\varphi$ allora $A^{\perp}$ è $\varphi$-invariante.
# Proposizione
Sia $\varphi:V_n(\mathbb{C})\to V_{n}(\mathbb{C})$ [[Trasformazione lineare|funzione lineare]].
Se tutti gli autovalori di $\varphi$ sono reali e $V_{n}(\mathbb{C})$ ammette una [[Base ortogonale e ortonormale|base ortonormale]] di [[Autovettori - autovalori - autospazi|autovettori]], allora $\varphi$ è hermitiana.
# Definizione | funzione antisimmetrica
Sia $\varphi:V_n(\mathbb{R})\to V_{n}(\mathbb{R})$ [[Trasformazione lineare|funzione lineare]].
$\varphi$ è antisimmetrica se e solo se $<\varphi(x),y>=-<x,\varphi(y)>\quad \forall x,y\in V_{n}(\mathbb{R})$
### Definizione matrici | Matrice antihermitiana
$M$ è antisimmetrica $\iff M = -M^{T}$, cioè $\begin{cases}a_{ij}=-a_{ij},i\not=j\\a_{ii}=0\end{cases}$
# Definizione | funzione antihermitiana
Sia $\varphi:V_n(\mathbb{C})\to V_{n}(\mathbb{C})$ [[Trasformazione lineare|funzione lineare]].
$\varphi$ è antisimmetrica se e solo se $<\varphi(x),y>=-<x,\varphi(y)>\quad \forall x,y\in V_{n}(\mathbb{C})$
### Definizione matrici | Matrice antihermitiana
$M$ è antihermitiana $\iff M = -M^{-T}$, cioè $\begin{cases}a_{ij}=-\bar{a_{ij}},i\not=j\\a_{ii}=\bar{a_{ii}}\end{cases}$

# Teorema | autovalori funzione hermitiana
Sia $\varphi:\mathbb{C}\to\mathbb{C}$ una trasformazione antihermitiana.
Allora i suoi [[Autovettori - autovalori - autospazi|autovalori]] sono numeri immaginari puri oppure nulli.
#dimostrazione-da-fare 