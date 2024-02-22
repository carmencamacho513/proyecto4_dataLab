# Prueba de Significancia Test Mann-Whitney U

### OPRIME <mark style="color:red;">**Colab Colaboratory**</mark> Se relaciona todos los cálculos realizados.

{% embed url="https://colab.research.google.com/drive/1yuv6CUyHP60Vgmr6KklY2k4odh8SbLi-#scrollTo=JG4cz8_t_b97&line=1&uniqifier=1" %}

### Conclusiones

Mann-Whitney U, que es una prueba no paramétrica para las variables independientes en relación con la variable dependiente ARR\_DELAY:

1. **Para ELAPSED\_DELAY:**
   * Estadístico U: 44314230875.5
   * P-valor: 0.0
   * Interpretación: Existe una diferencia estadísticamente significativa en la distribución de ELAPSED\_DELAY entre los vuelos con ARR\_DELAY y los vuelos sin ARR\_DELAY. Se rechaza la hipótesis nula de igualdad de distribuciones.
2. **Para DELAY\_DUE\_CARRIER:**
   * Estadístico U: 667238521.5
   * P-valor: 0.0
   * Interpretación: Hay una diferencia estadísticamente significativa en la distribución de DELAY\_DUE\_CARRIER entre vuelos con y sin ARR\_DELAY. La hipótesis nula de igualdad de distribuciones se rechaza.
3. **Para DELAY\_DUE\_WEATHER:**
   * Estadístico U: 46926050925.0
   * P-valor: 0.0
   * Interpretación: Se observa una diferencia estadísticamente significativa en la distribución de DELAY\_DUE\_WEATHER entre vuelos con ARR\_DELAY y sin ARR\_DELAY. Se rechaza la hipótesis nula.
4. **Para DELAY\_DUE\_NAS:**
   * Estadístico U: 35087923417.5
   * P-valor: 0.0
   * Interpretación: Existe una diferencia estadísticamente significativa en la distribución de DELAY\_DUE\_NAS entre vuelos con y sin ARR\_DELAY. La hipótesis nula se rechaza.
5. **Para DELAY\_DUE\_SECURITY:**
   * Estadístico U: 39820652.0
   * P-valor: 0.0
   * Interpretación: Hay una diferencia estadísticamente significativa en la distribución de DELAY\_DUE\_SECURITY entre vuelos con ARR\_DELAY y sin ARR\_DELAY. La hipótesis nula se rechaza.
6. **Para DELAY\_DUE\_LATE\_AIRCRAFT:**
   * Estadístico U: 573674795.5
   * P-valor: 0.0
   * Interpretación: Existe una diferencia estadísticamente significativa en la distribución de DELAY\_DUE\_LATE\_AIRCRAFT entre vuelos con ARR\_DELAY y sin ARR\_DELAY. La hipótesis nula de igualdad de distribuciones se rechaza.

En todos los casos, se encontró que hay diferencias significativas en la distribución de las variables independientes entre vuelos con ARR\_DELAY y aquellos sin ARR\_DELAY.

### OPRIME <mark style="color:red;">En conceptos Obtenidos en el Proceso</mark> encuentras la definición de Test Mann-Whitney U



{% content-ref url="../../../conceptos-obtenidos-en-el-proceso-proyecto-4-datalab.md" %}
[conceptos-obtenidos-en-el-proceso-proyecto-4-datalab.md](../../../conceptos-obtenidos-en-el-proceso-proyecto-4-datalab.md)
{% endcontent-ref %}
