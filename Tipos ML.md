# Tipos de Aprendizaje en Machine Learning

El aprendizaje en Machine Learning (ML) se produce mediante algoritmos que entrenan modelos capaces de distinguir datos y generar predicciones. Los algoritmos de ML se agrupan principalmente en tres tipos, según el modo en que reciben y procesan los datos de entrada:

- **Aprendizaje Supervisado**
- **Aprendizaje No Supervisado**
- **Aprendizaje por Refuerzo**

A continuación se explica cada tipo, con ejemplos claros para su comprensión.

---

## 1. Aprendizaje Supervisado

En el aprendizaje supervisado, los algoritmos trabajan con datos **etiquetados** (*labeled data*), es decir, datos que incluyen una etiqueta que los describe. El objetivo es encontrar una función que, a partir de las variables de entrada, asigne la etiqueta de salida adecuada. El modelo se entrena con un conjunto de datos históricos para desarrollar la capacidad de predecir la etiqueta de nuevos datos.

**Ejemplo:**  
> Un caso común es la clasificación de correos electrónicos como "spam" o "no spam".  
> - Se utiliza un conjunto de datos de correos electrónicos etiquetados (cada correo tiene una etiqueta: spam o no spam).
> - El modelo aprende los patrones en los correos y clasifica nuevos correos según esos patrones.

---

## 2. Aprendizaje No Supervisado

En el aprendizaje no supervisado, los algoritmos trabajan con datos **no etiquetados** (*unlabeled data*), es decir, datos que no cuentan con una etiqueta descriptiva. El objetivo es descubrir patrones o estructuras subyacentes en los datos, sin guía de etiquetas predefinidas. Se emplean técnicas como **agrupación** (*clustering*) o **reducción de dimensionalidad*. Es útil para segmentación de clientes, detección de anomalías y compresión de datos.

**Ejemplo:**  
> Segmentación de clientes en una empresa.  
> - Los datos de compras de los clientes no tienen etiquetas sobre su tipo.
> - Utilizando técnicas de agrupación, el algoritmo identifica grupos con comportamientos similares, ayudando a personalizar estrategias de marketing.

---

## 3. Aprendizaje por Refuerzo

El aprendizaje por refuerzo implica que los algoritmos aprenden a tomar decisiones mediante la **interacción con un entorno**. A diferencia de los anteriores, aquí se recibe retroalimentación en forma de **recompensas** o **castigos**. El objetivo es maximizar la recompensa acumulada, explorando diferentes acciones y aprendiendo de sus consecuencias. Se utiliza en juegos, robótica y sistemas de recomendación.

**Ejemplo:**  
> Un agente que juega a un videojuego.  
> - Recibe recompensas por acciones positivas (ganar puntos) y castigos por acciones negativas (perder vidas).
> - A través de la exploración y la retroalimentación, el agente aprende a tomar decisiones que maximizan su puntuación.

---

## Resumen Visual

| Tipo de ML             | Datos de entrada | Objetivo principal         | Ejemplo                                           |
|------------------------|------------------|---------------------------|---------------------------------------------------|
| Supervisado            | Etiquetados      | Predecir/Clasificar datos | Clasificación de spam                             |
| No Supervisado         | No etiquetados   | Encontrar patrones        | Agrupación de clientes                            |
| Por Refuerzo           | Interacción      | Maximizar recompensa      | Aprender a jugar un videojuego                    |

---

**Referencias:**  
- [Machine Learning Basics - Scikit-learn](https://scikit-learn.org/stable/tutorial/basic/tutorial.html)
- [Tipos de aprendizaje en ML - Wikipedia](https://es.wikipedia.org/wiki/Aprendizaje_autom%C3%A1tico)
