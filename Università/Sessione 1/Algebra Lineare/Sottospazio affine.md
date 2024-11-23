---
aliases:
  - sottospazi affini
  - sottospazio affine
pagina: 170
---
# Più piccolo sottospazio affine
Sia $\mathbb{X}$ un insieme di vettori non vuoto di $V$.
$Af(\mathbb{X})$ è il più piccolo sottospazio affine che contiene l'insieme $\mathbb{X}$.
1) $Af(\mathbb{X}) \supseteq \mathbb{X}$
2) $Af(\mathbb{X})$ è sottospazio affine
3) Se $\mathbb{S}$ [[Spazio affine]] tale che $\mathbb{X}\subseteq \mathbb{S}$.
	Allora $Af(\mathbb{X})\subseteq \mathbb{S}$

Siano $A, B$ basi
$Af(A,B) = A + L(B-A) =  B+(A-B) =  B+(B-A)$
-Stesso principio con più basi
# Proposizione
$$Af(\mathbb{X}) = \cap\{\mathbb{S}:\mathbb{S}\mbox{ spazio affine e } \mathbb{X}\subseteq \mathbb{S}\}$$
# Proprietà
Sia $\mathbb{X}\subseteq V$
- $\mathbb{X} \subseteq Af(\mathbb{X}), \forall\mathbb{X}\subseteq V$
- $\mathbb{X}\subseteq \mathbb{Y} \Rightarrow Af(\mathbb{X}) \subseteq \mathbb{Y}, \forall \mathbb{X}, \mathbb{Y}\subseteq V$
- $\mathbb{X}\subseteq Af(\mathbb{Y}) \iff Af(\mathbb{X})\subseteq Af(Af(\mathbb{Y})) = Af(\mathbb{Y})$
- $Af(\mathbb{X}\cap\mathbb{Y})\subseteq Af(\mathbb{X})\cap Af(\mathbb{Y})$
- $Af(\mathbb{X} \cup \mathbb{Y}) = Af(Af(\mathbb{X})\cup Af(\mathbb{Y}))$
- $Af(\mathbb{X})\subseteq L(\mathbb{X})$
- $Af(\mathbb{X}) = L(\mathbb{X})\iff 0\in Af(\mathbb{X})$
- $L(\mathbb{X}) = Af(\mathbb{X} \cup {0}) = Af(L(\mathbb{X})) = L(Af(\mathbb{X}))$
- $\dim(Af(\mathbb{X})) \le \dim(L(\mathbb{X})) \le \dim(Af(\mathbb{X})) + 1$
- 