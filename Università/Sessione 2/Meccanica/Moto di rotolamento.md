---
collegamenti:
  - "[[Capitolo 9 - Corpi rigidi]]"
---
Il moto di rotolamento è un moto di [[Moto di rotazione|rotazione]] e di [[Moto di traslazione|traslazione]] caratterizzato da avere, istante per istante, un punto con velocità nulla, ovvero il punto di contatto con il tracciato.

![[Moto di rotolamento.png]]

>[!def] Velocità generico punto
>La velocità di un generico punto può essere scritta, istante per istante come
>$$\vec{v}_{p}=\vec{\omega}\times\vec{r}_{CP}$$
>In particolare, per il centro di massa
>$$\vec{v}_{CM}=\vec{\omega}\times \vec{r}_{CM}$$

^8df93a

>[!def] Accelerazione centro di massa
>Da [[#^8df93a]]
>$$\vec{a}_{CM}=\alpha\vec{r}$$

^31ae89

Analizziamo ora la dinamica.
Supponiamo che sul centro di massa sia applicata una forza $\vec{F}$ orizzontale che trascina il disco lungo il piano.
Allora posso calcolare l'accelerazione del centro di massa dato che 
$$m\vec{a}_{CM}=\vec{R}$$
Dove $\vec{R}$ è la risultante delle forze, che sarà data da $\vec{F}$, $\vec{N}$, ovvero la reazione vincolare, $\vec{F}_{p}$, ovvero la forza peso e $\vec{f}$, che prende il nome di ==forza di aderenza==, ovvero la forza generata dall'attrito tra il disco e il tracciato, che consente il moto di rotolamento.

Se consideriamo solo le componenti orizzontali e verticali avremo che 
$$ma_{CM}=F-f$$
In direzione verticale, invece $$N-mg = 0$$
Adesso consideriamo i momenti, il momento angolare, da [[Moto di rotazione]] $$\vec{M}=\frac{d\vec{L}}{dt}$$
Sapendo che $\vec{L}=I_{z} \vec{\omega}$, avremo che $\vec{M}=I_{z}\vec{\alpha}$, dove $I_{z}$ è il [[Moto di rotazione#^a5ff25|momento di inerzia]] nella componente $z$.

Inoltre, da [[Momento di una forza]], avremo anche che $\vec{M}=\vec{r}\times \vec{f}$.
Allora calcoliamo il momento rispetto ad $0$
$$I_{z}\vec{\alpha}=\vec{r}\times \vec{f}$$
Possiamo solo considerare la componente in direzione perpendicolare al piano $(z)$. (negli appunti è scritto così, ma dipende come vediamo la situazione, nel nostro caso, la componente è quella in direzione dell'asse di rotazione)

$$I_{z}\alpha=fR\Rightarrow f= \frac{I_{z}\alpha}{R}$$
Riprendendo [[#^31ae89]], possiamo scrivere quindi che 
$$ma_{CM}=F-\frac{I_{z}a_{CM}}{R^{2}}$$
Possiamo allora ricavare l'accelerazione del centro di massa
>[!prp] Equazione accelerazione del centro di massa 1
>$$a_{CM}=\frac{F}{m+\frac{I_{z}}{R^{2}}}$$
Possiamo inoltre calcolare $f$

>[!prp] Equazione forza di aderenza 1
>$$f=\frac{F}{1+ \frac{mR^{2}}{I_{z}}}$$
>All'aumentare di $F$, $f$ aumenta.  Questo incremento però è limitato dalla relazione dell'attrito coulombiano ([[Capitolo 5 - Dinamica del punto materiale 1#^439577]]). Se questo limite non è soddisfatto, la condizione di rotolamento non può essere soddisfatta e la ruota slitta.

Analizziamo ora il caso in cui alla ruota è applicata una coppia di forze con momento pari a $\vec{M}$.
Riprendendo l'equazione dei momenti $$\frac{d\vec{L}}{dt}=\vec{M}_{tot}$$
Avremo che $$I_{z}\vec{\alpha}=\vec{r}\times \vec{f}+\vec{M}$$
Se consideriamo la componente in direzione del momento, $$I_{z}\alpha = -fR+M$$
Allora
>[!prp] Equazione forza di aderenza 2
>$$f=\frac{M-I_{z}\alpha}{R}$$

Se guardiamo l'accelerazione, avremo che 
$$ma_{CM}=f\Rightarrow ma_{CM} = \frac{M-I_{z}\alpha}{R}$$
Troviamo quindi
>[!prp] Equazione accelerazione del centro di massa 2
>$$a_{CM}=\frac{MR}{mR^{2}+I_{z}}$$

Possiamo scrivere nuovamente la forza di aderenza

>[!prp] Equazione forza di aderenza 3
>$$f=m\frac{MR}{mR^{2}+I_{z}}=\frac{M}{R(1+ \frac{I_{z}}{m}R^{2})}$$
>La forza di aderenza quindi dipende dal momento della coppia applicata, ma anche in questo caso deve rispettare il vincolo di aderenza
>$$f\le \mu_{s}N$$

