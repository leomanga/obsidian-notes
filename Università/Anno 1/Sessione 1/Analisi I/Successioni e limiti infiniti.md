---
capitolo: 7
collegamenti: "[[Successioni e limiti finiti]]"
---
# Limite infinito
Una successione $a_{n}$ si dice che diverge verso +  infinito se
$$\forall L \in \mathbb{R} \ \ \exists \nu_{L}\in \mathbb{N}:a_{n}> L\ \ \ \forall n > v_L$$
Una successione $a_{n}$ si dice che diverge verso -  infinito se
$$\forall L \in \mathbb{R} \ \ \exists \nu_{L}\in \mathbb{N}:a_{n}< L\ \ \ \forall n > v_L$$

### Confronto
Se $a_{n}\to +\infty$ e $b_{n}\ge a_{n}$ definitivamente in n, allora $b_{n}\to+\infty$.
Se $a_{n}\to -\infty$ e $b_{n}\le a_{n}$ definitivamente in n, allora $b_{n}\to -\infty$.
#dimostrazione-da-fare 

# Criteri di convergenza
Simile a 
[[Serie numeriche a termini di segno costante#Criteri di convergenza]]
Con c > 1.
##### Rapporto
Se
$$ \frac{a_{h+1}}{a_{h}} \ge c\ \ \ \forall h > n$$
allora $a_{h}\to +\infty$
#dimostrazione-da-fare 
##### Radice
Se 
$$\sqrt[h]{a_{h}} \ge c \ \ \ \forall h > n$$
allora $a_{h}\to +\infty$
#dimostrazione-da-fare 


# Teorema 7.0.12 - 7.0.13 | Sottosuccessioni estratte
Generalizzazione di [[Successioni e limiti finiti#Teorema di Bolzano-Weierstrass]]

- Se $a_n$ una successione divergente e $b_n$ una successione estratta da $a_n$, allora anche $b_n$ è divergente verso lo stesso limite.
- Da ogni successione $a_n$ si possono estrarre sottosuccessioni aventi limite finito o infinito. Se la successione $a_n$ non ha limite, da essa si possono estrarre sottosuccessioni aventi limiti finiti differenti.

#### Osservazione
Se prendiamo $a_{n}= (-1)^{n}n$ . Allora $a_n$ non ha limite né finito né infinito

#### Esercizi 7.0.16-17

# Operazioni algebriche e limiti infiniti
[[Successioni e limiti finiti#Operazioni algebriche e limiti finiti]]

#### Somma
Siano $a_n$ e $b_n$ due successioni reali tali che
$$a_{n}\to +\infty$$
e $$ b_{n}\ge s\ \ \ \forall n \in \mathbb{N}$$
allora $$\lim_{n\to +\infty}(a_{n}+ b_{n})= +\infty$$
#dimostrazione-da-fare 
##### Osservazione
Non vale se $a_{n}\to +\infty$ e $b_{n}\to -\infty$
Questa viene detta <mark style="background: #FFB86CA6;">forma indeterminata</mark>.

#### Prodotto
Siano $a_n$ e $b_n$ due successioni reali tali che
$$a_{n}\to +\infty$$
e
$$\exists p > 0 : b_{n}\ge p \ \ \ \forall n \in \mathbb{N}$$
allora $$\lim_{n\to +\infty}(a_{n} b_{n})= +\infty$$
#dimostrazione-da-fare 
##### Osservazione
Non vale con $a_{n}\to \pm \infty$ e $b_{n}= 0$
Anche questa è una <mark style="background: #FFB86CA6;">forma indeterminata</mark>.

#### Teorema 7.1.6
Se $b_{n}\ne 0\ \ \ \forall n \in \mathbb{N}$ e se $b_{n}\to 0$
allora
$$\frac{1}{|b_{n}|} \to +\infty$$
#dimostrazione-da-fare 

# Successioni monotone
[[Successioni e limiti finiti#Successioni monotone limitate]]
#### Teorema 7.2.1
Se la successione $a_n$ è <mark style="background: #FFB86CA6;">non decrescente e non superiormente limitata</mark> allora $a_{n}\to +\infty$.
#dimostrazione-da-fare 

#### Teorema 7.2.2
Se la successione $a_n$ è <mark style="background: #FFB86CA6;">non crescente e non inferiormente limitata</mark> allora $a_{n}\to -\infty$.

#### Teorema 7.2.3 | Teorema fondamentale delle successioni monotone

Sia $a_n$ una [[Serie numeriche a termini di segno costante#Successione monotona|successione monotona]]. Allora ammette sempre limite uguale all'estremo superiore o inferiore.
- Se $a_n$ è **non decrescente**:
$$\lim_{n\to +\infty} a_{n}= sup \{a_{n} : n\in \mathbb{N}\} = sup\ a(\mathbb{N})$$
- Se $a_n$ è **non crescente**:
$$\lim_{n\to +\infty} a_{n}= inf \{a_{n} : n\in \mathbb{N}\} = inf\ a(\mathbb{N})$$
###### <mark style="background: #FFB86CA6;">Quindi, ogni successione monotona o è convergente a un numero reale o diverge verso + o - infinito.</mark>

![[Limiti notevoli#7.2.4]]
Es 7.2.5-7.2.10

# Criterio del rapporto-radice
![[Critero del rapporto-radice limiti]]

# Medie di Cesaro
![[Medie di Cesaro]]