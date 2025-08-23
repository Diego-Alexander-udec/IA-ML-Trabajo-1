## A) NumPy – Creación y manipulación de arreglos

### Ejemplo 1: Crear un array
```python
import numpy as np
a = np.array([10, 20, 30])
print(a)
```
**Resultado:**
```
[10 20 30]
```
### Ejemplo 2: Usar reshape
```python
b = np.array([1, 2, 3, 4, 5, 6])
b_reshaped = b.reshape((2, 3))
print(b_reshaped)
```
**Resultado:**
```
[[1 2 3]
 [4 5 6]]
```
### Ejemplo 3: Concatenar arreglos
```python
import numpy as np
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
concatenado = np.concatenate((a, b))
print(concatenado)
```
**Resultado:**
```
[1 2 3 4 5 6]
```
