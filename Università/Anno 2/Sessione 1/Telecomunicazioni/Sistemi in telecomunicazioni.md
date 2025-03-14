Si può riprendere tutto quello che è stato studiato in [[Università/Anno 2/Sessione 1/Sistemi dinamici/ARGOMENTI TRATTATI|ARGOMENTI TRATTATI|sistemi dinamici]]

>[!def] Sistema non dispersivo
>Un sistema si dice non dispersivo quando non ha memoria, l’uscita al tempo $t_{0}$ dipende solo dall’ingresso al tempo $t_{0}$
>La [[Risposta forzata#Risposta impulsiva|risposta impulsiva]] allora deve assumere la forma $h(t)=k\delta(t)$.
>Allora $y(t_{0})=kx(t_{0})$

>[!prp] Stabilità in senso ILUL(BIBO)
>Un sistema è stabile in senso ILUL se e solo se
>$$\int_{-\infty}^{\infty}|h(t)|dt<+\infty$$
>La risposta impulsiva deve essere assolutamente integrabille.

^1c640e

# Risposta a un segnale esponenziale complesso
Sistema [[Sistemi lineari tempoinvarianti|LTI]] caratterizzato da una [[Risposta forzata#Risposta impulsiva|risposta impulsiva]] $h(t)$
Dato l’ingresso $x(t)=Ae^{j(2\pi f_{0}t+\phi)}$
$$y(t)=\int_{-\infty}^{\infty}h(\tau)Ae^{j(2\pi f_{0}(t-\tau) + \phi)}d\tau=Ae^{j\phi} e^{j2\pi f_{0} t}\int_{-\infty}^{\infty}h(\tau)e^{-j2\pi f_{0}\tau} d\tau=A|H(f_{0})|e^{j(2\pi f_{0}t+\phi +\measuredangle H(f_{0}))}$$
dove $H(f_{0})=|H(f_{0})|e^{j\measuredangle H(f_{0})}= \int_{-\infty}^{\infty}h(\tau)e^{-j2\pi f_{0}\tau} d\tau$

Nota: simile a [[Teorema della risposta in frequenza#^a625cb]]

Possiamo quindi dire che la risposta di un sistema LTI a un ingresso esponenziale complesso è un esponenziale complesso alla stessa frequenza ma con ampiezza e fase variate, dipendenti dalla frequenza e dalla risposta impulsiva del sistema.