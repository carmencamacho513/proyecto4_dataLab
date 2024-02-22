# ¿Es posible identificar el principal motivo de retraso?

### OPRIME <mark style="color:red;">**Colab Colaboratory**</mark> Se relaciona todos los cálculos realizados.

{% embed url="https://colab.research.google.com/drive/1yuv6CUyHP60Vgmr6KklY2k4odh8SbLi-#scrollTo=aEVFwPiIX1A4&line=1&uniqifier=1" %}

### Conclusiones

El resultado se basa en la clasificación de los motivos de retraso en función de la suma total de minutos atribuidos a cada categoría:

1. **Late Aircraft (Aeronave Tardía):**
   * Suma de Retrasos: 13,785,311.96 minutos
   * Ocupa el primer lugar en la cantidad total de minutos de retraso. Esto indica que los vuelos afectados por aeronaves que llegaron tarde contribuyen significativamente al tiempo total de retraso.
2. **Carrier (Operador de la Aerolínea):**
   * Suma de Retrasos: 12,934,192.78 minutos
   * Ocupa el segundo lugar en la cantidad total de minutos de retraso. Los problemas operativos internos de las aerolíneas, como tripulación y mantenimiento, también son una fuente importante de retrasos.
3. **NAS (Sistema Nacional de Aviación):**
   * Suma de Retrasos: 7,877,676.81 minutos
   * Ocupa el tercer lugar en la cantidad total de minutos de retraso. Problemas en el sistema de gestión del tráfico aéreo y congestiones en el espacio aéreo contribuyen a esta categoría de retrasos.
4. **Weather (Clima):**
   * Suma de Retrasos: 2,281,650.71 minutos
   * Ocupa el cuarto lugar en la cantidad total de minutos de retraso. Las condiciones meteorológicas adversas, como tormentas y nieve, también tienen un impacto significativo en el tiempo de retraso acumulado.
5. **Security (Seguridad):**
   * Suma de Retrasos: 78,497.77 minutos
   * Ocupa el último lugar en la cantidad total de minutos de retraso. Los retrasos relacionados con medidas de seguridad adicionales en los aeropuertos y durante los vuelos son menos frecuentes en comparación con otras categorías.

### **Aquí hay algunas observaciones clave:**

1. **Correlaciones:** La correlación entre ARR\_DELAY y diferentes tipos de retrasos (DELAY\_DUE\_CARRIER, DELAY\_DUE\_WEATHER, etc.) proporciona información sobre cómo estos factores están relacionados entre sí y con el retraso total de llegada. Por ejemplo, una correlación alta con DELAY\_DUE\_CARRIER podría indicar que los retrasos debidos a la aerolínea son un factor significativo en los retrasos totales de llegada.
2. **Regresión Lineal Ordinaria (OLS):** Los coeficientes y p-values en los resultados de la regresión lineal ordinaria (OLS) te dan una idea de la contribución relativa de cada variable independiente (por ejemplo, DELAY\_DUE\_CARRIER, DELAY\_DUE\_WEATHER) al retraso total de llegada (ARR\_DELAY). Un coeficiente positivo y un p-value bajo podrían indicar una relación significativa.
3. **Mann-Whitney U test:** Al realizar pruebas de Mann-Whitney U en variables como ELAPSED\_DELAY, DELAY\_DUE\_CARRIER, etc., y obtener p-values bajos, indicas que hay diferencias significativas entre las categorías. Esto puede ayudar a identificar si ciertos factores están contribuyendo de manera significativa a los retrasos.
4. **Regresión Logística:** El resultado de la regresión logística indica la relación entre las variables independientes binarias (CANCELLED, DEP\_DELAY\_dummy, etc.) y la probabilidad de que ARR\_DELAY\_dummy sea 1. Puedes observar los coeficientes para entender cómo cada variable afecta la probabilidad de retraso en llegada.

Aquí hay algunas pautas basadas en la información proporcionada:

1. **Correlación:** Observa las correlaciones entre ARR\_DELAY y otras variables. La correlación más alta podría indicar el factor más influyente. En este caso, la correlación más alta es con ELAPSED\_DELAY (0.9401), lo que sugiere que el tiempo de vuelo total (ELAPSED\_DELAY) tiene una fuerte relación positiva con los retrasos de llegada.
2. **Regresión Lineal Ordinaria (OLS):** Analiza los coeficientes en la regresión lineal ordinaria. Los coeficientes más grandes y significativos (p-value bajo) indican variables que tienen una mayor influencia en los retrasos. Según los resultados proporcionados, DELAY\_DUE\_LATE\_AIRCRAFT tiene el coeficiente más grande (0.9550), lo que sugiere que los retrasos debidos a problemas con la aeronave tienen una gran influencia en los retrasos de llegada.
3. **Mann-Whitney U test:** Las pruebas indican que hay diferencias significativas en ELAPSED\_DELAY, DELAY\_DUE\_CARRIER, DELAY\_DUE\_WEATHER, etc. Esto refuerza la idea de que estos factores están asociados con los retrasos en la llegada.

Según la información proporcionada, el tiempo de vuelo total (ELAPSED\_DELAY) y los retrasos debidos a problemas con la aeronave (DELAY\_DUE\_LATE\_AIRCRAFT) podrían ser dos de los principales motivos de los retrasos en la llegada.&#x20;
