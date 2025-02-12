Nel calcolo computazionale, non è possibile raggiungere una precisione infinitesima data la limitatezza della memoria. 
Si commettono quindi necessariamente degli errori.

>[!def] Errore assoluto
>Data una grandezza $z$ ed una sua approssimazione $\tilde z$, definizamo l’errore assoluto come:
>$$\delta z=\tilde z-z$$ 

^0c317c

>[!def] Errore relativo
>Data una grandezza $z$ ed una sua approssimazione $\tilde z$, definizamo l’errore assoluto come:
>$$\epsilon_{z}=\frac{\tilde z-z}{z}$$

^0f475d

# Tipi di errori
>[!def] Errore inerente
Con l’errore inerente si intende quell’errore di misura o di rappresentazione dovuto al calcolatore.
$$\frac{f(x+\delta x)-f(x)}{f(x)}$$

>[!def] Errore analitico o di troncamento
Con l’errore di troncamento si intende quell’errore dovuto dall’approssimazione di $f$ in $g$.
$$\frac{g(x)-f(x)}{f(x)}$$

>[!def] Errore algoritmico
Con l’errore algoritmico si intende quell’errore dovuto all’esecuzione di uno specifico algoritmo su un calcolatore ottenendo invece di $g$, la sua approssimazione $\tilde g$.
$$\frac{\tilde g(x)-g(x)}{g(x)}$$

Alla fine, invece di $y = f(x)$ si ottiene $\tilde y = \tilde g(x+\delta x)$

# Condizionamento e stabilità
>[!def] Problema bencondizionato
>Un problema si dice bencondizionato se a piccole variazione sui dati corrispondono piccole variazioni sui risultati. 
>$$\left|\frac{f(x+\delta x)-f(x)}{f(x)}\right|\simeq \left |\frac{\delta x}{x}\right|=\epsilon_{x}$$
>La condizione vale esclusivamente dal problema e non dall’algoritmo utilizzato.
>Per piccole perturbazioni $\epsilon_{x}$, 
>$$\left|\frac{f(x+\epsilon_{x}x)-f(x)}{f(x)}\right|\simeq \frac{xf^{'}(x)}{f(x)}$$

>[!def] Algoritmo stabile
>Un algoritmo si dice stabile se amplifica poco (relativamente alle caratteristiche del calcolatore) gli errori di arrotondamento introdotti nelle singole operazioni.

[[Algoritmi]]

# Propagazione degli errori
Nella [[Aritmetica finita#Somma algebrica $ oplus$]] si ha una grande amplificazione degli errori sui dati quando si sommano numeri quasi uguali in modulo ma opposti di segno. (CANCELLAZIONE NUMERICA)

