---
aliases:
  - probabilità
---
> [!def] Probabilità
> $$P(c) = \lim_{n\to +\infty}\frac{n_{c}}{n}\quad \scriptsize{n_{c} \mbox{, n volte che si verifica } c}$$

^f0d964

>[!axiom] Assiomi
>$1)\ \forall A\in \xi,\ P(A)\ge 0$
>$2)\ P(S) = 1$
>$3)\ \forall A,B\subset S:\ A\cap B = \varnothing,\ P(A\cup B) = P(A)+P(B)$

>[!corollary]
>$1)\ P(\varnothing)=0$
>$2) P(\overline{A}) = 1-P(A)\quad\scriptsize{(\overline{A} = \mbox{ complementare di } A)}$
>$3)\ A,B\in \xi\subset S, \ P(A\cup B)=P(A)+P(B)-P(A\cap B)$
>$4) A\subset B\Rightarrow P(A)\le P(B)$
>$5)(\mbox{Caso } S\mbox{ discreto})A\subset S, P(A)=\sum_{S_{i}\in A}P(S_{i})$
>$5.1)(\mbox{Caso } S\mbox{ continuo})A\subset S, P(x\in A)=\int_{A}a(x)dx$
>

![[Probabilità condizionata]]

>[!thm] Teorema della probabilità totale
>$$P(B)=\sum_{i=1}^{n}P(B|A_{i})P(A_{i})\quad \scriptsize{(S=\bigcup_{i=1}^{n}A_{i})}$$

>[!thm] Teorema di Bayes
>$$P(A|B)=\frac{P(B|A)\cdot P(A)}{P(B)}$$
>Estensione con $$\bigcup_{i=1}^{n}A_{i}=S$$
>$$P(A_{i}|B)=\frac{P(B|A_{i})\cdot P(A_{i})}{P(E)}=\frac{P(B|A_{i})\cdot P(A_{i})}{\sum_{j=1}^{n}P(E|A_{j}\cdot P(A_{j}))}$$

