---
aliases:
  - Segnale numerico
---
Un segnale digitale è una funzione del tipo
$$s[n]$:\mathbb{N}\to \{1,2,\ldots,M\}$$
dove $1,2,\ldots, M$ sono i valori discreti [[Quantizzazione|quantizzati]] di un segnale analogico.

# Segnali antipodali
$M=2$
$S_{1}(t)=-S_{2}(t)$
$E_{1}= E_{2}=E_{b}$ ($E_{i}$ è [[Segnali#^f4d1be]], $E_b$ sta per energia di un bit)

Studiando la [[Rappresentazione vettoriale di un segnale]], avremo che la dimensione della base per rappresentare questi segnali è 1, dato che uno è combinazione dell’altro.
Avremo allora come base
$$\left\{\phi_{1}=\frac{S_{1}(t)}{\sqrt E_{1}}\right\}$$
$S_{1}(t)=\sqrt E_{b}\phi_{1}(t)\rightarrow \vec{S_{1}}=\sqrt E_{b}$ 
$S_{2}(t)=-\sqrt E_{b} \phi_{1}(t)\rightarrow \vec{S_{1}}=-\sqrt E_{b}$

![[Segnali antipodali.excalidraw]]
# Segnali ortogonali
$M$ segnali [[Rappresentazione vettoriale di un segnale#^9ac538|ortogonali]].

Avremo allora che $\phi(i)=\frac{S_{i}(t)}{\sqrt E_{i}}\quad \forall i,\ldots, M$ e
$$\vec{s_{i}}=(0,0,\ldots, \sqrt E_{i},\ldots, 0)$$

![[Segnali ortogonali.excalidraw]]

