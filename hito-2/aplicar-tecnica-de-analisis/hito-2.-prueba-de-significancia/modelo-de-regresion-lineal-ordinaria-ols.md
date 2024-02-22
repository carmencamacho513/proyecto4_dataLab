# Modelo de regresión lineal ordinaria (OLS)

### OPRIME <mark style="color:red;">**Colab Colaboratory**</mark> Se relaciona todos los cálculos realizados.

{% embed url="https://colab.research.google.com/drive/1yuv6CUyHP60Vgmr6KklY2k4odh8SbLi-#scrollTo=O_P7rACgOfEY" %}

### Conclusiones

Modelo de regresión lineal ordinaria (OLS) que trata de explicar la variable dependiente `ARR_DELAY` utilizando varias variables independientes:

1. **R-squared y Adj. R-squared:**
   * **R-squared:** Representa la proporción de la variabilidad en la variable dependiente (ARR\_DELAY) que es explicada por el modelo. En este caso, el 54% de la variabilidad en ARR\_DELAY se explica por las variables independientes del modelo.
   * **Adj. R-squared:** Similar a R-squared, pero ajusta el valor según la cantidad de variables en el modelo.
2. **F-statistic y Prob (F-statistic):**
   * **F-statistic:** Es una estadística que evalúa si al menos una de las variables independientes tiene un impacto significativo en la variable dependiente. Cuanto mayor sea el valor, mejor.
   * **Prob (F-statistic):** Es el p-valor asociado al F-statistic. En este caso, el p-valor es 0, lo que indica que el modelo en su conjunto es estadísticamente significativo.
3. **Coeficientes (coef):**
   * **const:** Intercepto del modelo, el valor esperado de ARR\_DELAY cuando todas las variables independientes son cero.
   * **ELAPSED\_DELAY, CANCELLED, etc.:** Coeficientes de las variables independientes. Indican cómo cambia el valor esperado de ARR\_DELAY cuando la variable independiente correspondiente aumenta en una unidad.
4. **Std err, t-statistic, P>|t|, \[0.025, 0.975]:**
   * **Std err:** Desviación estándar del coeficiente, mide la variabilidad del coeficiente.
   * **t-statistic:** Mide cuántas desviaciones estándar está el coeficiente del valor cero. Cuanto mayor sea el valor absoluto, más significativo es.
   * **P>|t|:** P-valor asociado al t-statistic. Indica la significancia estadística del coeficiente.
   * **\[0.025, 0.975]:** Intervalo de confianza del 95% para el coeficiente.
5. **Omnibus, Durbin-Watson, Jarque-Bera, Skew, Kurtosis:**
   * **Omnibus:** Una prueba estadística global de normalidad de los residuos.
   * **Durbin-Watson:** Evalúa la autocorrelación de los residuos (idealmente cerca de 2).
   * **Jarque-Bera:** Una prueba de normalidad de los residuos.
   * **Skew:** Mide la asimetría de los residuos.
   * **Kurtosis:** Mide la "pesadez de la cola" de los residuos.
6. **Cond. No.:** Número de condición, mide la estabilidad numérica del cálculo de los coeficientes.

El modelo parece ser significativo en conjunto, y cada variable independiente tiene un impacto significativo en la variable dependiente, según los p-valores asociados y la magnitud de los coeficientes.



### OPRIME <mark style="color:red;">En conceptos Obtenidos en el Proceso</mark> encuentras la definición de Modelo de Regresión Lineal Ordinaria (OLS)

{% content-ref url="../../../conceptos-obtenidos-en-el-proceso-proyecto-4-datalab.md" %}
[conceptos-obtenidos-en-el-proceso-proyecto-4-datalab.md](../../../conceptos-obtenidos-en-el-proceso-proyecto-4-datalab.md)
{% endcontent-ref %}
