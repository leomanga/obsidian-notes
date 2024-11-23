>[!thm] Dini 1
>Sia $F:A\subseteq \mathbb{R}^{2}\to \mathbb{R}$
>Supponiamo $F\in C^{1}(A)$ e consideriamo l'insieme
>$$\Gamma=\{(x,y)\in A:F(x,y)=0\}$$
>Sia $(x_{0},y_{0})\in \Gamma(\iff ((x_{0},y_{0})\in A:F(x_{0},y_{0})=0)$ e supponiamo che $$\frac{\partial F}{\partial y}(x_{0},y_{0})\not =0$$
>### Parte 1
>Allora $\exists$ un intorno $I$ di $x_{0}$ e un intorno $J$ di $y_{0}$ tali che
>$$\forall x\in I, \exists!\ y\in J:F(x,y)=0$$
>Quindi ponendo $y=g(x)$ possiamo trovare una funzione $g:I\to J$ tale che $\forall x\in I, F(x,g(x))=0$
>Inoltre $g:I\to J$ è di [[Classi di funzioni#^08c68a|$C^1(I)$]] e soddisfa
>$$g^{'}(x)=-\frac{\frac{\partial F}{\partial x}(x,g(x))}{\frac{\partial F}{\partial y}(x,g(x))}\quad \forall x\in I$$
>### Parte 2
>Allora $\exists$ un intorno $I$ di $x_{0}$ e un intorno $J$ di $y_{0}$ tali che
>$$\forall y\in J, \exists!\ x\in I:F(x,y)=0$$
>Quindi ponendo $x=g(y)$ possiamo trovare una funzione $g:J\to I$ tale che $\forall y\in J, F(g(y),y)=0$
>Inoltre $g:J\to I$ è di [[Classi di funzioni#^08c68a|$C^1(I)$]] e soddisfa
>$$g^{'}(x)=-\frac{\frac{\partial F}{\partial y}(g(y),y)}{\frac{\partial F}{\partial x}(g(y),y)}\quad \forall x\in I$$
>---
>Dimostrazione a pag 6 argomenti5c

>[!thm] Dini 2
>Supponiamo $A\subseteq \mathbb{R}^{3}$ aperto e sia $(x_{0},y_{0},z_{0})\in A$.
>Sia $F:A\to \mathbb{R}$ tale che sia di classe $C^{1}(A)$ e $F(x_{0},y_{0},z_{0})=0$.
>Se $$\frac{\partial F}{\partial z}(x_{0},y_{0},z_{0})\not = 0$$
>Allora $\exists$ un intorno di $(x_{0},y_{0}, z_{0})$ della forma $I\times J\times H$ dove $I=(x_{0}-\delta,x_{0}+\delta), J=(y_{0}-\eta,y_{0}+\eta), H=(z_{0}-h,z_{0}+h)$ tale che  $$\forall (x,y)\in I\times J\ \exists !\ z\in H: F(x,y,z)=0$$
>Denotando con $z=g(x,y)$ risulta che $g:I\times J\to H$ è di classe $C^{1}([I\times J])$ e $\forall(x,y)\in I\times J$ si ha
>$$\frac{\partial g}{\partial x}(x,y)=-\frac{\frac{\partial F}{\partial x}(x,y,g(x,y))}{\frac{\partial F}{\partial z}(x,y,g(x,y))}$$
>$$\frac{\partial g}{\partial y}(x,y)=-\frac{\frac{\partial F}{\partial y}(x,y,g(x,y))}{\frac{\partial F}{\partial z}(x,y,g(x,y))}$$
>Il teorema vale anche scambiando il ruolo di $x$, $y$ e $z$.
>

 >[!thm]
 >Se $S=\{F(x,y,z)=0\}$ e $(x_{0},y_{0},z_{0})\in \Gamma$ con $$\frac{\partial F}{\partial z}(x_{0},y_{0},z_{0})\not = 0\Rightarrow \nabla F(x_{0},y_{0})\perp \Gamma$$

  guarda spiegazioni a pag 16-17-18. Si capisce molto bene.
  Arriviamo anche a dire che il gradiente di $F$ è parallelo al gradiente di $f$.
  Possiamo allora enunciare il seguente teorema

>[!thm] Moltiplicatori di Lagrange
>Supponiamo $A\subseteq \mathbb{R}^{3}$ e $S=\{F(x,y,z)=0\}$ e supponiamo che $\nabla F(x,y,z)\not = 0\ \forall (x,y,z)\in S$ dove $F\in C^{1}(A)$. Se $f:A\to \mathbb{R}$ è di classe $C^{1}(A)$, allora condizione necessaria affinchè $f$ ammetta un massimo o un minimo relativo su $S$ nel punto $(x_{0},y_{0},z_{0})$ è che esista $\lambda\in \mathbb{R}$ tale che 
>$$\begin{cases}
>\frac{\partial f}{\partial x}(x_{0},y_{0},z_{0})=\lambda \frac{\partial F}{\partial x}(x_{0},y_{0},z_{0})\\
>\frac{\partial f}{\partial y}(x_{0},y_{0},z_{0})=\lambda \frac{\partial F}{\partial y}(x_{0},y_{0},z_{0})\\
>\frac{\partial f}{\partial z}(x_{0},y_{0},z_{0})=\lambda \frac{\partial F}{\partial z}(x_{0},y_{0},z_{0})\\
>F(x_{0},y_{0},z_{0})=0
>\end{cases}$$
>Similmente se $F:A\subseteq \mathbb{R}^{2}\to \mathbb{R}$

^ffc5a3

