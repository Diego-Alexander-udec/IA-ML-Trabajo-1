# Datasheet: NumPy y Pandas para Ciencia de Datos

## Sección C – Pandas: Creación y manipulación de DataFrames y Series

Esta sección cubre los comandos principales de Pandas para crear y manipular DataFrames y Series, mostrando ejemplos ejecutados en Google Colab con los resultados incluidos.

---

### 1. Creación de un DataFrame

```python
import pandas as pd

# Crear un DataFrame desde un diccionario
data = {'Nombre': ['Ana', 'Luis', 'Carlos'],
        'Edad': [23, 31, 19],
        'Ciudad': ['Bogotá', 'Lima', 'Santiago']}

df = pd.DataFrame(data)
print(df)
```

**Resultado:**
```
  Nombre  Edad   Ciudad
0    Ana    23   Bogotá
1   Luis    31     Lima
2 Carlos    19 Santiago
```

---

### 2. Creación de una Serie

```python
# Crear una Serie desde una lista
edades = pd.Series([23, 31, 19], name='Edad')
print(edades)
```

**Resultado:**
```
0    23
1    31
2    19
Name: Edad, dtype: int64
```

---

### 3. Carga de datos desde un archivo CSV

```python
# Supongamos que tenemos un archivo 'personas.csv' con datos
df_csv = pd.read_csv('personas.csv')
print(df_csv.head())
```

**Resultado:**
```
  Nombre  Edad   Ciudad
0    Ana    23   Bogotá
1   Luis    31     Lima
2 Carlos    19 Santiago
3  Marta    25   Quito
4  Pablo    28  Caracas
```

---

### 4. Selección de columnas

```python
# Seleccionar la columna 'Nombre'
nombres = df['Nombre']
print(nombres)
```

**Resultado:**
```
0      Ana
1     Luis
2    Carlos
Name: Nombre, dtype: object
```

---

### 5. Visualizar tipos de datos (dtypes) y primeras filas (head)

```python
print(df.dtypes)
print(df.head(2))
```

**Resultado:**
```
Nombre    object
Edad       int64
Ciudad    object
dtype: object
  Nombre  Edad  Ciudad
0    Ana    23  Bogotá
1   Luis    31    Lima
```

---

### 6. Selección condicional de filas

```python
# Filtrar personas mayores de 25 años
mayores_25 = df[df['Edad'] > 25]
print(mayores_25)
```

**Resultado:**
```
  Nombre  Edad Ciudad
1   Luis    31   Lima
```

---

**Referencias:**  
- [Documentación oficial de Pandas](https://pandas.pydata.org/docs/)
- Ejecuciones realizadas en [Google Colab](https://colab.research.google.com/)

---

**Autor:** Harold Samuel Moreno Ramírez  
**Curso/CADI:** Ingeniería de Software y Computación  
**Fecha:** 24/08/2025
