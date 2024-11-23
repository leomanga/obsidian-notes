---
pagina: 272
collegamenti:
  - "[[Matrice elementare di Jordan o blocco di Jordan]]"
---

# Definizione
Una matrice quadrata di ordine $n$ è in FORMA DI JORDAN o MATRICE DI JORDAN se è una matrice diagonale a blocchi e ogni blocco è una [[Matrice elementare di Jordan o blocco di Jordan]].

# Proprietà
pg 291
Sia $\varphi:V_n(\mathbb{K})\to V_n(\mathbb{K})$ una [[Trasformazione lineare|funzione lineare]]
Sia $a$ l'unico [[Autovettori - autovalori - autospazi|autovalore]] di $\varphi$ tale che $ma(a) = n$, $mg(a)=p$
- $p$ rappresenta il numero di blocchi che saranno presenti nella matrice di Jordan.

### Procedimento per calcolare la grandezza dei blocchi
Sia $d_1=mg(a)$
1) $rank(M-aI)=n-d_{1}$
2) $rank(M-aI)^2=rank((M-aI)\circ(M-aI))=n-d_1-d_2$ (Si aggiunge $d_2$ perchè $rank(M-aI)^2$ è più piccolo di $rank(M-aI)=n-d_{1}$) 
3) Si continua finchè non esiste un $h$ tale che $d_{h+1}=d_{h+2}=0$

Il numero di blocchi di Jordan di grandezza 1 sarà uguale a $d1-d2$
Il numero di blocchi di Jordan di grandezza 2 sarà uguale a $d_2-d_3$
Così via....
