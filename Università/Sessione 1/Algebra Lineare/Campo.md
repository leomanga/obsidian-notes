---
pagina: 1
---
# Definizione
Sia $\mathbb{K}$ un insieme non vuoto
$(\mathbb{K},+,\cdot)$ è un campo se e solo se valgono le seguenti proprietà
$0,1 \in \mathbb{K}$
1) Proprietà commutativa
	$\forall x,y\in \mathbb{K}\quad x+y = y+x$
	$\forall x,y\in \mathbb{K}\quad x\cdot y = y\cdot x$
2) Proprietà associativa
	$\forall x,y,z\in \mathbb{K}\quad x+(y+z) = (x+y)+z$
	$\forall x,y,z\in \mathbb{K}\quad x\cdot(y\cdot z) = (x\cdot y)\cdot z$
3) Proprietà distributiva
	$\forall x,y,z\in \mathbb{K}\quad x\cdot(y+z) = x\cdot y+x\cdot z$
4) 0 elemento neutro rispetto alla somma
	$\forall x\in \mathbb{K}\quad x+0 = x = 0+x$
5) 1 elemento neutro rispetto al prodotto
	$\forall x\in \mathbb{K}\quad x\cdot 1 = x = 1\cdot x$
6) Esistenza di un opposto di $x$
	$\forall x\in\mathbb{K}\quad \exists y \in \mathbb{K}$ tale che $x+y = 0 = y+x$
7) Esistenza di un inverso o reciproco di $x$
		$\forall x\in\mathbb{K}\setminus\{0\}\quad \exists y \in \mathbb{K}$ tale che $x\cdot y = 1 = y\cdot x$
# Esempi
Sono campi $\mathbb{Q}, \mathbb{R}\ e\ \{0,1\}$

# Caratteristica
Dato un campo $\mathbb{K}$ si definisce "caratteristica di $\mathbb{K}$" come il più piccolo numero naturale $n>1$ tale che $\underbrace{1+1+\ldots+1}_{n\ volte}=0$
Se non esiste, si dice che il campo ha caratteristica $0$.($\mathbb{Q},\mathbb{R}$)
L'esempio $\{0,1\}$ è il più piccolo campo con caratteristica $2$.

# Proprietà
1) Legge di cancellazione
	$a+b=a+c\imp b=c$
2) Unicità degli opposti, ovvero, dato $a\in \mathbb{K}$, l'opposto di $a$ è unico.
3) Dati $a,b\in\mathbb{K}:\exists! x:a+x=b$
4) $-(-a)=a$
5) $a\cdot 0 = 0$
6) $a\cdot b = a\cdot c$ con $a\not = 0\imp b=c$
7) L'inverso di $a\in \mathbb{K}\setminus\{0\}$ è unico
8) Dato $a$ e $b$ con $a\not = 0\quad \exists! x:a\cdot x=b$
9) Legge dell'annullamento del prodotto
	$a\cdot b = 0\iff (a=0)\lor (b=0)$