Partiamo da un segnale informativo analogico [[Segnali passa-basso e passa-banda|passa-basso]] $m(t)$.

Questo segnale può essere trasmesso su un canale di comunicazione tramite modulazione analogica di portante.
La trasmissione può avvenire inserendo l'informazione presente nel segnale modulante $m(t)$ nell’ampiezza, nella frequenza o nella fase di una portante sinusoidale.

La frequenza $f_c$ della portante sinusoidale dovrà essere sufficientemente alta da rendere adatta ed efficiente la trasmissione del segnale modulato sul canale di comunicazione, tenendo conto della larghezza di banda del segnale $m(t)$.

# Modulazione analogica
Il segnale analogico da trasmettere è $m(t)$, è passa-basso con banda $W$, ovvero $M(f)=0$ per $|f|>W$.
Avremo che la [[Segnali#^5a2215]]
$$P_{m}=\lim_{T\to \infty}\frac{1}{T}\int_{\frac{-T}{2}}^{\frac{T}{2}}|m(t)|^{2}dt$$
Avremo inoltre $c(t)$ la portante su cui imprimere il segnale modulante $m(t)$.
$$c(t)=A_{c}\cos(2\pi f_{c}t +\phi_{c})$$
I nostri obiettivi sono:
1) Traslare la frequenza del segnale modulante in modo che il segnale modulato sia un segnale passa-banda adatto alle caratteristiche del segnale.
2) Rendere possibile la trasmissione nello spazio libero con antenne di dimensioni ragionevoli.
3) Trasmettere simultaneamente più segnali $m_{i}(t), i=1,\ldots,N$ sullo stesso canale con tecniche di multiplexing a divisione di frequenza.
4) Espandere la banda del segnale per ridurre gli effetti negativi della trasmissione su canali rumorosi. (Gli obiettivi 1-3 sono possibili solo con la modulazione di ampiezza)

[[Modulazione di ampiezza]]

# Modulazione digitale
Studieremo le modulazioni digitali in canali affetti da disturbo [[AWGN]].
Questo modello è adatto alle linee cablate e ad alcuni canali radio.

Nella fase della modulazione digitale, si associa ad $M$ simboli digitali, un segnale analogico, così da poter essere trasmesso.
$$m\iff S_{m}(t), \quad m=1,\ldots, M$$
Ricordando che il rumore AWGN è additivo, avremo che nel canale avremo un segnale del tipo
$$\mathbb{r}(t)=S_{m}(t)+\mathbb{n}(t)$$
dove $\mathbb{n}(t)$ è il rumore.