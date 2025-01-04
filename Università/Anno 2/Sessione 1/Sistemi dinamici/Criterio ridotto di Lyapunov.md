Sia $\bar x$ uno [[Stati di equilibrio|stato di equilibrio]] del sistema lineare a tempo continuo
$$
\dot x(t)=f(x(t))
$$

^8c8dd1

calcoliamo la [[Matrice Jacobiana]] di $f$ nello stato di equilibrio. Sappiamo che, da [[Tecniche di linearizzazione dei sistemi dinamici non lineari]]
$$A = [\frac{\partial f}{\partial x}]_{x=\bar x}\in \mathbb{R}^{n\times n}$$
Siano $\lambda_{1},\lambda_{2},\ldots,\lambda_{n}$ gli [[Autovettori - autovalori - autospazi#Definizione Autovalore|autovalori]] di $A$. Si ha che
- Se $Re[\lambda_{i}]<0\ \forall i=1,\ldots,n$, allora $\bar x$ è uno [[Stabilità dei sistemi dinamici#^9f43ed|stato di equilibrio asintoticamente stabile]] per il sistema [[#^8c8dd1]].
- Se esiste $\lambda_{j}>0$, allora $\bar x$ è uno [[Stabilità dei sistemi dinamici#^24cae2|stato di equilibrio instabile]] per il sistema [[#^8c8dd1]]. 

Per i sistemi a tempo discreto vale lo stesso, solo che
- Se $\lambda_{i}<1\ \forall i=1,\ldots,n$, allora $\bar x$ è asintoticamente stabile.
- Se esiste $\lambda_{i}>1$, allora $\bar x$ è uno stato di equilibrio instabile.