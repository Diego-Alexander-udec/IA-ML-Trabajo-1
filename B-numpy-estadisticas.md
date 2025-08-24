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
###Ejemplo 3: Generar números aleatorios
```python
aleatorios = np.random.rand(3, 2)
print(aleatorios)
```
**Resultado:**
```
[[0.93912605 0.69946397]
 [0.39729219 0.20085467]
 [0.60398808 0.71203604]]
```
###Ejemplo 4: Producto matricial y determinante
```python
A = np.array([[1, 2], [3, 4]])
B = np.array([[2, 0], [1, 2]])
producto = np.dot(A, B)
det_A = np.linalg.det(A)
print("Producto matricial:\n", producto)
print("Determinante de A:", det_A)
```
**Resultado:**
```
Producto matricial:
 [[ 4  4]
 [10  8]]
Determinante de A: -2.0000000000000004
```