# Hito 1. Validación de Hipótesis.

Analizamos cada hipótesis en función de los resultados de las correlaciones y los riesgos relativos:

**Hipótesis:** A mayor retraso en la salida programada, mayor será el retraso en la llegada.

* **Correlación:** 0.9400778480455102 (Fuerte correlación positiva)
* **Riesgo Relativo:** r\_DEP\_DELAY: 0.38125 (Positivo)
* **Interpretación:** La hipótesis es verdadera. Existe una fuerte correlación positiva entre el retraso en la salida (DEP\_DELAY) y el retraso en la llegada (ARR\_DELAY). Además, el riesgo relativo es positivo, lo que sugiere que a medida que aumenta el retraso en la salida, el riesgo de tener retraso en la llegada también aumenta.

**Hipótesis:** Si hay retrasos en la llegada del vuelo, influye en la hora de salida real del siguiente vuelo.

* **Correlación:** -0.3585672329243136 (Correlación negativa moderada)
* **Riesgo Relativo:** rr\_ELAPSED\_DELAY: -0.001984126984126984 (Negativo)
* **Interpretación:** La hipótesis es verdadera. Existe una correlación negativa moderada entre el retraso en la llegada (ARR\_DELAY) y la diferencia en minutos entre el tiempo total de vuelo transcurrido y el tiempo total de vuelo transcurrido real (ELAPSED\_DELAY). Además, el riesgo relativo es negativo, indicando que a medida que disminuye el tiempo total de vuelo transcurrido, el riesgo de tener retraso en la llegada aumenta.

**Hipótesis:** Los problemas internos de la aerolínea afectan la programación de vuelos, incluyendo la hora de salida real.

* **Correlación:** 0.32340139932838385 (Correlación positiva)
* **Riesgo Relativo:** rr\_DELAY\_DUE\_CARRIER: -0.0048971596474045058 (Negativo)
* **Interpretación:** La hipótesis es verdadera. Existe una correlación positiva entre el retraso en la llegada (ARR\_DELAY) y el retraso atribuido al operador de la aerolínea (DELAY\_DUE\_CARRIER). Además, el riesgo relativo es negativo, lo que sugiere que a medida que disminuye el retraso atribuido al operador de la aerolínea, el riesgo de tener retraso en la llegada aumenta.

**Hipótesis:** Las condiciones climáticas adversas pueden afectar tanto la salida como la llegada de los vuelos, influyendo en la hora de salida real.

* **Correlación:** 0.16986664734248974 (Correlación positiva)
* **Riesgo Relativo:** rr\_DELAY\_DUE\_WEATHER: 0.0081049416111705647 (Positivo)
* **Interpretación:** La hipótesis es verdadera. Existe una correlación positiva entre el retraso en la llegada (ARR\_DELAY) y el retraso debido a condiciones meteorológicas (DELAY\_DUE\_WEATHER). Además, el riesgo relativo es positivo, indicando que a medida que aumenta el retraso debido a condiciones meteorológicas, el riesgo de tener retraso en la llegada también aumenta.

**Hipótesis:** La congestión del tráfico aéreo puede impactar en la puntualidad de los vuelos, afectando la hora de salida real de los vuelos.

* **Correlación:** 0.1585968622354697 (Correlación positiva)
* **Riesgo Relativo:** rr\_DELAY\_DUE\_NAS: 0.0026521279552607457 (Positivo)
* **Interpretación:** La hipótesis es verdadera. Existe una correlación positiva entre el retraso en la llegada (ARR\_DELAY) y el retraso atribuido al Sistema Aéreo Nacional (DELAY\_DUE\_NAS). Además, el riesgo relativo es positivo, indicando que a medida que aumenta el retraso atribuido al Sistema Aéreo Nacional, el riesgo de tener retraso en la llegada también aumenta.

**Hipótesis:** La seguridad de procesos adicionales afecta la programación de vuelos y la hora de salida real.

* **Correlación:** 0.004116278492951491 (Correlación positiva débil)
* **Riesgo Relativo:** rr\_DELAY\_DUE\_SECURITY: 0.010907288288786539 (Positivo)
* **Interpretación:** La hipótesis es verdadera en parte. Existe una correlación positiva débil entre el retraso en la llegada (ARR\_DELAY) y el retraso de seguridad (DELAY\_DUE\_SECURITY). Además, el riesgo relativo es positivo, indicando que a medida que aumenta el retraso de seguridad, el riesgo de tener retraso en la llegada también aumenta, pero la correlación es débil.

**Hipótesis:** La llegada tardía de la aeronave asignada puede generar retrasos en la salida del vuelo actual, influyendo en la hora de salida real de los vuelos.

* **Correlación:** 0.35928659772844646 (Correlación positiva)
* **Riesgo Relativo:** rr\_DELAY\_DUE\_LATE\_AIRCRAFT: 0.0127063358260089 (Positivo)
* **Interpretación:** La hipótesis es verdadera. Existe una correlación positiva entre el retraso en la llegada (ARR\_DELAY) y el retraso debido a la llegada tardía de la aeronave asignada (DELAY\_DUE\_LATE\_AIRCRAFT). Además, el riesgo relativo es positivo, indicando que a medida que aumenta el retraso debido a la llegada tardía de la aeronave asignada, el riesgo de tener retraso en la llegada también aumenta.

**Hipótesis:** La hora de llegada real no se ve significativamente afectada por si el vuelo fue cancelado.

* **Correlación:** 0.003181822810102347 (Correlación positiva débil)
* **Riesgo Relativo:** No hay riesgo relativo asociado a la variable CANCELLED
* **Interpretación:** La hipótesis es falsa. La correlación positiva débil entre el retraso en la llegada (ARR\_DELAY) y la variable de vuelo cancelado (CANCELLED) sugiere una relación débil, pero no se puede establecer una relación significativa sin un riesgo relativo asociado.













