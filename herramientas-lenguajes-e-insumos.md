# 🛫 Herramientas, lenguajes e insumos

### 1.1 Herramientas y/o plataformas <a href="#id-11herramientasyoplataformas" id="id-11herramientasyoplataformas"></a>

En este proyecto podrás elegir con qué herramientas trabajarás, recordando que cada herramienta tiene su función, por ejemplo, no podemos procesar y limpiar datos en PowerBI, y algunas técnicas de análisis se aplican más fácilmente usando el lenguaje Python. Herramientas disponibles:

* BigQuery
* Power BI
* Google Colab
* Canva

#### 1.2 Lenguajes <a href="#id-12lenguajes" id="id-12lenguajes"></a>

Podrás utilizar el lenguaje SQL en BigQuery y Python en Google Colab.

#### **Opción 3: Flight Delay and Cancellation** <a href="#opcin3flightdelayandcancellation" id="opcin3flightdelayandcancellation"></a>

Conjunto de datos sobre cancelaciones y retrasos de vuelos de aerolíneas de enero de 2023, datos extraídos del Departamento de Transporte de EE. UU., Oficina de Estadísticas de Transporte (https://www.transtats.bts.gov) y disponibles en Kaggle.

Las variables incluyen rutas de vuelo (origen y destino), rangos de tiempo para eventos (minutos, hora en destino), motivos/atribuciones de retrasos y cancelaciones.

**Descripción de las variables:**

**Tabla DOT**_**CODE**_**DICTIONARY**

* Code: Identificador numérico del U.S. Department of Transportation (DOT) para aerolíneas
* Description: descripción de la aerolínea

**Tabla AIRLINE**_**CODE**_**DICTIONARY**

* Code: Código de operador único para agencias operadoras de aeronaves
* Description: descripción de la agencia operadora de aeronaves

**Tabla flights\_202301**

* FL\_DATE: Fecha de vuelo (yyyymmdd)
* AIRLINE\_CODE: Código de operador único. Cuando varios operadores han utilizado el mismo código, se utiliza un sufijo numérico para usuarios anteriores, por ejemplo, PA, PA(1), PA(2).
* DOT\_CODE: Un número de identificación asignado por el DOT de EE. UU. para identificar una aerolínea (transportista) única. Una aerolínea (transportista) única se define como aquella que posee y reporta bajo el mismo certificado DOT independientemente de su código, nombre o compañía/corporación holding.
* FL\_NUMBER: Número de vuelo
* ORIGIN: Aeropuerto de origen
* ORIGIN\_CITY: Aeropuerto de origen, nombre de la ciudad
* DEST: Aeropuerto de destino
* DEST\_CITY: Aeropuerto de destino, nombre de la ciudad
* CRS_DEP_TIME: Hora de salida registrada CRS (Sistema de control de reservas) (hora local: hhmm)
* DEP\_TIME: Hora de salida real (hora local: hhmm)
* DEP\_DELAY: Diferencia en minutos entre la hora de salida prevista y la real. Las salidas anticipadas arrojan cifras negativas.
* TAXI\_OUT: Tiempo de taxi en la salida en minutos (taxi es el proceso de mover un avión mientras se encuentra en la pista)
* WHEELS\_OFF: hora exacta de despegue (hora local: hhmm)
* WHEELS\_ON: hora exacta de aterrizaje (hora local: hhmm)
* TAXI\_IN: tiempo de taxi en la llegada en minutos
* CRS_ARR_TIME: Hora de llegada registrada en CRS (hora local: hhmm)
* ARR\_TIME: Hora de llegada real (hora local: hhmm)
* ARR\_DELAY: Diferencia en minutos entre la hora de llegada prevista y la real. Las llegadas anticipadas arrojan cifras negativas.
* CANCELLED: Indicador de vuelo cancelado (1=Sí)
* CANCELLATION\_CODE: Especifica el motivo de la cancelación
* DIVERTED: Indicador de vuelo desviado (1=Sí)
* CRS_ELAPSED_TIME: Tiempo total de vuelo transcurrido en minutos registrado en CRS
* ELAPSED\_TIME: Tiempo total de vuelo transcurrido en minutos real
* AIR\_TIME: Tiempo de vuelo en el aire en minutos
* DISTANCE: Distancia entre aeropuertos (millas)
* DELAY_DUE_CARRIER: Retraso del operador en minutos
* DELAY_DUE_WEATHER: Retraso meteorológico en minutos
* DELAY_DUE_NAS: Retraso del Sistema Aéreo Nacional en Minutos
* DELAY_DUE_SECURITY: Retraso de seguridad en minutos
* DELAY_DUE_LATE\_AIRCRAFT: Retraso de aeronaves tardías en minutos

Haga download del conjunto de datos [aquí](https://drive.google.com/file/d/1cEepkz0X-l0855bPWHhj2f5Z2jM-nvcb/view?usp=sharing).
