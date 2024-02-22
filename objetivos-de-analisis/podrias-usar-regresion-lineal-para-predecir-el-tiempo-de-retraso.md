# ¿Podrías usar regresión lineal para predecir el tiempo de retraso?

### OPRIME <mark style="color:red;">**Colab Colaboratory**</mark> Se relaciona todos los cálculos realizados.

{% embed url="https://colab.research.google.com/drive/1yuv6CUyHP60Vgmr6KklY2k4odh8SbLi-#scrollTo=qIlohjUH6RmB&line=1&uniqifier=1" %}

### Conclusiones

En base a los resultados proporcionados:

1. **Variables predictoras:** Las variables predictoras que estás utilizando para tu modelo son `DELAY_DUE_CARRIER`, `DELAY_DUE_WEATHER`, `DELAY_DUE_NAS`, `DELAY_DUE_SECURITY`, y `DELAY_DUE_LATE_AIRCRAFT`.
2. **Valores faltantes:** No hay valores faltantes en estas variables predictoras, ya que el recuento de valores nulos es 0 para cada una.
3. **Mean Squared Error (MSE):** El MSE obtenido es relativamente alto (914.21). Esto sugiere que las predicciones del modelo pueden tener una variabilidad significativa con respecto a los valores reales. Un MSE más alto indica una mayor dispersión en las predicciones, lo cual puede deberse a la naturaleza de los datos o a la calidad de las variables predictoras.
4. **R-squared (R²):** El R-squared es moderado (0.709), lo que significa que el modelo explica alrededor del 70.9% de la variabilidad en la variable de respuesta. .

El modelo de regresión lineal aún puede utilizarse para predecir el tiempo de retraso, es importante tener en cuenta que el rendimiento del modelo puede depender de la calidad y relevancia de las variables predictoras seleccionadas.&#x20;

\


\


\
