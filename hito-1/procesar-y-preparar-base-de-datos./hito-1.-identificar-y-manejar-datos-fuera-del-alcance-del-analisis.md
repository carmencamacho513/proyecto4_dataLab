# Hito 1. Identificar Y Manejar Datos Fuera Del Alcance Del Análisis

### OPRIME <mark style="color:red;">**Colab Colaboratory**</mark> Se relaciona todos los calculos realizados.

{% embed url="https://colab.research.google.com/drive/1yuv6CUyHP60Vgmr6KklY2k4odh8SbLi-#scrollTo=Vlqq_pQy0Jvr" %}

### Conclusiones

* Realizamos una tablas para saber cuantas columnas y cuales son float-Object-Int.
*

    Para el estudio determinamos las siguientes variables:

    * \*_DEP\_TIME \*_(Hora de salida real): Indica la hora exacta en que un vuelo despega.
    * **CANCELLED**: Indicador de vuelo cancelado (1=Sí)
    * **DEP\_DELAY** (Diferencia en minutos entre la hora de salida prevista y la real): Esta variable indica cuánto tiempo se ha retrasado el vuelo en comparación con la hora de salida programada. Un valor positivo significa un retraso.
    * **ARR\_DELAY** Diferencia en minutos entre la hora de llegada prevista y la real. Las llegadas anticipadas arrojan cifras negativas.
    * **ELAPSED DELAY** Diferencia en minutos entre el total de minutos de vuelo transcurrido y total de minutos de vuelo transcurrido real. Las llegadas anticipadas arrojan cifras negativas.
    * **DELAYDUECARRIER** (Retraso del operador en minutos): Muestra el retraso atribuido al operador de la aerolínea. Puede deberse a problemas operativos internos de la aerolínea.
    * **DELAYDUEWEATHER** (Retraso meteorológico en minutos): Indica el retraso causado por condiciones meteorológicas adversas. Las condiciones climáticas pueden afectar el despegue y el aterrizaje.
    * **DELAYDUENAS**(Retraso del Sistema Aéreo Nacional en Minutos): Representa el retraso atribuido al Sistema Aéreo Nacional, lo que puede incluir congestión del tráfico aéreo, problemas de gestión del espacio aéreo, etc.
    * **DELAYDUESECURITY** (Retraso de seguridad en minutos): Indica el retraso debido a cuestiones de seguridad. Esto puede deberse a inspecciones de seguridad adicionales u otras preocupaciones de seguridad.
    * **DELAYDUELATE\_AIRCRAFT**(Retraso de aeronaves tardías en minutos): Muestra el retraso causado por la llegada tardía de la aeronave asignada al vuelo. Si la aeronave anterior llega tarde, puede afectar el horario del vuelo actual.

###





