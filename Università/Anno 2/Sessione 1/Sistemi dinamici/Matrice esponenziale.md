---
collegamenti:
  - "[[Numero di Nepero]]"
---
 Con $A\in \mathbb{R}^{n\times n}$
$$e^{At}:=\sum_{k=0}^{+\infty}\frac{A^{k}t^{k}}{k!}=I+At+A^{2}\frac{t^2}{2}+\ldots+A^{k}\frac{t^{k}}{k!}+\ldots$$
## Proprietà
1) $e^{A\cdot 0}=I$ 
2) $e^{(A+B)t}\not = e^{At}\cdot e^{Bt}$, è vero solo se $AB=BA$ 
3) $[e^{At}]^{-1}=e^{-At}$
4) $\frac{d}{dt}e^{At}=Ae^{At}$
5) Siano $v\in \mathbb{C}^{n},\lambda \in \mathbb{C}:Av=\lambda v\Rightarrow e^{At}\cdot v=e^{\lambda t}\cdot v$
   - La matrice esponenziale ha gli stessi [[Autovettori - autovalori - autospazi|autovettori]] di $A$
   - La matrice esponenziale ha come [[Autovettori - autovalori - autospazi|autovalori]] $e^{\lambda_{i}t}$ dove $\lambda_{i}$ sono gli autovalori di $A$
6) 