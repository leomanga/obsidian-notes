---
pagina: 11
collegamenti:
  - "[[Campo]]"
---
Non ci è possibile trovare soluzione reale dell'equazione $x^{2}+1 = 0$
Definiamo con il simbolo $i\not \in \mathbb{R}$ la soluzione, cioè $i^{2}=-1$
Lo scopo è quello di costruire un campo tale che $\mathbb{R}$ sia contenuto in esso come sottocampo, che contenga $i$ e sia il più piccolo possibile.
Tale campo lo indichiamo con $<\mathbb{R},i>$
Indichiamo con $+$ e $\cdot$ le equazioni di somma e prodotto nel campo appena definito.
$$<\mathbb{R},i>=\mathbb{R}\cup\{i\}\cup\{-i\}\cup\{a+i:a\in \mathbb{R}\}\cup\{\underbrace{i^{-1}}_{=-i}\}, b\cdot i, \underbrace{i^{2}}_{=-1},\underbrace{i^{3}}_{=-i},\underbrace{i^4}_{=1},(a+bi)^{-1},(a+bi),\ldots\}$$
Dato che tutte le potenze di $i$ danno come risultato $\pm 1,\pm i$ possiamo riassumere il campo così:
$<\mathbb{R},i>=\{x+yi:x,y\in\mathbb{R}\}$

Definiamo ora
- Elemento neutro rispetto alla somma
	$0: 0+0i$
- Elemento neutro rispetto al prodotto
	$1: 1+0i$
- Somma
	$(x+yi)+(x^{'}+y^{'}i):= (x+x^{'})+(y+y^{'})i\quad \forall x,x^{'},y,y^{'}\in \mathbb{R}$
- Prodotto
	$(x+yi)\cdot(x^{'}+y^{'}i):=(xx^{'}-yy^{'})+(xy^{'}+x^{'}y)i\quad \forall x,x^{'},y,y^{'}\in \mathbb{R}$
- Opposto
	$-(x+yi):= -x-yi$
- Inverso
	$(x+yi)^{-1}:=\frac{x}{x^2+y^2}-\frac{y}{x^2+y^2}i$

# Definizioni
$z\in \mathbb{X}\quad z= \underbrace{x}_{parte\ reale}+\underbrace{y}_{parte\ immaginaria}i$
Se $x=0$ allora $z=yi$ e viene chiamato numero immaginario puro.

- Coniugato
Se $z=x+yi\in \mathbb{C}$ allora $\bar z=x-yi\in\mathbb{C}$ e viene detto coniugato di $z$. ^b34f54

# Definizione | Funzione di coniugio
$\sigma: \mathbb{C}\to\mathbb{C}$
$\sigma(z)=\bar z$
Questa funzione è detta funzione di coniugio ed è invertibile.
- $\sigma(0)=0$
- $\sigma(1)=1$
- $\sigma(z_{1}+z_{2})=\sigma(z_{1})+\sigma(z_{2}),\quad \forall z_{1},z_{2}\in\mathbb{C}$
- $\sigma(z_{1}\cdot z_{2})=\sigma(z_{1})\cdot \sigma(z_{2}),\quad \forall z_{1},z_{2}\in\mathbb{C}s$
- $\sigma(-z)=-\sigma(z)$
- $z\not = 0\quad \sigma(z^{-1}) = (\sigma(z))^{-1}\quad \forall z\in \mathbb{C}\setminus \{0\}$
La funzione di coniugio è un [[Automorfismo]] di $\mathbb{C}$

# Proprietà
La parte reale di $z = \frac{z+\bar z}{2}$
La parte immaginaria di $z=\frac{z-\bar z}{2i}$
- $z\cdot \bar z = a^{2}\cdot b^{2}\in \mathbb{R}$
- $|z|:=\sqrt{z\cdot \bar z}$
- $|z_{1}+z_{2}|\le |z_{1}|+|z_{2}|$
- $|z_{1}\cdot z_2| =|z_{1}|\cdot |z_{2}|\quad \forall z_1,z_{2}\in\mathbb{C}$

- In $\mathbb{C}$ non è definito un ordinamento
	$0<i$ ma $0>i^{2}$ oppure $i<0$, ma $-1 < 0$
Possiamo comunque lavorare con il modulo perchè appartiene ai numeri reali.

# Numeri complessi nel grafico
Ad un numero complesso possiamo associare un vettore $(a,b)\in \mathbb{R}^{2}$, che rappresenta le coordinate nel grafico.
$f(a+bi)=(a,b)$.
$|z|$ indica la distanza di $z$ dall'origine del sistema di riferimento. Rappresenta cioè la lunghezza del vettore nel grafico.

# Altri modi per rappresentare i complessi
### Coordinate polari
Possiamo prenderci $\rho = |z|\in \mathbb{R}^{+}$, dove $z$ è un qualsiasi numero complesso.
Prendiamo inoltre $\theta$, l'angolo formato dall'asse delle ascisse e la semiretta $L_{z}$, che parte dall'origine e contiene $z$.
$(\rho,\theta)$ sono dette coordinate polari di $z$
- $\rho$ viene chiamato modulo
- $\theta$ viene chiamata fase o argomento

$(\rho_1,\theta_{1})=(\rho_2,\theta_{2})$ se e solo se $\begin{cases}\rho_{1} = \rho_{2}\\\theta_{1}-\theta_{2}=2k\pi\ k\in\mathbb{Z} \end{cases}$ 

### Rappresentazione trigonometrica
Sapendo $\rho$ e $\theta$ possiamo sapere la parte immaginaria e reale del nostro numero.
$\rho = \sqrt{a^{2}+b^{2}}$
$a=\rho\cdot cos\theta$
$b=\rho\cdot sin\theta$
$z = \rho(cos\theta+sin\theta\cdot i)$

##### Operazioni
$z_{1}=\rho(\cos\theta+i\sin\theta), z_{2}=\mu(\cos\varphi+i\sin\varphi)$
$z_{1}\cdot z_{2}=\rho\mu(\cos(\theta+\varphi)+i\sin(\theta+\varphi))$
### Rappresentazione algebrica
La rappresentazione algebrica è il metodo usato fino ad ora
$z=a+b\cdot i$
### Rappresentazione esponenziale
Ogni numero complesso $z\not = 0$ può essere scritto come 
$$z=\underbrace{e^{t}}_{modulo}\cdot e^{i\underbrace{\theta}_{argomento}}$$
$$e^{t+i\theta}:=e^{t}(\cos\theta+i\sin\theta)$$
# Formula di De Moivre
Se $z=\rho(\cos\theta+i\sin\theta)$
Allora $z^{n}=\rho^{n}(\cos n\theta+i\sin n\theta)$ 

### Significato geometrico potenze
Le potenze si distribuiscono su vertici di un poligono regolare di centro $0$ avente $\frac{2\pi}{\theta}$ lati.

# Proprietà potenze
L'equazione $x^{n}=a, \quad x,a\in\mathbb{C}$, ammette $n$ soluzioni distinte.

# Proprietà dell’argomento o fase
$$
\measuredangle a\cdot b=\measuredangle a+\measuredangle b
$$

^fa4be1

