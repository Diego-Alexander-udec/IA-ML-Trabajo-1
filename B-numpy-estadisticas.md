# B) NumPy – Operaciones estadísticas y funciones avanzadas

###Ejemplo 1: Calcular media, desviación estándar y suma
```python
import numpy as np
datos = np.array([5, 10, 15, 20, 25])
print("Media:", np.mean(datos))
print("Desviación estándar:", np.std(datos))
print("Suma:", np.sum(datos))
```
**Resultado:**
```
Media: 15.0
Desviación estándar: 7.0710678118654755
Suma: 75
```
###Ejemplo 2: Usar arange y linspace
```python
print("Arange:", np.arange(0, 10, 2))
print("Linspace:", np.linspace(0, 1, 5))
```
**Resultado:**
```
Arange: [0 2 4 6 8]
Linspace: [0.   0.25 0.5  0.75 1.  ]
```