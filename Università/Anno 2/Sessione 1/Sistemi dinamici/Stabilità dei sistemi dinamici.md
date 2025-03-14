>[!def] Stato di equilibrio stabile
>Uno stato di equilibrio $\bar x$ si dice stabile se
>$$\forall \epsilon>0,\ \ \exists\delta>0:||x(0)-\bar x||<\delta\Rightarrow||x(t)-\bar x||<\epsilon\ \ \forall t\ge 0$$
>In poche parole se, perturbando minimamente lo stato di equilibrio, il sistema, nel tempo, assumerà stati che non si discosteranno mai troppo dallo stato di equilibrio.
>![[Equilibrio stabile.excalidraw]]

^3ca209

>[!def] Stato di equilibrio asintoticamente stabile
>Uno stato di equilibrio $\bar x$ si dice asintoticamente stabile se è sia [[#^3ca209|stabile]] che [[Stati di equilibrio#^8441cb|convergente]].

^9f43ed

>[!def] Stato instabile
>Sia $\bar x$ uno stato di equilibrio. 
>Si ha che se $\bar x$ non è [[Stati di equilibrio#^a3abc3|stabile]] , allora si dice instabile

^24cae2

>[!def] Stato marginalmente stabile
>Se $\bar x$ è [[Stati di equilibrio#^a3abc3|stabile]] ma non [[Stati di equilibrio#^8441cb|convergente]], allora si dice marginalmente stabile.

^e54644

>[!prp]
>Esistono stati di equilibrio [[Stati di equilibrio#^8441cb|convergenti]] ma [[#^24cae2|instabili]]. Questo accade solo nei sistemi non lineari. 
>Nei sistemi lineari gli stati di equilibrio convergenti sono sempre stabili.

>[!def] Stato di equilibrio GAS
>Uno stato di equilibrio $\bar x$ si dice globalmente asintoticamente stabile (GAS) se
>$$\forall x(0)\in \mathbb{R}^{n}\quad \lim_{t\to +\infty}||x(t)-\bar x||=0$$
>

^3e6b69

![[Criterio ridotto di Lyapunov]]

# Studio della stabilità
Chiamiamo traiettoria del sistema lineare la risposta libera e si ha che, da [[Analisi modale nello spazio degli stati per sistemi a tempo discreto|(L1)]] e [[Analisi modale nello spazio degli stati per sistemi a tempo continuo|(L2)]]
- nel tempo continuo $x(t)=e^{At}\cdot x(0)$
- nel tempo discreto $x(k)=A^{k}\cdot x(0)$

Nel tempo contino, da [[#^3ca209]], con $\bar x=0$ si ha
$$\forall \epsilon >0,\exists \delta >0:||x(0)||<\delta\Rightarrow||x(t)||<\epsilon$$
Però $||x(t)||<\epsilon\iff ||e^{At}\cdot x(0)||<\epsilon$.
Avremo che (vale anche per il tempo discreto)
- se tutti i modi sono convergenti[^1], allora $\bar x=0$ è [[#^9f43ed|asintoticamente stabile]].
- se i modi sono convergenti oppure limitati non convergenti[^2], allora $\bar x=0$ è [[#^e54644|marginalmente stabile]].
- se è presente un modo divergente[^3], allora $\bar x$ è [[#^24cae2|instabile]].

In termini di autovalori $\lambda_{1},\lambda_{2},\ldots,\lambda_{n}$ di $A$, possiamo dire che,

nel tempo continuo il sistema è:
- **Asintoticamente stabile** se $Re[\lambda_{i}]<0\ \forall i=1,\ldots,n$ (Da [[Criterio ridotto di Lyapunov]])
- **Marginalmente stabile** se rispetta entrambi:
	- $Re[\lambda_{i}]\le 0$ per $i=1,2,\ldots,n$
	- $\forall \lambda_{i}$ tale che $Re[\lambda_{i}]=0$ allora [[Autovettori - autovalori - autospazi#Molteplicità algebrica|ma]]$(\lambda_{i})$ = [[Autovettori - autovalori - autospazi#Molteplicità geometrica di $ lambda$|mg]]$(\lambda_i )$
- **Instabile** negli altri casi

nel tempo discreto il sistema è:
- **Asintoticamente stabile** se $|\lambda_{i}|<1\ \forall i=1,\ldots,n$ (Da [[Criterio ridotto di Lyapunov]])
- **Marginalmente stabile** se rispetta entrambi:
	- $|\lambda_{i}|\le 1$ per $i=1,2,\ldots,n$
	- $\forall \lambda_{i}$ tale che $|\lambda_{i}|=1$ allora [[Autovettori - autovalori - autospazi#Molteplicità algebrica|ma]]$(\lambda_{i})$ = [[Autovettori - autovalori - autospazi#Molteplicità geometrica di $ lambda$|mg]]$(\lambda_i )$
- **Instabile** negli altri casi

# Proprietà dei sistemi lineari
- Nei sistemi autonomi ($u(t)=0\forall t$), $\bar x=0$ è sempre stato di equilibrio.
- Il sistema può essere asintoticamente stabile solo se $\bar x=0$ è l’unico stato di equilibrio.
- Se $\bar x=0$ è stato di equilibrio convergente, allora è anche stabile e quindi asintoticamente stabile.
- Se $\bar x=0$ è asintoticamente stabile, allora è anche [[#^3e6b69|GAS]].

# Stabilità esterna
Fin ora abbiamo studiato la stabilità interna, che riguarda i sistemi nella [[Rappresentazione ingresso-stato-uscita]], ora studiamo i sistemi nella [[Rappresentazione ingresso-uscita]]

>[!def] Stabilità in senso ILUL
>Un sistema dinamico è stabile in senso ILUL(ingresso limitato, uscita limitata)(in inglese BIBO, bounded-input, bounded-output) se
>$$\forall U>0,\ \exists Y>0:\ ||u(t)||\le U\ \ \forall t\ge 0\Rightarrow ||y(t)||\le Y\ \forall t\ge 0$$
>Come per definizione del nome infatti abbiamo che se l’ingresso è l’imitato, anche l’uscita è limitata.

^ef9adb


Abbiamo che,
in un sistema a tempo continuo, dato che $Y(s)=G(s)U(s)$, allora se per ogni polo di $G(s)$ a parte reale nulla, $\exists$ un ingresso $u(t)$ limitato che genera un $y(t)$ divergente, allora deduciamo che

>[!prp]
>Un sistema a tempo continuo è [[#^ef9adb|stabile in senso ILUL]] se e solo se tutti i poli di $G(s)$ hanno parte reale negativa.

Invece, nel caso del tempo discreto
>[!prp]
>Un sistema a tempo discreto è [[#^ef9adb|stabile in senso ILUL]] se e solo se tutti i poli di $G(s)$ hanno modulo minore di 1.

>[!lemma]
>Se un sistema è asintoticamente stabile internamente, allora è ILUL stabile, perché i poli della funzione di trasferimento sono un sottoinsieme degli autovalori di $A$. 
>Inoltre si ha che il viceversa non è vero perché potrebbero esserci autovalori di $A$ non convergenti, ma che si cancellano con uno zero.

[^1]:[[Modi di un sistema dinamico lineare a tempo continuo#Convergenti]], [[Modi di un sistema dinamico lineare a tempo discreto]]
[^2]:[[Modi di un sistema dinamico lineare a tempo continuo#Limitati non convergenti]], [[Modi di un sistema dinamico lineare a tempo discreto]]
[^3]:[[Modi di un sistema dinamico lineare a tempo continuo#Divergenti]], [[Modi di un sistema dinamico lineare a tempo discreto]]
