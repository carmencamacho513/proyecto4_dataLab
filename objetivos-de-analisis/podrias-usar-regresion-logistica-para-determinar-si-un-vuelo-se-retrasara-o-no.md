# ¿Podrías usar regresión logística, para determinar si un vuelo se retrasará o no?

### OPRIME <mark style="color:red;">**Colab Colaboratory**</mark> Se relaciona todos los cálculos realizados.

{% embed url="https://colab.research.google.com/drive/1yuv6CUyHP60Vgmr6KklY2k4odh8SbLi-#scrollTo=lKTNBEUJA2oh&line=1&uniqifier=1" %}

### Conclusiones

El resultado del modelo de regresión logística proporciona información sobre su rendimiento en la tarea de predecir si un vuelo se retrasará o no. Aquí hay una interpretación de los resultados:

**Accuracy (Exactitud): 79.34%**

* Esto significa que, en general, el modelo acierta alrededor del 79.34% de las veces al predecir si un vuelo se retrasará o no.

**Confusion Matrix (Matriz de Confusión):**

* Hay cuatro números importantes:
  * Verdaderos Negativos (TN): 60,933 vuelos sin retraso correctamente clasificados.
  * Falsos Positivos (FP): 6,384 vuelos sin retraso clasificados erróneamente como con retraso.
  * Falsos Negativos (FN): 15,874 vuelos con retraso clasificados erróneamente como sin retraso.
  * Verdaderos Positivos (TP): 24,577 vuelos con retraso correctamente clasificados.

**Classification Report (Informe de Clasificación):**

* Para entender el informe:
  * Precision (Precisión): De los vuelos que predice como sin retraso o con retraso, ¿cuántos son realmente así?
  * Recall (Recuperación): De todos los vuelos sin retraso o con retraso, ¿cuántos predice correctamente?
  * F1-score: Combina precisión y recuperación en una sola métrica.
* Ejemplo:
  * Para vuelos sin retraso (clase 0):
    * Precision: De los vuelos que predice como sin retraso, el 79% realmente lo son.
    * Recall: De todos los vuelos sin retraso, el 91% los predice correctamente.
    * F1-score: Una combinación de precisión y recall, siendo 1 el mejor.
  * Para vuelos con retraso (clase 1):
    * Precision: De los vuelos que predice como con retraso, el 79% realmente lo son.
    * Recall: De todos los vuelos con retraso, el 61% los predice correctamente.
    * F1-score: Una combinación de precisión y recall, siendo 1 el mejor.

En resumen, el modelo tiene un buen rendimiento al prever vuelos sin retraso.

\
