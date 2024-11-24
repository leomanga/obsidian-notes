---
capitolo: 5
collegamenti: "[[Estremo superiore e inferiore]]"
---
---
### Successione
Una successione di numeri reali è una funzione $f:\mathbb{N}\rightarrow\mathbb{R}$
Si indica $f_{n}$ al posto di $f(n)$

### Successione monotona
Una successione è detta *monotona* quando è **strettamente crescente** o **strettamente decrescente**, o **non decrescente** o **non crescente**.

### Serie numeriche a termini positivi
Accanto ad una successione di numeri reali
$$a_{1}, a_2,\ldots,a_n $$
possiamo considerare la successione
$$s_1:=a_1, \ s_2:=a_1+a_2, \ s_n:=a_1+a_2+\ldots+a_n$$
$$s_n=\sum_{n}^{i=1}{a_i}$$
### Successione delle somme parziali
$$\sum_{i=1}^{+\infty}{a_i}$$
Studiamo il caso in cui $a_i\ge0$
Quindi, dato che $a_{i}\ge0\ \forall i\in\mathbb{N}$, la successione è [[Serie numeriche a termini di segno costante#Successione monotona|monotona]] non decrescente se gli $a_i\ge0$ e strettamente crescente se gli $a_i>0$.

### Somma di una quantità numerabile di addendi
Sia $a_i$ una successione di numeri reali non negativi, l'[[Estremo superiore e inferiore|estremo superiore]] dell'insieme       {$s_n:n\in\mathbb{N}$} si indica con il simbolo $\sum_{i=1}^{+\infty}a_i$, cioè:
$$\begin{equation}
\begin{split}
\sum_{i=1}^{+\infty}a_{i}:&=sup\{s_n:n\in\mathbb{N}\}\\
&=sup\{\sum_{i=1}^{n}a_{i}:n\in\mathbb{N}\}
\end{split}
\end{equation}
$$
Se $\{s_{n}:n\in\mathbb{N}\}$ non è [[Estremo superiore e inferiore#Insieme superiormente e inferiormente limitato|superiormente limitato]], allora
$$\sum_{i=1}^{+\infty}a_i=+\infty,$$
e diremo che la serie è **divergente**.
Nel caso contrario,
$$\sum_{i=1}^{+\infty}a_{i} = s\ oppure\ \sum_{i=1}^{+\infty}a_i<+\infty$$
### Studio del carattere di una serie
Non sempre è possibile calcolare esplicitamente $s$, quindi ci si limita a capire il carattere della serie, ovvero se converge o diverge.
##### Carattere definitivo
Il carattere di una serie non è alterato se vengono modificati un numero finito di addendi.
Siano $\sum_{n=1}^{+\infty}a_n$[^1], $\sum_{n=1}^{+\infty}b_n$[^2] due serie e sia $\nu\in\mathbb{N}$ tale che
$$a_n=b_n\ \ \ \ \ \ \forall n>\nu$$
Allora se la serie [^1] è convergente, anche [^1] lo sarà, e se la serie [^1] è divergente, anche [^2] lo sarà.

![[Serie geometrica di ragione tra 0 e 1#Serie geometrica di ragione tra 0 e 1]]

![[Serie di Mengoli#Serie di mengoli]]
### Omogeneità
Con c>0
$$\sum_{k=1}^{+\infty}ca = c\sum_{k=1}^{+\infty}a$$
### Linearità
$$\sum_{k=1}^{+\infty}{(a_n+b_{n)}}= \sum_{k=1}^{+\infty}a_n+\sum_{k=1}^{+\infty}b_n$$
### Confronto
Suppongo 
- Se
$(i) \sum_{n=0}^{+\infty}b_n <+\infty$
$(ii) a_n \le b_n\ \forall n \in \mathbb{N}$
Allora 
$\sum_{n=0}^{+\infty}a_n \le \sum_{n=0}^{+\infty} b_n$

- Se
$(i) \sum_{n=0}^{+\infty}b_n =+\infty$
$(ii) a_n \ge b_n\ \forall n \in \mathbb{N}$
Allora
$\sum_{n=0}^{+\infty}a_n \ge \sum_{n=0}^{+\infty} b_n$

### Definitivamente e frequentemente
Se una proprietà è vera definitivamente, è vera frequentemente, ma non il contrario.
##### Definitivamente
Una proprietà P(n), dipendente da $n\in\mathbb{N}$, **si dice vera definitivamente in n** se è vera "da un certo indice in poi", cioè se
$$\exists ñ\in \mathbb{N} : P(n)\ vera\ \forall n \in \mathbb{N}, n > ñ$$
##### Frequentemente
Una proprietà P(n), dipendente da $n\in\mathbb{N}$, **si dice vera frequentemente in n** se è vera "per un numero infinito di indici", cioè se
$$\forall n \in \mathbb{N}, \exists m\in \mathbb{N}, m>n : P(n)\ vera$$

### Confronto definitivo
Siano $(a_b)$ e $(b_n)$ due successioni reali di numeri non negativi. Se
- Se
$(i) \sum_{n=1}^{+\infty}b_n <+\infty$
$(ii) a_n \le b_n$ definitivamente in n,
Allora 
$\sum_{n=1}^{+\infty}a_n < +\infty$

- Se
$(i) \sum_{n=1}^{+\infty}b_n =+\infty$
$(ii) a_n \ge b_n$ definitivamente in n,
Allora
$\sum_{n=1}^{+\infty}a_{n } = +\infty$


![[Serie armonica#Serie armonica]]

![[Numero di Nepero#Numero di Nepero]]
### Criteri di convergenza
![[Criteri di convergenza serie a termini positivi]]

### Piccolezza definitiva degli addendi di una serie convergente
Sia $\sum_{h=1}^{+\infty}a_h$, una serie a termini positivi, convergente.
Allora per ogni $\epsilon > 0$ esiste $\nu_{\epsilon}\in \mathbb{N}$ tale che
$$a_{n}<\epsilon \ \ \ \forall n > \nu_\epsilon$$
##### Dimostrazione
Da fare

### Criterio di condensazione
Sia $a_n$ una successione non crescente. Allora
$$la\ serie \sum_{h=1}^{+\infty}a_{h}\ converge \iff \ la\ serie \sum_{h=1}^{+\infty}{2^ha_{2^h}}\ converge$$
##### Dimostrazione
Da fare

[[Serie armonica generalizzata]]
