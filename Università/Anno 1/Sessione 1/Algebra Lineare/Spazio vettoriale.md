---
aliases:
  - spazio vettoriale
  - Spazio lineare
  - spazio lineare
pagina: 27
---
# Definizione
Sia $V$ un insieme non vuoto e $0\in V$ e sia $\mathbb{K}$ un [[Campo]] fissato. Gli elementi di $\mathbb{K}$ vengono detti scalari.
Siano
- $+:V\times V\to V$ la somma vettoriale
- $\cdot:\mathbb{K}\times V\to V$ il prodotto per scalari
tali che vengano verificate
1) La proprietà associativa
	   $x+(y+z)=(x+y)+z,\quad \forall x,y,z\in\mathbb{V}$
2) La proprietà commutativa
	   $x+y=y+x\quad \forall x,y\in\mathbb{V}$
3) Lo $0$ sia l'elemento neutro rispetto alla somma vettoriale
	   $o+x=x+0=x\quad \forall x\in V$
4) Esista opposto
	   $\forall x\in V,\ \exists!y\in V:x+y=0=y+x$
5) Le proprietà distributive$$\begin{split}
	   &1)\ (a+b)\cdot x=a\cdot x+b\cdot x\quad \forall x\in V,\forall a,b\in\mathbb{K}\\
	   &2)\ a\cdot(x+y)=a\cdot x+a\cdot y\quad \forall x,y\in V,\forall a\in \mathbb{K}\\
	   &3)\ a\cdot(b\cdot x)=a\cdot b\cdot x\quad \forall x\in V,\forall a,b\in \mathbb{K} 
	   \end{split}$$
6) L'$1$ sia l'elemento neutro rispetto la prodotto per scalari
	   $1\cdot x=x\quad \forall x\in V$


Allora $V$ è detto spazio vettoriale su $\mathbb{K}$
- Gli elementi di $V$ si dicono vettori.
- $0$ è detto vettore nullo.
N.B. (Non c'è inverso in uno spazio vettoriale)

# Proprietà
1) $x+y=z\iff x=z-y\quad \forall x,y,z\in V$
2) $x-y=0\iff x=y\quad \forall x,y\in V$
3) $x+y=0\iff y=-x\quad \forall x,y\in V$
4) $x+x=0\iff x=0$
5) $x+y=x+z\iff y=z\quad \forall x,y,z\in V$
6) $-(-x)=x\quad \forall x\in V$
7) $-(x+y)=(-x)+(-y)\quad \forall x,y\in V$
8) $-0=0$
9) $0\cdot x=0$
10) $a\cdot 0=0\quad\forall a\in \mathbb{K}$
11) $-a\cdot x=(-a)\cdot x=a\cdot (-x)\quad \forall x\in V,\forall a\in \mathbb{K}$
12) $a\cdot x=(-a)\cdot(-x)\quad \forall x\in V,\forall a\in \mathbb{K}$
13) $-x=(-1)\cdot x\quad \forall x\in V$
14) $a^{-1}\cdot(a\cdot x)=x\quad \forall x\in V,\forall a\in \mathbb{K}\setminus\{0\}$
15) $a\cdot x=y\iff x=a^{-1}\cdot y\quad \forall x,y \in V,\forall a\in \mathbb{K}$
16) $a\cdot x=0\iff (a=0)\lor (x=0)$
17) $a\cdot x=a\cdot y \iff x=y$
18) $a\cdot x=b\cdot x\iff a=b$

# Esempi
- $P_n(\mathbb{K})$, ovvero l'insieme dei polinomi a coefficienti in $\mathbb{K}$ è uno [[Spazio vettoriale|spazio vettoriale]] su $\mathbb{K}$.
- $E_{n}(\mathbb{K})$, ovvero l'insieme delle equazioni lineari in $n$ variabili a coefficienti in $\mathbb{K}$ è uno spazio vettoriale su $\mathbb{K}$.
- $EO_{n}(\mathbb{K})$, ovvero l'insieme delle equazioni lineari omogenee in $n$ variabili a coefficienti in $\mathbb{K}$ è uno spazio vettoriale su $\mathbb{K}$
N.B. $V_{1}(\mathbb{K})=\mathbb{K}$ Ogni campo può essere visto come spazio vettoriale su se stesso 
