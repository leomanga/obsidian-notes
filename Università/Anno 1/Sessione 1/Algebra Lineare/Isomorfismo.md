---
pagina: 129
---
# Definizione | isomorfismo per campi
[[Campo]]
Siano $(\mathbb{K},+,\cdot,-,-1,0,1)\ e\ (\mathbb{K}^{'},+^{'},\cdot^{'},-^{'},-1^{'},0^{'},1^{'})$
Se esiste una funzione $f:\mathbb{K}\to\mathbb{K}^{'}$ iniettiva e suriettiva tale che valgano le seguenti proprietà
1) $f(0)=0^{'}$
2) $f(1)=1^{'}$
3) $f(x+y)=f(x)+^{'}f(y)\quad \forall x,y\in \mathbb{K}$
4) $f(x\cdot y)=f(x)\cdot^{'}f(y)\quad \forall x,y\in \mathbb{K}$
5) $f(-x)=-^{'}f(x)\quad \forall x \in \mathbb{K}$
6) $f(x^{-1})=(f(x))^{-1}\quad \forall x\in \mathbb{K}\setminus \{0\}$

Allora i due campi si dicono ISOMORFI e si scrive $\mathbb{K}\cong \mathbb{K}^{'}$ ed $f$ si dice ISOMORFISMO.

# Definizione | isomorfismo per spazi vettoriali
Siano $V$ e $W$ due [[Spazio vettoriale|spazi vettoriali]] definiti sullo stesso campo
$V=(V,+_{v},-v,\cdot_{v},0_{v})\quad W=(W,+_{w},-w,\cdot_{w},0_{w})$
$V$ e $W$ sono isomorfi($V\sim W$) se esiste una funzione invertibile $f:V\to W$ tale che:
1) $f(0_{v})=0_{w}$
2) $f(v_{1}+_{v}v_{2})=f(v_{1})+_{w}f(v_{2})$
3) $f(-_{v}v)=-_{w}f(v)$
4) $f(\lambda \cdot_{v}v)=\lambda \cdot_{w}f(v)$
La funzione con queste proprietà si dice isomorfismo
# Lemma 1
Sia $V$ uno [[Spazio vettoriale]] di [[Dimensione]] $n$ sul [[Campo]] $\mathbb{K}$.
Sia $\mathbb{E} = (E_1,E_2,\ldots,E_n)$ base ordinata di $V$.
Sia $\rho : V \to V_n(\mathbb{K})$  
$\rho(x)=(x)_\mathbb{E}$

Allora $\rho$ è un isomorfismo da $V$ a $V_n(\mathbb{K})$ ($V\cong V_n(\mathbb{K}$) 
#dimostrazione-da-fare 

# Lemma 2
Sia $V$ spazio vettoriale su $\mathbb{K}$
Sia $\mathbb{E} = (E_i)_{i\in I}$ base ordinata di $V$.
$V_I(\mathbb{K}) = \{f:I \to \mathbb{K}\}$ spazio vettoriale delle funzioni da $I$ a $\mathbb{K}$.
$$\forall x \in V, \ x = \sum_{i\in I}x_iE_{i\qquad}(x)_\mathbb{E} = (x_i)_{i\in I}$$
$(x_i)_{i\in I}\mbox{ coordinate di x rispetto ad } \mathbb{E}$

# Proposizione 
Sia $V$ spazio vettoriale su $\mathbb{K}$
Sia $\mathbb{E}$ base ordinata fissata di $V$.
$$f:V\to V_I(\mathbb{K})\mbox{ è un isomorfismo}$$
# Primo teorema di isomorfismo
$V \cong V_I(\mathbb{K})$ con $dim(V) = card(I)$
- caso particolare: Se $dim(V) = n$ allora $V \cong Vn{\mathbb{K}}$

# Lemma 3
Siano $V$ e $W$ spazi vettoriali definiti nello stesso campo $\mathbb{K}$.
$$dim(V) = dim(W) \Rightarrow V \cong W$$
#dimostrazione-da-fare 

# Lemma 4
[[Dipendenza lineare]]
Siano $V \cong W$ e $\alpha: V \to W$ isomorfismo.
Allora:
1) $\alpha(L(\mathbb{X})) = L(\alpha(\mathbb{X}))\ \ \forall x \subset V$
2) $$\left(\begin{split} 
   &\mathbb{X} \subset V\\ 
   &\mbox{lin indip} 
   \end{split}\right)\Rightarrow \left(\begin{split}
   &\alpha(\mathbb{X}) \subseteq W\\ 
   &\mbox{è lin indip}
   \end{split}\right)$$
#dimostrazione-da-fare 
### Casi particolari
1) Sia $\alpha : V \to W$ isomorfismo
	$L(\mathbb{X}) = V \to L(\alpha(\mathbb{X})) = W$
2) Sia $\alpha : V \to W$ isomorfismo
	$\mathbb{X}$ base di $V \Rightarrow \alpha(\mathbb{X})$ base di $W$.

# Secondo teorema di isomorfismo
Siano $V$ e $W$ [[Spazio vettoriale|spazi vettoriali]] definiti sullo stesso campo
$$V \cong W \iff dim(V) = dim(W)$$
#dimostrazione-da-fare 