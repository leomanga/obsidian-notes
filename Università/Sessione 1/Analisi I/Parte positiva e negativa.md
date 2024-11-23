# Parte positiva
Si indica con $x^+= max(x,0)$
```functionplot
---
title: Parte positiva
xLabel: 
yLabel: 
bounds: [-10,10,-10,10]
disableZoom: false
grid: true
---
y = max(x,0)
```

# Parte negativa
Si indica con $x^-= - min(x,0)$

```functionplot
---
title: Parte negativa
xLabel: 
yLabel: 
bounds: [-10,10,-10,10]
disableZoom: false
grid: true
---
y = - min(x,0)
```
# Valore assoluto
Il valore assoluto si indica con $|x| = x^{+}+x^{-}$
```functionplot
---
title: Valore assoluto
xLabel: 
yLabel: 
bounds: [-10,10,-10,10]
disableZoom: false
grid: true
---
y = max(x,0) - min(x,0)
```
# Rappresentazione di x con le due parti positiva e negativa
$$x = x^{+} - x^-$$
```functionplot
---
title: X
xLabel: 
yLabel: 
bounds: [-10,10,-10,10]
disableZoom: false
grid: true
---
y = max(x,0) + min(x,0)
```