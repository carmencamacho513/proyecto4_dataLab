# Hito 3. Regresión Logística

#### Se importa dataframe de BigQuery donde se relizó las variables Dummies.

### OPRIME <mark style="color:red;">**Colab Colaboratory**</mark> Se relaciona todos los cálculos realizados.

{% embed url="https://colab.research.google.com/drive/1yuv6CUyHP60Vgmr6KklY2k4odh8SbLi-#scrollTo=iEuAhOzVehUz" %}

### Conclusiones

Explicación del resultado de la regresión logística:

1. **Accuracy (Exactitud):** 0.8104
   * La exactitud representa la proporción de predicciones correctas en el conjunto de datos de prueba. En este caso, el modelo tiene una exactitud del 81.04%, lo que significa que acierta en la clasificación del 81.04% de las instancias.
2. **Confusion Matrix (Matriz de Confusión):**
   * La matriz de confusión muestra la distribución de las predicciones del modelo en comparación con los valores reales.
   * Verdaderos positivos (TP): 10,550
   * Falsos positivos (FP): 5,584
   * Verdaderos negativos (TN): 76,783
   * Falsos negativos (FN): 14,851
3. **Classification Report (Informe de Clasificación):**
   * **Precision (Precisión):**
     * Para la clase 0 (sin ARR\_DELAY): 0.84
     * Para la clase 1 (con ARR\_DELAY): 0.65
     * La precisión mide la proporción de instancias positivas correctamente clasificadas entre todas las instancias clasificadas como positivas.
   * **Recall (Sensibilidad):**
     * Para la clase 0: 0.93
     * Para la clase 1: 0.42
     * El recall mide la proporción de instancias positivas correctamente clasificadas en relación con todas las instancias que realmente son positivas.
   * **F1-score (Puntuación F1):**
     * Para la clase 0: 0.88
     * Para la clase 1: 0.51
     * La puntuación F1 es una métrica que combina precisión y recall en un solo valor. Es especialmente útil cuando hay un desequilibrio en las clases.
   * **Support (Soporte):**
     * Para la clase 0: 82,367
     * Para la clase 1: 25,401
     * El soporte indica la cantidad de instancias de cada clase en el conjunto de datos de prueba.

El modelo tiene un rendimiento razonablemente bueno en la clasificación de las instancias sin ARR\_DELAY (clase 0), pero tiene un recall más bajo para las instancias con ARR\_DELAY (clase 1), lo que indica que puede haber dificultades para identificar correctamente todas las observaciones positivas.

### OPRIME <mark style="color:red;">En conceptos Obtenidos en el Proceso</mark> encuentras la definición de la Regresión Logística.

{% content-ref url="../../conceptos-obtenidos-en-el-proceso-proyecto-4-datalab.md" %}
[conceptos-obtenidos-en-el-proceso-proyecto-4-datalab.md](../../conceptos-obtenidos-en-el-proceso-proyecto-4-datalab.md)
{% endcontent-ref %}

