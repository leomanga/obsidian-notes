# Il valore temporale del denaro
Il denaro ha un valore diverso nel tempo, un euro oggi vale più di un euro tra un anno.
Questo è dovuto dal fatto che oggi potrei investire l’euro ed ottenere un profitto.

>[!note] Nomenclatura e definizioni
>$VA$ → valore attuale, indica la quantità di denaro oggi.
>$C_{t}$ → ammontare di denaro al periodo $t$.
>$r,i$ → tasso di rendimento o di interesse su base annua
>$(1+r)$ → fattore di capitalizzazione
>$FA$ → fattore di attualizzazione, permette di convertire un ammontare di denaro futuro ad oggi. 
 >$\qquad VA = FA \cdot C_{t}\qquad FA = \frac{1}{(1+r)^{t}}$
 >$VAN$ → valore attuale netto. $VAN = C_{0}+ VA(C_{0}<0)$ 

^1b2fe3

 
Il [[Costo opportunità]] di un investimento in un progetto è il tasso di rendimento atteso richiesto dagli investitori per un investimento che abbia lo stesso rischio del progetto.

# TAN, TAEG, ISC
[[Tasso annuale netto(TAN)]]
[[Tasso annuale effettivo grezzo(TAEG)]]

# Rendita perpetua
Una rendita perpetua è un flusso di cassa costante in eterno.
$C$ è il flusso di cassa costante in eterno.
$$VA = \frac{C}{1+r}+\frac{C}{(1+r)^{2}+\ldots+\frac{C}{(1+r)^{\infty}}}= \sum^{\infty}_{t=1}{\frac{C}{(1+r)^{t}}}=\frac{C}{r}$$
# Rendita annua
Praticamente come la rendita perpetua ma fino ad un tempo $t$.
Basta sottrarre alla rendita perpetua la rendita da $t+1 \mbox{ fino a } \infty$.
$$
VA = \frac{C}{r}- \frac{C}{r(1+t)^{t}} = C\frac{(1+r)^{t}-1}{r(1+r)^{t}}
$$

^2511d3

# Calcolo del valore futuro
Immaginiamo di ricavare il valore futuro $F_{t}$ di una serie di pagamenti dall’anno 1 all’anno t.
Da $F_{t}=VA \cdot (1+r)^{t}$ e [[#^2511d3]], avremo
$$F_{t}=C\frac{(1+r)^{t}-1}{r(1+r)^{t}} \cdot (1+r)^{t}= C\frac{(1+r)^{t}-1}{r}$$
# Euro correnti e costanti
- **Euro correnti(nominali)**: Sono i valori relativi ad importi(flussi di cassa) nel momento in cui si verificano
- **Euro costanti(reali):** Sono i valori basati sul potere di acquisto. Sono depurati dall’inflazione. $\mbox{Euro reale} = (\frac{\mbox{Euro nominale}}{1+\mbox{tasso di inflazione}})^{t}$
# Tassi di interesse nominali e reali
- **Tasso di interesse nominale**: Tasso di crescita del valore di un investimento
- **Tasso di interesse reale**: Tasso di crescita del potere di acquisto di un investimento. $(1+\mbox{tasso di interesse reale})=\frac{1+\mbox{ tasso di interesse nominale}}{1+\mbox{inflazione}}$ 
# Mutuo
[[Mutuo]]

# Obbligazioni
[[Obbligazioni]]