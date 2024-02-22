---
description: Big Query
---

# Hito 1. Calcular Riesgo Relativo

```sql
WITH
  cuartiles AS (
  SELECT
    APPROX_QUANTILES(DEP_TIME, 4) AS cuartiles_DEP_TIME,
    APPROX_QUANTILES(DEP_DELAY, 4) AS cuartiles_DEP_DELAY,
    APPROX_QUANTILES(ARR_DELAY, 4) AS cuartiles_ARR_DELAY,
    APPROX_QUANTILES(DELAY_DUE_CARRIER, 4) AS cuartiles_DELAY_DUE_CARRIER,
    APPROX_QUANTILES(DELAY_DUE_WEATHER, 4) AS cuartiles_DELAY_DUE_WEATHER,
    APPROX_QUANTILES(DELAY_DUE_NAS, 4) AS cuartiles_DELAY_DUE_NAS,
    APPROX_QUANTILES(DELAY_DUE_SECURITY, 4) AS cuartiles_DELAY_DUE_SECURITY,
    APPROX_QUANTILES(DELAY_DUE_LATE_AIRCRAFT, 4) AS cuartiles_DELAY_DUE_LATE_AIRCRAFT
  FROM
    `proyecto-4-datalab-413416.dataLab.imputados_202301` )
SELECT
  (cuartiles_DEP_TIME[1] / cuartiles_DEP_TIME[4]) AS rr_DEP_TIME,
  (cuartiles_DEP_DELAY[1] / cuartiles_DEP_DELAY[4]) AS rr_DEP_DELAY,
  (cuartiles_ARR_DELAY[1] / cuartiles_ARR_DELAY[4]) AS rr_ARR_DELAY,
  (cuartiles_DELAY_DUE_CARRIER[1] / cuartiles_DELAY_DUE_CARRIER[4]) AS rr_DELAY_DUE_CARRIER,
  (cuartiles_DELAY_DUE_WEATHER[1] / cuartiles_DELAY_DUE_WEATHER[4]) AS rr_DELAY_DUE_WEATHER,
  (cuartiles_DELAY_DUE_NAS[1] / cuartiles_DELAY_DUE_NAS[4]) AS rr_DELAY_DUE_NAS,
  (cuartiles_DELAY_DUE_SECURITY[1] / cuartiles_DELAY_DUE_SECURITY[4]) AS rr_DELAY_DUE_SECURITY,
  (cuartiles_DELAY_DUE_LATE_AIRCRAFT[1] / cuartiles_DELAY_DUE_LATE_AIRCRAFT[4]) AS rr_DELAY_DUE_LATE_AIRCRAFT 
FROM
  cuartiles;
```

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

### Conclusiones

Explicación de cada variable:

1. **rr\_DEP\_DELAY (0.38125):**
   * **Interpretación:** El riesgo relativo de DEP\_DELAY es 0.38125. Esto significa que, el riesgo relativo de experimentar un retraso en la salida (DEP\_DELAY) disminuye en aproximadamente un 38.13%. En otras palabras, a medida que la hora de salida aumenta, el riesgo relativo de experimentar un retraso en la salida tiende a disminuir.
2. **rr\_ARR\_DELAY (-0.001984126984126984):**
   * **Interpretación:** El riesgo relativo de ARR\_DELAY es -0.00198. En este caso, el valor es muy cercano a cero, lo que indica que no hay un cambio sustancial en el riesgo relativo de experimentar un retraso en la llegada (ARR\_DELAY) en función de la hora de salida.
3. **rr\_DELAY\_DUE\_CARRIER (-0.0048971596474045058):**
   * **Interpretación:** El riesgo relativo de DELAY\_DUE\_CARRIER es -0.0049. Similar al caso anterior, este valor cercano a cero sugiere que no hay un cambio sustancial en el riesgo relativo de experimentar un retraso atribuido al operador de la aerolínea en función de la hora de salida.
4. **rr\_DELAY\_DUE\_WEATHER (0.0081049416111705647):**
   * **Interpretación:** El riesgo relativo de DELAY\_DUE\_WEATHER es 0.0081. Esto significa que, el riesgo relativo de experimentar un retraso debido a condiciones meteorológicas adversas tiende a aumentar en aproximadamente un 0.81%.
5. **rr\_DELAY\_DUE\_NAS (0.0026521279552607457):**
   * **Interpretación:** El riesgo relativo de DELAY\_DUE\_NAS es 0.00265. Indica que, el riesgo relativo de experimentar un retraso atribuido al Sistema Aéreo Nacional tiende a aumentar en aproximadamente un 0.27%.
6. **rr\_DELAY\_DUE\_SECURITY (0.010907288288786539):**
   * **Interpretación:** El riesgo relativo de DELAY\_DUE\_SECURITY es 0.0109. Esto implica que, el riesgo relativo de experimentar un retraso debido a problemas de seguridad tiende a aumentar en aproximadamente un 1.09%.
7. **rr\_DELAY\_DUE\_LATE\_AIRCRAFT (0.00062498988496949325):**
   * **Interpretación:** El riesgo relativo de DELAY\_DUE\_LATE\_AIRCRAFT es 0.000625. Indica que, el riesgo relativo de experimentar un retraso debido a la llegada tardía de la aeronave asignada al vuelo tiende a aumentar en aproximadamente un 0.06%.

### OPRIME <mark style="color:red;">En conceptos Obtenidos en el Proceso</mark> encuentras la definición de Riesgo Relativo.&#x20;

{% content-ref url="../../conceptos-obtenidos-en-el-proceso-proyecto-4-datalab.md" %}
[conceptos-obtenidos-en-el-proceso-proyecto-4-datalab.md](../../conceptos-obtenidos-en-el-proceso-proyecto-4-datalab.md)
{% endcontent-ref %}
