Una funzione si trova nella forma di Bode quando
$$
G(s)=
\frac{k_{B}}{s^{g}}\cdot
\frac
  {\prod_{i=1}^{r_z}(1+\hat{\tau_{i}}\cdot s)}
  {\prod_{i=1}^{r_p}(1+\tau_{i}\cdot s)}
\frac
{\prod_{i=1}^{c_{z}}(1+2\cdot\frac{\hat\zeta_{i}}{\hat{\omega_{i}}}s+\frac{1}{\hat{\omega_{i}}^2}s^2)}
{\prod_{i=1}^{c_{z}}(1+2\cdot\frac{\zeta_{i}}{\omega_{i}}s+\frac{1}{\omega_{i}^{2}}s^2)}$$
dove 
- $k_{B}\in \mathbb{R}$ è il **guadagno di Bode**
- $s^{g}$, $g\in \mathbb{Z}$ è il **termine monomio**
  Se $g = 0$ allora il termine è ininfluente
  Se $g>0$ allora ci sono $g$ ha poli in $0$
  Se $g<0$ allora ci sono $g$ zeri in 0
- $1+\tau_{i}s$ è il **termine binomio**, $\tau_{i}\in \mathbb{R}$
  Ha singolarità in $s=\frac{-1}{\tau_{i}}$ 
- $1+2\cdot\frac{\zeta_{i}}{\omega_{i}}s+\frac{1}{\omega_{i}^{2}}s^2$ , $\omega_{i}>0$ è il **termine trinomio**.
  Se $|\zeta_{i}|<1$, allora le singolarità sono complesse.
