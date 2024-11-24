---
capitolo: 6
collegamenti: "[[Serie numeriche a termini di segno costante]]"
---
### Limite finito
Data una successione di numeri reali, il limite per n tendente all'infinito è $\ell\in \mathbb{R}$
se
$$\forall \epsilon > 0 \ \ \exists\nu_{\epsilon}\in \mathbb{N} : \forall n > \nu_{\epsilon}\ \ |a_{n} - \ell| <\epsilon$$
(Per ogni $\epsilon$ > 0, $|a_{n}-l| < \epsilon$ definitivamente in $n$)

### Limite = Sup per serie convergenti a termini positivi
Abbiamo una serie convergente a $s \in [0,+\infty]$ e la successione delle sue somme parziali.
$$s = \lim_{n\to+\infty}s_n$$
Dall' estremo superiore dell'insieme
$$s(\mathbb{N}) = \{s_n:n\in\mathbb{N}\}$$
I due sono uguali.

### Unicità del limite
Basta risolvere ([[#Limite finito]]) e trovare $\nu_\epsilon$.
Se esiste il limite, quindi, è unico.

![[Teorema dei carabinieri#Teorema dei carabinieri]]

### Operazioni algebriche e limiti finiti

1) Limite della somma = somma limiti
2) Limite differenza = differenza limiti
3) Il limite del prodotto è il prodotto dei limiti
4) Il valore assoluto del limite è il limite dei valori assoluti

#dimostrazione-da-fare 
### Successione limitata dall'alto e dal basso
Una successione si dice 
- ##### limitata dall'alto 
	Se esiste un numero reale M tale che valga
	$$a_{n}< M\ \ \forall n \in \mathbb{N}$$
- ##### limitata dal basso 
	Se esiste un numero reale M tale che valga
	$$a_{n}> M\ \ \forall n \in \mathbb{N}$$
### Successione limitata
Una successione è limitata se esiste un numero positivo M tale che
$$|a_{n}|< M\ \ \forall n \in \mathbb{N}$$

### Le successioni convergenti sono limitate
Dimostrazione:
#dimostrazione-da-fare

### Una successione definitivamente limitata è limitata

### Il limite di una successione limitata moltiplicata ad una convergente a zero fa zero
#dimostrazione-da-fare 

### Il limite finito e l'ordinamento dei numeri reali

Se $$a_{n}\le b_{n}\ \ \forall n \in \mathbb{N}$$
allora
$$\lim_{n\to +\infty} a_{n}\le \lim_{n\to +\infty} b_{n}$$

*** Importante è il minore uguale
#dimostrazione-da-fare 

### Osservazione 6.2.3
Se $a_n$ è una successione di numeri reale convergente e vale
$$s\le a_{n}\le t \ \ \forall n \in \mathbb{N}$$
allora
$$s\le \lim_{n\to +\infty}a_{n}\le t \ \ \forall n \in \mathbb{N}$$
### Permanenza del segno per le successioni
Abbiamo una successione $a_n$ convergente a $\ell > 0$. Allora
$$\exists \nu \in \mathbb{N} : a_{n}>0 \ \ \forall n > \nu$$
_Se il limite di una successione convergente è positivo, i termini della successione sono positivi definitivamente in n_
#dimostrazione-da-fare 

### Carattere definitivo del limite
Se $a_n$ e $b_n$ sono due successioni di numeri reali e se esiste indice $\nu \in \mathbb{N}$ tale che $$a_{n}= b_{n}\ \ \forall n > \nu$$
allora la successione $a_n$ converge solo se converge la successione $b_n$ ed in tal caso hanno lo stesso limite
[[Es 6.2.6 e 6.2.8]]

# Successioni monotone limitate
[[Serie numeriche a termini di segno costante#Successione monotona]]
[[Successioni e limiti finiti#Successione limitata]]
### Teorema fondamentale delle successioni monotone

Se $a_n$ è limitata non decrescente allora $\exists \lim a_{n}= sup\ a(\mathbb{N}) \in \mathbb{R}$
Se $a_n$ è limitata non crescente allora $\exists \lim a_{n}= inf\ a(\mathbb{N}) \in \mathbb{R}$

#dimostrazione-da-fare 

# Ancora sul numero $e$
![[Numero di Nepero#Numero di Nepero-2]]
6.4

### Stima dall'alto e dal basso sul fattoriale

![[Stima fattoriale#2]]

### Teorema del contrario
Se $a_{n}> 0$ e se $\sum_{n=1}^{+\infty}a_{n}<+\infty$
Allora
$$\lim_{n\to+\infty}a_{n}= 0$$
### La coda di una serie convergente è infinitesima
Sia $\sum_{n\ge 1}a_n$ una serie a termini positivi, convergente, allora
$$\lim_{N\to +\infty}\sum_{n=N+1}^{+\infty} a_n = 0$$
#dimostrazione-da-fare 

### Limiti notevoli
![[Limiti notevoli#6.4.9]]
![[Limiti notevoli#6.4.10]]
# Criteri di convergenza
Simile a 
[[Serie numeriche a termini di segno costante#Criteri di convergenza]]
Con c < 1.
##### Rapporto
Se
$$\frac{a_{h+1}}{a_{h}}\le c\ \ \forall h > n$$
allora
$$\lim_{h\to \infty}a_{h}= 0$$
#dimostrazione-da-fare 

#### Radice
Se
$$\sqrt[h]{a_{h}}\le c\ \ \ \forall h > n$$
allora
$$\lim_{h\to \infty}{a_{h}}= 0$$
#dimostrazione-da-fare 

# Sottosuccessioni

### Sottosuccessione estratta
Diremo che una successione $b_n$ è estratta da una successione $a_n$ se esiste una successione crescente $i_n$ di interi positivi che valga
$$b_{n}= a_{i_{n}}\ \ \ \ \ \forall n \in \mathbb{N}$$
In poche parole possiamo scrivere 
$$b = a \circ i$$
###### Esempio
Un esempio è la successione $b_n$ costante uguale a 1, cioè $b_{n}= 1 \ \ \ \forall n \in \mathbb{N}, è estratta dalla successione a_{n}= (-1)^n$ prendendo
$$i_{n}= 2n$$
per avere 
$$b_{n}= (-1)^{2n} = 1$$
### Teorema 6.6.3
Se $a_n$ è una successione convergente ad $\ell$, allora ogni successione $b_n$ estratta da $a_n$ è convergente e vale $\ell$.
#dimostrazione-da-fare 

### Teorema di Bolzano-Weierstrass
Da ogni successione [[Successioni e limiti finiti#Successione limitata|limitata]] si possono estrarre sottosuccessioni convergenti.
###### Esempi
$(-1)^n$ è limitata ma non convergente e si possono estrarre le successioni costanti uguali a 1 e -1.

###### Esercizio 6.6.8
Secondo me con m=n, tende a 0, sennò tende ad 1

