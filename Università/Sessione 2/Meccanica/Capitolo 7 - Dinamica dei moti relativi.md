In questo capitolo studiamo il moto di un punto materiale visto da due sistemi di riferimento, dopo l'azione di una forza $\vec{F}$. 
Dal [[Capitolo 5 - Dinamica del punto materiale 1#^ee9546|secondo principio della dinamica]] sappiamo che $\vec{F}=m\vec{a}$.
Dato però che nei moti relativi, i due punti vedono il punto muoversi con accelerazioni diverse fra loro, dobbiamo fare attenzione a quale sistema di riferimento scegliere per rappresentare il moto.

>[!def] Sistema di riferimento inerziale
>Un sistema di riferimento inerziale è un sistema per il quale vale il [[Capitolo 5 - Dinamica del punto materiale 1#^538083|principio di inerzia]].

^338e71

Sia $S_{O}=\{O,x,y,z\}$ un sistema inerziale, se scegliamo un secondo sistema di riferimento $S_{O^{'}}=\{O^{'},x^{'},y^{'},z^{'}\}$ che si muove rispetto al primo con velocità costante (moto uniforme) e $\vec{\omega}=0$. Abbiamo visto in [[Capitolo 7 - Cinematica dei moti relativi]] che $\vec{a}=\vec{a^{'}}$.
I due sistemi vedono quindi il punto $P$ muoversi con la stessa accelerazione.
Allora se per $S_{O}$ vale $\vec{F}=m\vec{a}$, lo stesso vale per $S_{O^{'}}$.
Vuol dire quindi che anche $S_{O^{'}}$ è inerziale.
Allora abbiamo questo principio

>[!prp] Principio di relatività galileiana
>Non abbiamo modo di considerare fissi e mobili due sistemi inerziali.

Supponiamo ora che il secondo sistema $\vec{S_{O^{'}}}$ verifichi almeno una di queste condizioni
$$\vec{\omega}\not=0,\quad \frac{d\vec{\omega}}{dt}\not =0,\quad\vec{a}_{O^{'}}\not = 0$$
In questo modo, ricordandoci che
![[Accelerazione - moti relativi#^2f665c]]
potremo dire che $\vec{a}\not = \vec{a^{'}}$.

Allora, se per $S_{O}$, che consideriamo il sistema fisso, ho $\vec{F}=m\vec{a}$, avrò che per $S_{O^{'}}$ $$\vec{F}=m(\vec{a^{'}}+\vec{a}_{tr}+\vec{a}_{c})=m\vec{a^{'}} + m\vec{a_{tr}}+m\vec{a_{c}}$$

>[!def] Forze apparenti
>Abbiamo visto che in $S_{O^{'}}$, $\vec{F} = m\vec{a^{'}} + m\vec{a_{tr}}+m\vec{a_{c}}$. Chiameremo forze di inerzia o forze apparenti $$\vec{F}_{a}=-m\vec{a}_{tr}-m\vec{a}_{c}$$
