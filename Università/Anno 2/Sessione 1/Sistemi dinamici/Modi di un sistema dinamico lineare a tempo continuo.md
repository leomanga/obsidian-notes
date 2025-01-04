I modi sono le funzioni caratteristiche di ogni sistema lineare [[Sistemi lineari tempoinvarianti|LTI]].

# Modi aperiodici
![[Segnali esponenziali#^4cdd45]]
(Quando i poli sono reali e la molteplicità dei poli è uguale a 1)

# Modi pseudoperiodici
Una combinazione fra [[Segnali esponenziali]] e [[Segnali sinusoidali]].
$$e^{\sigma t}\cos({\omega t})\cdot \mathbb{1}(t)\mbox{ e } e^{\sigma t}\sin({\omega t})\cdot \mathbb{1}(t)$$
$\sigma$ è la parte reale e $\omega$ è la parte complessa
(Quando i poli hanno parte reale e complessa e la molteplicità dei poli è uguale a 1)
# Modi aperiodici
$$e^{pt}\mathbb{1}(t),\   te^{pt}\mathbb{1}(t),\ t^{2}e^{pt}\mathbb{1}(t) \ldots,t^{\mu - 1} e^{pt}\mathbb{1}(t)$$
dove $\mu$ è la molteplicità, maggiore di 1 e $p\in \mathbb{R}$ è un polo

# Modi completi
$$e^{\sigma t}\cos(\omega t)\mathbb{1}(t),\   te^{\sigma t}\cos(\omega t)\mathbb{1}(t),\ t^{2}e^{\sigma t}\cos(\omega t)\mathbb{1}(t) \ldots,t^{\mu - 1} e^{\sigma t}\cos(\omega t)\mathbb{1}(t)$$
$$e^{\sigma t}\sin(\omega t)\mathbb{1}(t),\   te^{\sigma t}\sin(\omega t)\mathbb{1}(t),\ t^{2}e^{\sigma t}\sin(\omega t)\mathbb{1}(t) \ldots,t^{\mu - 1} e^{\sigma t}\sin(\omega t)\mathbb{1}(t)$$
dove $\sigma$ è la parte reale e $\omega$ la parte complessa del polo.
(Quando i poli hanno parte reale e complessa e la molteplicità è maggiore di 1)

# Caratteristiche di convergenza dei modi
$m(t)$ è un modo generico
## Convergenti
Un modo è convergente se $\lim_{t\to \infty}m(t)=0$
Questo avviene se la parte reale è **negativa**.
## Limitati non convergenti
Un modo è limitato non convergente se non è [[#Convergenti|convergente]] ed $\exists M > 0 : \forall t\ge 0, |m(t)|<M$
Questo avviene quando la parte reale è **uguale a 0** e la molteplicità è 1. (sono i casi [[#Modi aperiodici]] e [[#Modi pseudoperiodici]])
## Divergenti
Questo avviene **per i poli a molteplicità 1**, se hanno **parte reale maggiore di 0**, **per gli altri** se la **parte reale è maggiore o uguale a 0.**
