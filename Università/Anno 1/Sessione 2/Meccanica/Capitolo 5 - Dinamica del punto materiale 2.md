---
collegamenti:
  - "[[Capitolo 5 - Dinamica del punto materiale 1]]"
---
# Forza elastica
Si definisce forza elastica $$\vec{F_{e}}=-kx\vec{i}$$ con la legge di *Hooke*. Indica con quanta forza, la molla, rilancia il corpo indietro.
dove $\vec{i}$ è la direzione, $x$ la variazione di lunghezza prima e dopo l'impatto e $k$ la costante di rigidezza dell'elemento elastico $[\frac{N}{m}]$
$\vec{F}_{e}$ è negativo perchè il corpo immaginiamo che il corpo stia impattando su un molla in verso opposto all'asse delle $x$.

FARE PER BENE 
L'equazione delle $x$ è quella del [[Moto rettilineo#Moto armonico|moto armonico]].
$$x=A\sin(\omega t +\varphi)$$
$$\omega = \sqrt{\frac{k}{m}}$$
Il periodo $T$ è pari a
$$T=\frac{2\pi}{\omega}=2\pi\sqrt{\frac{m}{k}}$$
La frequenza sarà allora
$$f=\frac{1}{T}=\frac{1}{2\pi}\sqrt{\frac{k}{m}}$$
L'ampiezza $A$ e la fase $\varphi$ dipendono dalle condizioni iniziali $x_{0}$ e $v_{0}$
Ad esempio se il punto parte da una configurazione in cui la molla è deformata, con velocità nulla
$$x_{0}=x_{0}\qquad v_0=0=A\omega\cos\varphi$$
Risolvendo si ottiene $\varphi=0\quad A=x_{0}$

# Elementi flessibili
Per modellare elementi flessibili come fili, cavi, funi, catene, tendini, ecc., in meccanica solitamente si fanno le seguenti ipotesi. Gli elementi flessibili sono: 
- Inestensibili (la sua lunghezza non varia) 
- Perfettamente flessibili (possono applicare forze soltanto se sono tesi) 
- Massa trascurabile

Consideriamo un elemento flessibile mantenuto teso da due forse di trazione $\vec{F}_{a},\vec{F}_{b}$
Indichiamo con $\vec{T}$ la tensione della fune
Nel tratto iniziale, $\vec{F}_{a}+\vec{T}=m_{f}\vec{a}$
Dato che la massa è trascurabile, $\vec{F}_{a}=-\vec{T}$
Stessa cosa per il tratto finale $\vec{F}_{b}=-\vec{F}_{a}=\vec{T}$. 
Possiamo quindi dire che la tensione è costante.

Spesso gli elementi flessibili vengono avvolti intorno a supporti rigidi come carrucole, pulegge ecc...
Supponiamo il supporto sia fisso e che la fune possa scivolare senza attrito su di esso.

Supponiamo che la carrucola sia circolare ed analizziamo un tratto infinitesimo di fune. Ipotizziamo che il tratto sia un arco di circonferenza con angolo al centro $\alpha$.
Indichiamo con $\vec{T}_{1}$ e $\vec{T}_{2}$ le tensioni ai capi del tratto infinitesimo e con $\vec{N}$ la reazione vincolare della carrucola.

Allora, applicando [[Capitolo 5 - Dinamica del punto materiale 1#^ee9546|la seconda legge di netwon]]
$$ma_{t}=T_{2}\cos\frac{\alpha}{2}-T_{1}\cos(\frac{\alpha}{2})$$
e dato che la massa è trascurabile
$$T_{2}=T_{1}=T$$
Quindi vediamo che il modulo della tensione non varia lungo l'arco, cambia solo di direzione.

## Esempio 1 - La macchina di Atwood
Consideriamo due masse sospese tramite un'unica fune ideale che passa attraverso una carrucola di massa trascurabile.
Vogliamo determinare l'accelerazione delle due masse e la tensione della fune.

Possiamo applicare la seconda legge di Newton
$m_{1}a_{1} = m_{1}g -T$
$m_{2}a_{2}=m_{2}g-T$

Dato che la fune è inestensibile, risulta che 
$a_{2}=-a_{1}=-a$
Unendo le espressioni troviamo che
$$a=\frac{m_1-m_{2}}{m_{1}+m_{2}}g$$
La tensione della fune sarà
$$T=\frac{2m_1m_2}{m_{1}+m_{2}}g$$
## Esempio 2
Due punti di massa $m_{p}$ e $m_{q}$ sono collegati da un filo e vincolati a scorrere su una superficie priva di attrito.
 Al punto P è applicata una forza $\vec{F}=F\vec{i}$.
 Possiamo calcolare l'accelerazione dei due punti e la tensione del filo
Applicando la seconda legge di Newton
$$m_pa_p=F-T$$
$$m_qa_q=T$$
Dato che il filo è inestensibile risulta che 
$$a_{p}=a_{q}=a$$
Otteniamo, facendo un po' di calcoli, che 
>[!def] Accelerazione senza attrito
>$$a=\frac{F}{m_p+m_q}$$

^c30763

Sostituendo ottengo che 
$$T=\frac{m_{q}}{m_{p}+m_{q}}F$$
## Esempio 3
Analizziamo l'[[#Esempio 2]], supponendo però che tra i due corpi e il piano ci sia un attrito dinamico $\mu_{p}$ e $\mu_q$ rispettivamente.

Applichiamo ancora la seconda legge di Newton alle due masse, considerando però le forze di attrito.
$\vec{F}_{ap}=-\mu_{p}m_{p}g\vec{i}$ e $\vec{F}_{ap}=-\mu_{q}m_{q}g\vec{i}$
(vengono da [[Piano inclinato#^56587a]])
Allora
$m_{p}a_{p}=F-T-\mu_{p}m_{p}g$
$m_{q}a_{q}=T-\mu_{q}m_{q}g$

Essendo il filo inestensibile avremo che $a_{p}=a_{q}=a$

Sostituendo ed applicando i calcoli, si ottiene alla fine
>[!def] Accelerazione con attrito
>$$a=(F-(\mu_{p}m_{p}+\mu_{q}m_{q})g)\frac{1}{m_{p}{m}_{q}}$$
>Ricordiamoci che senza attrito avevamo [[#^c30763]]

## Esempio 4
Due punti materiali sono collegati da una fune inestensibile che passa su una carrucola di massa trascurabile. Il primo è sospeso verticalmente e il secondo scorre su una superficie orizzontale priva di attrito.
Vogliamo calcolare l'accelerazione dei due punti e la tensione nella fune.

Applicando la seconda legge di Newton ai due corpi, avremo
$m_{1}a_{1}=m_{1}g-T$
$m_{2}a_{2}=T-F_{a}$
Dato, come sempre, che $a_1=a_{2}=a$ dato che la fune è inestensibile, si ottiene

$$a=\frac{m_{1}g}{m_{1}+m_{2}}$$


# Pendolo semplice
![[Pendolo]]

# Momento di una forza
![[Momento di una forza]] ^daccc8
# Momento angolare della quantità di moto
![[Momento angolare della quantità di moto]]