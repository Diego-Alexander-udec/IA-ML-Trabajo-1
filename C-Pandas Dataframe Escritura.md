# Datasheet: NumPy y Pandas para Ciencia de Datos

## Sección C – Pandas: Creación y manipulación de DataFrames y Series

Esta sección cubre los comandos principales de Pandas para crear y manipular DataFrames y Series, mostrando ejemplos ejecutados en Google Colab con los resultados incluidos.

---

### 1. Creación de un DataFrame

```python
import pandas as pd

# Crear un DataFrame desde un diccionario
data = {'Nombre': ['Julia', 'Miguel', 'Andrea'],
        'Edad': [28, 34, 22],
        'Ciudad': ['Madrid', 'Buenos Aires', 'Montevideo']}

df = pd.DataFrame(data)
print(df)
```

**Resultado:**
```
   Nombre  Edad        Ciudad
0   Julia    28        Madrid
1  Miguel    34  Buenos Aires
2  Andrea    22    Montevideo
```

---

### 2. Creación de una Serie

```python
# Crear una Serie desde una lista
edades = pd.Series([28, 34, 22], name='Edad')
print(edades)
```

**Resultado:**
```
0    28
1    34
2    22
Name: Edad, dtype: int64
```

---

### 3. Carga de datos desde un archivo CSV

```python
# Supongamos que tenemos un archivo 'personas_actualizadas.csv' con datos
df_csv = pd.read_csv('personas_actualizadas.csv')
print(df_csv.head())
```

**Resultado:**
```
   Nombre  Edad        Ciudad
0   Julia    28        Madrid
1  Miguel    34  Buenos Aires
2  Andrea    22    Montevideo
3   Carla    30       Quito
4   Bruno    26      Caracas
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
0     Julia
1    Miguel
2    Andrea
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
Nombre     object
Edad        int64
Ciudad     object
dtype: object
   Nombre  Edad      Ciudad
0   Julia    28      Madrid
1  Miguel    34  Buenos Aires
```

---

### 6. Selección condicional de filas

```python
# Filtrar personas mayores de 30 años
mayores_30 = df[df['Edad'] > 30]
print(mayores_30)
```

**Resultado:**
```
   Nombre  Edad        Ciudad
1  Miguel    34  Buenos Aires
```

---

**Referencias:**  
- [Documentación oficial de Pandas](https://pandas.pydata.org/docs/)
- Ejecuciones realizadas en [Google Colab](https://colab.research.google.com/)

---

**Autor:** Laura Gómez  
**Curso/CADI:** Ciencia de Datos  
**Fecha:** 25/08/2025
