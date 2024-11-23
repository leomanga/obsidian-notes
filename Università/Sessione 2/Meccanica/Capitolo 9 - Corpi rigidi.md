>[!def] Corpo rigido
>Un corpo rigido è un sistema di [[Capitolo 8 - Sistemi di punti materiali|punti materiali]] in cui la distanza tra una qualsiasi coppia di punti che lo costituiscono rimane costante.

Per lo studio del moto di un corpo rigido possiamo definire diversi sistemi di riferimento:
- Sistema di riferimento [[Capitolo 7 - Dinamica dei moti relativi#^338e71|inerziale]].
- Sistema di riferimento con origine nel centro di massa e assi paralleli a quelli del sistema inerziale.
- Sistema di riferimento con origine nel centro di massa e assi che ruotano assieme al corpo rigido.

Nel caso dei corpi rigidi, il lavoro interno è pari a zero dato che i punti non si sposano uno rispetto l'altro. Terremo quindi solo di conto il lavoro delle forze esterne. ==Verrà quindi omesso l'apice==$(E)$

>[!prp] Coordinate di un corpo rigido
>In un corpo rigido, le coordinate di un qualsiasi punto solidare rispetto al sistema di riferimento con origine in $CM$ e assi solidali al corpo sono fisse.
>Per conoscere la posizione di qualsiasi punto solidale al corpo sarà quindi sufficiente conoscere le coordinate del $CM$(coordinate dell'origine del sistema mobile) e quelle del punto rispetto al $CM$(coordinate del punto nel sistema mobile).
>
>Il sistema di riferimento sarà quindi definito dalla posizione del centro di massa $\vec{r}_{CM}$ e $\vec{i}^{'},\vec{j}^{'},\vec{k}^{'}$.
>Chiaramente per definire $\vec{r}_{CM}$ avrò bisogno delle 3 componenti cartesiane $x,y,z$.
>Inoltre posso definire le componenti dei versori $\vec{i}^{'},\vec{j}^{'},\vec{k}^{'}$.
>$$\vec{i}^{'}=i^{'}_{x}\vec{i}+i^{'}_{y}\vec{j}+i^{'}_{z}\vec{k}$$
>$$\vec{j}^{'}=j^{'}_{x}\vec{i}+j^{'}_{y}\vec{j}+j^{'}_{z}\vec{k}$$
>$$\vec{k}^{'}=k^{'}_{x}\vec{i}+k^{'}_{y}\vec{j}+k^{'}_{z}\vec{k}$$
>
>Inoltre, sapendo che i versori $\vec{i}^{'},\vec{j}^{'},\vec{k}^{'}$ hanno modulo unitario e sono ortogonali tra loro, ottengo che sono legati da 6 relazioni. Dato che i parametri di cui ho bisogno sono 9, ottengo che solo 3 di loro sono indipendenti. 
>
>Dovrò quindi specificare 3 parametri per $\vec{r}_{CM}$ e 3 parametri per i versori $\vec{i}^{'},\vec{j}^{'},\vec{k}^{'}$.
>
>---
>$CM$ è il [[Capitolo 8 - Sistemi di punti materiali#^a2fd88|centro di massa]].

>[!def] Densità di un volume
>$$\rho = \frac{dm}{dV}\Rightarrow dm = \rho dV\qquad[\frac{kg}{m^{3}}]$$
>Questo concetto, in caso di prevalenza di alcune dimensioni sulle altre, si può ridurre a 2 dimensioni (piastre, membrane, lamiere) e ad 1 dimensione (cavi, aste, funi).

^8c930d

>[!def] Corpo continuo
>I corpi continui sono sistemi costituiti da un numero molto elevato di punti di massa infinitesima.
>Abbiamo visto che per un sistema discreto, la massa si calcola con l'operazione della sommatoria su tutti i punti, per un sistema continuo dobbiamo usare l'integrale:$$m=\int dm=\underbrace{\int_{V}\rho dV}_{(*)}$$
>Da qui avremo che il [[Capitolo 8 - Sistemi di punti materiali#^a2fd88|centro di massa]] potrà essere calcolato così:$$\vec{r}_{CM}=\frac{\int \vec{r} dm}{\int dm}=\frac{\int_{V}\vec{r}\rho dV}{m}$$
>$(*)$ da [[#^8c930d]].

>[!def] Corpo omogeneo
>Se la [[#^8c930d|densità]] è costante, il corpo si dice omogeneo e vale la relazione $$m=\rho V$$
>

^ee70c9

>[!prp] Centro di simmetria in un corpo omogeneo
>Se un corpo è [[#^ee70c9|omogeneo]] ed ha un centro di simmetria, allora avrà una coincidenza fra il centro di massa e il centro di simmetria.
>
>Inoltre, se un corpo omogeneo ha un asse di simmetria, allora il centro di massa si troverà su quell'asse.
>
>Se un corpo ha un piano di simmetria, il centro di massa si troverà su quel piano, se un corpo omogeneo ha due o più piani di simmetria, il centro di massa si trova nell'intersezione dei piani.
>
>Guarda pag 26 per esempi
# Moto di traslazione
![[Moto di traslazione]]

# Moto di rotazione
![[Moto di rotazione]]

>[!def] Moto generico
>Il moto generico è quel moto rappresentabile istante per istante come combinazione di una rotazione o una traslazione.

# Moto di rotolamento
![[Moto di rotolamento]]

# Energia cinetica in un moto generico
Abbiamo visto che nel [[Moto di traslazione]], l'energia cinetica è definita come
![[Moto di traslazione#^1bf629]]

Nel [[Moto di rotazione]], invece, l'energia cinetica è definita come
![[Moto di rotazione#^5ff6dc]]

Avremo quindi che l'energia cinetica in un moto generico sarà 
$$E_{k}= E_{kt}+E_{kr}$$
dove $E_{kr}$ è l'energia cinetica della parte di rotazione, mentre $E_{kt}$ tiene conto della parte di traslazione del moto generico.

Studiamo il caso particolare in cui $E_{kr}=\frac{1}{2} I\omega ^{2}$
Sapendo che nel moto di rotolamento $v_{CM}=R\omega$, possiamo scrivere
$$
E_{k}= \frac{1}{2}I_{z}\omega^{2}+ \frac{1}{2}mv^{2}_{CM}=\frac{1}{2}(I_{z}+mR^{2})\omega^{2}
$$
esempio a pag 21