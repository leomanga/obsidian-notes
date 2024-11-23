---
pagina: 261
collegamenti:
  - "[[Kernel di una funzione lineare|Kernel]]"
---
Siano $\varphi: V\to W$ , $\psi:W\to U$ [[Trasformazione lineare|funzioni lineari]]
$\psi \circ \varphi:V\to W$ [[Trasformazione lineare|funzione lineare]]
### Iniettività
$$\psi \circ \varphi\mbox{ è iniettiva} \iff \begin{cases}\varphi \mbox{ iniettiva} \\ker(\psi)\cap Im(\varphi) = 0\end{cases}$$
### Suriettività
$$\psi \circ \varphi\mbox{ è suriettiva} \iff \begin{cases}\psi \mbox{ suriettiva} \\ker(\psi)+ Im(\varphi) = W\end{cases}$$
### Invertibilità
$$\psi \circ \varphi\mbox{ è invertibile} \iff \begin{cases}\varphi \mbox{ iniettiva}\\\psi \mbox{ suriettiva} \\ker(\psi)\oplus Im(\varphi) = W\end{cases}$$