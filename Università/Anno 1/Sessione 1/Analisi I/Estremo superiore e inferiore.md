Capitolo 4
## Minimi e Massimi
Sia $E\subseteq\mathbb{R}$ un insieme. Se esiste un numero $m\in\mathbb{R}$ che verifica:
  $(i)\ m \in E$
  $(ii)\ m \le e\ per\ ogni\ e \in E$
Se $m$ esiste, è unico e si dice **minimo di E** e si indica con $min\ E$.

Se il caso $(ii)$ è "$\ge$" , allora si parla di **massimo di E** e si indica con $max\ E$.

Esempi:
(0,1] non ammette minimo.
Se $E \subseteq \mathbb{N}$ allora $E$ ammette minimo ma non necessariamente massimo.

## Estremi superiori ed inferiori
Vogliamo trovare un sostituto del minimo di $E$ che esista sempre e coincida con $min\ E$ quando esiste, così come per il massimo.

#### Elemento separatore
Per ogni coppia di insiemi $A,B \subseteq \mathbb{R}$ non vuoti tali che $A \cup B = \mathbb{R}$ e 
$\qquad a \le b$ per ogni $a \in A$ e per ogni $b \in B$,
esiste ed è unico $c \in \mathbb{R}$ tale che
$\qquad a \le c \le b$ per ogni $a \in A$ e per ogni $b \in B$.

- $c$ viene detto **elemento separatore**.

$\mathbb{Q}$ ==non ha la proprietà dell'elemento separatore==
#### Insieme superiormente e inferiormente limitato
Un insieme $E \subseteq R$ non vuoto si dice superiormente limitato se esistono numeri reali maggiori di ogni elemento di E.
$$Maior(E) := \{a \in \mathbb{R}:a \ge e\ per\ ogni\ e \in E\}$$
Si dice inferiormente limitato se sono minori
$$Minor(E) := \{a \in \mathbb{R}:a \le e\ per\ ogni\ e \in E\}$$
#### Esistenza ed unicità estremi superiori ed inferiori
Dimostrazione
$$A := \{a \in \mathbb{R} : a \le e\ per\ qualche\ e\in E\}$$
$$B := Maior(E)$$
$$A\cup B = \mathbb{R} $$
Quindi per ogni $a\in A$ e $b\in B$, e per l' [[#Elemento separatore]], esiste un unica $c\in \mathbb{R}$ tale che
$$a \le c \le b$$
###### L'estremo superiore sarà indicato come:
$$sup\ E = min(Maior(E)).$$
Se E non fosse superiormente limitato, $sup\ E = +\infty$

Per l'estremo inferiore è tutto uguale con segno opposto.
###### L'estremo inferiore sarà indicato come
$$inf\ E = max(Minor(E))$$
Se E non fosse inferiormente limitato, $\inf E = -\infty$.

### Caratterizzazione
Supponiamo s = $sup E \in\mathbb{R}$, allora $s$ ha le seguenti proprietà:
$(i) s\ge e\ per\ ogni\ e\in E$
$(ii) \forall \epsilon > 0\ \exists e \in E : e > s - \epsilon$

Nel caso di $inf E$
$(i) i\ge e\ per\ ogni\ e\in E$
$(ii) \forall \epsilon > 0\ \exists e \in E : e < i + \epsilon$
### Esercizi 
4.0.14 - 4.0.18