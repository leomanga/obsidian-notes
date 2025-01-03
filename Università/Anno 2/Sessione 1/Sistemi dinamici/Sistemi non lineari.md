Nei sistemi non lineari non possiamo applicare il principio della sovrapposizione degli effetti.
Inoltre, non sempre è possibile esprimere la funzione esplicita con le funzioni elementari.

Rappresentazione i/s/o di un sistema non lineare a tempo continuo
$$\begin{cases} \dot{x}(t)=f(x(t),u(t),t)\\
y(t)=h(x(t),u(t),t) \\
x(0)=x_{0}
 \end{cases}
$$

^c46d8f

Rappresentazione i/s/o di un sistema non lineare a tempo discreto
$$\begin{cases} x(k+1)=f(x(k),u(k),k)\\
y(k)=h(x(k),u(k),k) \\
x(0)=x_{0}
 \end{cases}
$$

Gran parte delle tecniche sui sistemi non lineari si basa su quelli lineari, cercando di sfruttare delle approssimazioni.
[[Tecniche di linearizzazione dei sistemi dinamici non lineari]]