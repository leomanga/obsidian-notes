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
6) Sia $T\in \mathbb{R}^{n\times n}$ con $\det (T)\not = 0$ 
   Se $A=T\bar{A}T^{-1}\Rightarrow e^{At}=Te^{\bar{A}t}T^{-1}$.
   Se $\exists v_{1}, v_{2},\ldots ,v_{n}$ [[Autovettori - autovalori - autospazi|autovettori]] linearmente indipendenti, allora $T=[v_{1}\ v_{2}\ \ldots v_{n}]$ è invertibile
   Allora vale sempre il caso 5, $Av_{i}=\lambda_{i}v_{i}$ per qualche $\lambda_{i}$
   - Se $A$ è [[Proprietà e definizioni matrici#Definizione Matrice diagonalizzabile|diagonalizzabile]], allora $$\exists T:A=T\Lambda T^{-1}$$
     con $\Lambda=\begin{bmatrix}\lambda_{1} & 0& \ldots &0\\ 0& \lambda_{2}& \ddots &\vdots\\ \vdots &\ddots& \ddots& 0\\ 0 &\ldots& 0&\lambda_{n}\end{bmatrix}$ la matrice diagonale
     Allora $AT=T\Lambda$ , allora $e^{At}=Te^{\Lambda t}T^{-1}$ ed avremo che
     $$e^{At}=Te^{\bar At}T^{-1}=T\cdot\begin{bmatrix}e^{\lambda_{1}} & 0& \ldots &0\\ 0& e^{\lambda_{2}}& \ddots &\vdots\\ \vdots &\ddots& \ddots& 0\\ 0 &\ldots& 0&e^{\lambda_{n}}\end{bmatrix}\cdot T^{-1}$$
    - Se $A$ non è diagonalizzabile, allora
      $$\exists T, \det(T)\not=0:A=TJT^{-1}$$
      dove $J$ è la [[Matrice di Jordan o Forma di Jordan|forma di Jordan]].
      Allora avremo che $e^{At} = Te^{Jt}T^{-1}$, dove $$e^{Jt}=\begin{bmatrix}e^{J_{1}t}&0&\ldots&0\\0&e^{J_{2}t}&\ddots&\vdots\\\vdots&\ddots&\ddots&0\\0&\ldots&0&e^{J_{r}t}\end{bmatrix}$$
      $$e^{J_{i}t}=\begin{bmatrix}e^{\lambda_{i}t}&te^{\lambda_{i}t}&\ldots&\ldots&e^{\lambda_{i}t}\frac{t^{m_{i}-1}}{(m_{i}-1)!}\\0& e^{\lambda_{i}t}&te^{\lambda_{i}t}& & \vdots\\0&0&\ddots&\ddots& \vdots\\\vdots& & \ddots&\ddots&te^{\lambda_{i}t}\\0&\ldots&\ldots&0&e^{\lambda_{i}t}\end{bmatrix}\in \mathbb{R}^{m_{i}\times m_{i}}$$
      