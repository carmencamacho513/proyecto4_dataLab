# Correlaciones-Prueba t de Student y Regresión Logística

### OPRIME <mark style="color:red;">**Colab Colaboratory**</mark> Se relaciona todos los cálculos realizados.

{% embed url="https://colab.research.google.com/drive/1yuv6CUyHP60Vgmr6KklY2k4odh8SbLi-#scrollTo=5H1bgEM0vbo-&line=1&uniqifier=1" %}

### Conclusiones&#x20;

**Correlación:**

La matriz de correlación muestra la relación entre diferentes variables en tu conjunto de datos:

1. **DEP\_DELAY y ARR\_DELAY:**
   * **Correlación:** 0.9401
   * **Interpretación:** Existe una correlación positiva fuerte (0.9401) entre el tiempo de retraso en la salida (DEP\_DELAY) y el tiempo de retraso en la llegada (ARR\_DELAY). Esto significa que los vuelos con retrasos en la salida tienden a tener también retrasos en la llegada.
2. **DEP\_DELAY y ELAPSED\_DELAY:**
   * **Correlación:** -0.0351
   * **Interpretación:** Hay una correlación débil negativa (-0.0351) entre el tiempo de retraso en la salida (DEP\_DELAY) y el tiempo total de vuelo (ELAPSED\_DELAY). Esto sugiere que, en general, los retrasos en la salida no están fuertemente relacionados con el tiempo total de vuelo.
3. **DEP\_DELAY y CANCELLED:**
   * **Correlación:** 0.0083
   * **Interpretación:** Hay una correlación muy débil positiva (0.0083) entre el tiempo de retraso en la salida (DEP\_DELAY) y la variable binaria que indica si un vuelo fue cancelado (CANCELLED). Esto sugiere que, en general, los retrasos en la salida no están fuertemente relacionados con la probabilidad de cancelación del vuelo.
4. **ARR\_DELAY y ELAPSED\_DELAY:**
   * **Correlación:** -0.3586
   * **Interpretación:** Existe una correlación moderada negativa (-0.3586) entre el tiempo de retraso en la llegada (ARR\_DELAY) y el tiempo total de vuelo (ELAPSED\_DELAY). Esto indica que los vuelos con retrasos en la llegada tienden a tener tiempos totales de vuelo más cortos.
5. **ARR\_DELAY y CANCELLED:**
   * **Correlación:** 0.0028
   * **Interpretación:** Hay una correlación muy débil positiva (0.0028) entre el tiempo de retraso en la llegada (ARR\_DELAY) y la probabilidad de cancelación del vuelo (CANCELLED). Esto sugiere que los retrasos en la llegada no están fuertemente relacionados con la probabilidad de cancelación del vuelo.
6. **ELAPSED\_DELAY y CANCELLED:**
   * **Correlación:** 2.35e-05
   * **Interpretación:** Hay una correlación extremadamente débil (2.35e-05) entre el tiempo total de vuelo (ELAPSED\_DELAY) y la probabilidad de cancelación del vuelo (CANCELLED). Esto sugiere que estas dos variables no están fuertemente relacionadas.

**Modelo de Regresión Logística:**

1. **Precisión del Modelo:**
   * **Resultado:** 0.9807
   * **Interpretación:** El modelo de regresión logística tiene una alta precisión del 98.07%, lo que indica que es eficaz para predecir si un vuelo será cancelado o no.
2. **Reporte de Clasificación:**
   * **Precision:** 0.98
   * **Recall:** 0.00
   * **F1-Score:** 0.01
   * **Interpretación:** El modelo tiene una precisión alta para predecir vuelos no cancelados, pero su capacidad para identificar vuelos cancelados (recall) es baja. Esto podría indicar que el modelo tiende a predecir menos vuelos cancelados de los que realmente existen.

**Prueba t de Student:**

* **Estadístico t:** 6.10
* **Valor p:** 1.03e-09

**Interpretación:**

* Hay evidencia significativa (valor p muy bajo) para rechazar la hipótesis nula de que no hay diferencia en los tiempos de retraso debido al transportista (DELAY\_DUE\_CARRIER). Esto sugiere que el tiempo de retraso debido al transportista es estadísticamente diferente de cero.

El modelo de regresión logística parece ser preciso en general, pero puede tener limitaciones en la predicción de vuelos cancelados. La prueba t indica que ciertos tipos de retrasos, como los debidos al transportista, son estadísticamente significativos.
