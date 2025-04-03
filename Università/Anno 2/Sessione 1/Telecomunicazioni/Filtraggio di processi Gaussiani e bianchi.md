Considerando un filtro [[Segnali passa-basso e passa-banda#^144169|passa banda]] ideale, allora l’uscita sarà un processo aleatorio passa-banda del tipo
$$X(t)=X_{c}(t)\cos(2\pi f_{c}t)-X_{s}(t)\sin(2\pi f_{c}t)$$
$X_c$ è la componente in fase e $X_s$ in quadratura

Nel caso di processo bianco e gaussiano avremo che
- $X_{c}(t)$ e $X_{s}(t)$ sono a media nulla, congiuntamente stazionari e congiuntamente Gaussiani
- $P_{X}=P_{X_{c}}=P_{X_s}=\int_{-\infty}^{\infty}S_{X}(f)df$
- $S_{X_{1c}}(f)=S_{X_{1s}}(f)=\begin{cases}N_{0}\quad |f|\le W\\ 0\quad \mbox{altrimenti}\end{cases}$, $X_{1c}(t)$ e $X_{1s}(t)$ sono processi indipendenti.
Nel caso di un filtro passa-banda non simmetrico rispetto a $f_{c}$
- $S_{X_{2}}(f)=\begin{cases}\frac{N_{0}}{2}\quad f_{c}\le |f|\le f_{c}+W\\ 0\quad \mbox{altrimenti}\end{cases}$
- $X_{2c}(t)$ e $X_{2s}(t)$ sono a media nulla, congiuntamente stazionari e Gaussiani
- $P_{X_2}=P_{X_{2c}}=P_{X_{2s}}=\int_{-\infty}^{\infty}S_{X_2}(f)df$
- $X_{2c}(t)$ e $X_{2s}(t)$ non sono indipendenti
