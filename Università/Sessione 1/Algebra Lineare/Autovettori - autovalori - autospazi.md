---
pagina: 265
aliases:
  - autovalore
  - autovettore
  - autospazio
---
# Definizione | Autovettore
Sia $\varphi:V\to V$ [[Trasformazione lineare#Endomorfismo]].
Sia $A\in V, A\not  = 0$.
$A$ è un autovettore di $\varphi$ se e solo se $L(A)$ è [[f-invariante e fissato da f|f-invariante]].
# Definizione | Autovalore
Se $A$ autovettore, 
$\varphi(L(A))=L(\varphi(A))\subseteq L(A)\iff \varphi(A)\in L(A)$ 
$$\iff\varphi(A)=\lambda\cdot A$$
con $\lambda$ opportuno scalare. 
$\lambda$ è definito come autovalore, è univocamente determinato.

# Proposizione 1
$\varphi:V\to V$ [[Trasformazione lineare#Endomorfismo]]
$A\in V,A\not = 0$
A è un autovettore di autovalore $\lambda$ di $\varphi$ se e solo se $\varphi(A)=\lambda A$.

# Base di autovettori di f
$\varphi:V\to V$ [[Trasformazione lineare#Endomorfismo]], [[Dimensione|dim]]$(V)=n$.
Sia $\mathbb{E}=(E_1,E_2,\ldots,E_n)$ [[Base]] di $V$.
Supponiamo che $E_1,E_2,\ldots,E_n$ siano autovettori di $\varphi$, cioè
$\varphi(E_{1})=\lambda_{1}E_{1}$
$\varphi(E_{2})=\lambda_{2}E_{2}$
$\ldots$
$\varphi(E_{n})=\lambda_{n}E_{n}$

$$\mu_\mathbb{E}(\varphi)=\left(\begin{split}
&\lambda_{1}\ 0\ \ldots\ 0\\
&0\ \lambda_{2}\ \ldots \ 0\\
&\ldots\\
&0\ 0\ \ldots \ \lambda_{n}
\end{split}\right)$$
$\mu_{\mathbb{E}}(\varphi)$ è una matrice diagonale
Allora $\varphi\in \ell(V)$ è diagonalizzabile $\iff \mu_{\mathbb{E}}$ è [[Proprietà e definizioni matrici#Definizione Matrice diagonalizzabile|diagonalizzabile]] per una opportuna base $\mathbb{E}$ di V $\iff \mu_B(\varphi)$ è diagonale per una opportuna base $B$ di $V$.
$$\iff V\mbox{ ammette una base di AUTOVETTORI di }\varphi$$
# Proposizione 2
$\varphi\in \mathcal{L}(V)$
$\lambda$ è un autovalore di $\varphi$
$$\begin{split}
&\iff \exists A \not = 0 \mbox{ autovettore di }\varphi \mbox{ avente } \lambda \mbox{ come autovalore}\\
&\iff\exists A \in V,A\not = 0\mbox{ tale che }\varphi(A)=\lambda A\\
&\iff(\varphi-\lambda I)\mbox{ non è iniettiva(I sta per immagine)}\\
&\iff rank(\varphi-\lambda I)< n\\
&\iff ker(\varphi-\lambda I)\not = 0\\
&\iff det(\underbrace{M}_{rappresenta\ \varphi}-\lambda I) = 0
\end{split}$$
# Definizione | Autospazio
Dato $\varphi\in \mathcal{L}(V)$ e dato $\lambda$ autovalore di $\varphi$.
Si dice autospazio di $\lambda$, il [[Kernel di una funzione lineare|nucleo]] $\varphi-\lambda I$
$$A(\lambda)=ker(\varphi-\lambda I)=(\varphi-\lambda I)^{-1}(0)$$
### Molteplicità geometrica di $\lambda$
Si indica con $mg(\lambda):=dim(A(\lambda))=dim(ker(\varphi-\lambda I))$

### Molteplicità algebrica
Si indica con $ma(\lambda):=$ numero di volte in cui $\lambda$ compare come autovalore di $\varphi$.

# Esempi
- [[Omotetia di ragione a#Autovalori]]
- [[Proiezione di A lungo B]]