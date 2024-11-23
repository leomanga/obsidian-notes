---
capitolo: 12
---
Vogliamo studiare una classe generale di funzioni $f$. Prima abbiamo studiato solo funzioni da $\mathbb{N}$ a $\mathbb{R}$.
Adesso studiamo le funzioni definite su un insieme $E\subseteq \mathbb{R}$ e a valori reali
$$f:E\subseteq\mathbb{R}\to\mathbb{R}$$
# Proprietà
Siano $\bar x \in \bar E,\qquad e \in \mathbb{R}$
Consideriamo queste proprietà:
1) $\forall \epsilon > 0\ \exists\delta_{\epsilon}> 0\mbox{ tale che }\forall x \in E, |x-\bar x| < \delta_{\epsilon}\ : |f(x)-p| <\epsilon$ 
2) Per ogni successione $e_{n}\subseteq E$ tale che $\lim_{n\to+\infty}e_{n}= \bar x$ si ha
$$\lim_{n\to+\infty}f(e_{n})= p$$
Le due proprietà sono equivalenti
### Osservazione
L'ipotesi $\bar x \in \bar E$ garantisce che esista almeno una successione di punti di $E$ convergente a $\bar x$.

#dimostrazione-da-fare 

# Definizione
Se per una funzione $f:E\subseteq \mathbb{R}\to \mathbb{R}$ per un punto $\bar x \in \bar E$ e un numero reale $p$ valgono le [[Limiti finiti di una funzione in un punto#Proprietà|proprietà]] 1 e 2, allora si dice che la funzione $f$ ha limite $p$ quando $x$ tende a $\bar x$ su $E$, e si scrive
$$\lim_{x\to\bar x}f(x) = p\qquad \mbox{su }\ E $$
o anche
$$f(x)\to p\mbox{ per }x\to\bar x \mbox{ su }\ E$$
# Teorema 12.0.12 | Limite della somma di funzioni
Se $f$ e $g$ sono due funzioni a valori reali definite su un insieme $E \subseteq \mathbb{R}$, se per $\bar x \in \bar E$ vale 
$$\lim_{x\to\bar x}f(x) = p \qquad su\ E,\qquad \lim_{x\to\bar x}g(x) = q\qquad su\ E$$
con $p,q \in \mathbb{R}$, allora anche la funzione $f+g$ ha limite per $x$ che tende a $\bar x$ su $E$ ed è
$$\lim_{x\to\bar x}(f(x)+g(x)) = p+q\qquad su\ E$$
#dimostrazione-da-fare 

# Definizione 12.0.13 | Funzione superiormente e inferiormente limitata
Sia $f:E \subseteq\mathbb{R}\to \mathbb{R}$ una funzione. Diciamo che $f$ è superiormente limitata se esiste $K\in\mathbb{R}$ tale che
$$f(x)\le K \qquad \forall x \in E$$
Invece si dice che è inferiormente limitata se esiste $K \in \mathbb{R}$ tale che
$$f(x)\ge K\qquad\forall x \in E$$

Una funzione $f:E \subseteq\mathbb{R}\to \mathbb{R}$ è superiormente limitata se $f(E)$ è un sottoinsieme [[Estremo superiore e inferiore#Insieme superiormente e inferiormente limitato|superiormente limitato]] dei numeri reali, è inferiormente limitata se $f(E)$ è un sottoinsieme [[Estremo superiore e inferiore#Insieme superiormente e inferiormente limitato|inferiormente limitato]] dei numeri reali.
# Definizione 12.0.15 | Funzione limitata
Una funzione $f:E \subseteq\mathbb{R}\to \mathbb{R}$ è limitata se esiste $K \in \mathbb{R}$ tale che
$$|f(x)|\le K\qquad \forall x \in E$$
cioè se $f$ è limitata sia dall'alto che dal basso.
Una funzione $f:E \subseteq\mathbb{R}\to \mathbb{R}$ è limitata se $f(E)$ è un sottoinsieme limitato dei numeri reali.

# Teorema 12.0.16
Siano $f$ e $g$ due funzioni a valori reali definite su $E \subseteq \mathbb{R}$. Se $g$ è limitata e se per $\bar x \in \bar E$ è
$$\lim_{x\to\bar x}f(x) = 0\qquad su\ E,$$
allora
$$\lim_{x\to\bar x}f(x)g(x) = 0\qquad su\ E$$
#dimostrazione-da-fare 

# Lemma 1 | Restrizione
Sia $f$ una funzione reale definita su $E\subseteq \mathbb{R}$ e per $\bar x \in \bar E$ e $p\ in\ \mathbb{R}$ sia
$$lim_{x\to\bar x}f(x) = p\qquad su\ E$$
Allora, se $L \subseteq E$ e $\bar x \in \bar L$ si ha anche
$$\lim_{x\to\bar x}f(x) = p\qquad su\ L$$
#dimostrazione-da-fare 

# Lemma 2 | Localizzazione
Sia $f$ una funzione reale definita su $E\subseteq \mathbb{R}$ e per $\bar x \in \bar E$. Se per $p > 0$ si pone
$$L:= \{x\in E : |x-\bar x| < p\} = E\ \cap\ \{x-p,x+p\}$$
Si ha che il limite di $f$ su $E$ per $x$ tendente a $\bar x$ esiste se e solo se esiste il limite di $f$ su $L$ per $x$ tendente a $\bar x$.
#dimostrazione-da-fare 
# Lemma 3 | Unione
Se $f$ è una funzione reale definita su $E \cup L \subseteq \mathbb{R}$
Se $\bar x \in \bar E \cap \bar L$ e se vale
$$\lim_{x\to\bar x}f(x) = p\qquad \mbox{ su E},\qquad \lim_{x\to\bar x}f(x) = p\qquad \mbox{ su L}$$
allora si ha anche
$$\lim_{x\to\bar x}f(x) = p\qquad \mbox{ su } E\cup L$$
#dimostrazione-da-fare 

# Lemma 4| Composizione
Sia $f$ una funzione reale definita su $E \subseteq \mathbb{R}$ e $g$ una funzione reale definita su $L \supseteq f(E)$. Per $\bar x \in \bar E$ sia
$$\lim_{x\to \bar x}f(x) = p\quad su\ E,$$
$$\lim_{y\to p}g(y) = q\quad su\ L.$$
Allora esiste una funzione composta $g(f(x))$ per $x$ tendente a $\bar x$ su $E$ e si ha
$$\lim_{x\to \bar x}g(f(x)) = q\quad su\ E$$
Si noti che $p \in \overline {f(E)}$.
#dimostrazione-da-fare 
