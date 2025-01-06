L’idea è quella di scegliere un ingresso $u(k)$ in base allo stato $x(k)$.
Ho quindi bisogno di conoscere le variabili di stato.

Dato il sistema [[Sistemi lineari tempoinvarianti|LTI]] a tempo discreto
$$\begin{cases}x(k+1)=Ax(k)+Bu(k)\\y(k)=Cx(k)+Du(k)\end{cases}$$

Sceglieremo $u$ come combinazione lineare delle variabili di stato.
$$u(k)=Fx(k)+r(k)$$
Dove $F\in \mathbb{R}^{m\times n}$ e $r$ è il segnale di riferimento.

![[Controllo in retroazione.excalidraw]]

Sostituendo avremo $$x(k+1)=(A+BF)x(k)+Br(k)$$
>[!prp]
>Se e solo se il sistema è [[Raggiungibilità di un sistema dinamico#^04bbfd|completamente raggiungibile]] allora $\forall\ n-pla$ di [[Autovettori - autovalori - autospazi|autovalori]] $\bar\lambda_{1},\bar\lambda_{2},\ldots,\bar\lambda_{n}$, $\exists F$ tale che $$det(zI-(A+BF))=(\lambda-\bar\lambda_1)(\lambda-\bar\lambda_2)\ldots(\lambda-\bar\lambda_n)$$

Se il sistema non fosse completamente raggiungibile devo fare la [[Decomposizione di raggiungibilità]] ed avrò la possibilità di modificare solo la parte raggiungibile dato che 
$$\bar A+\bar B\bar F=\begin{bmatrix}A_{r}+B_{r}\bar F_{r}&A_{r\bar r}+B_{r}\bar F_{\bar r}\\0&A_{\bar r}\end{bmatrix}$$
#da-finire pg 129

>[!def] Forma canonica di controllo

#da-finire pg 132

