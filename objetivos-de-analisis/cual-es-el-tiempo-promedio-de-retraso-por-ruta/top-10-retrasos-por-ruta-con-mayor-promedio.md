# Top 10 Retrasos por Ruta con Mayor Promedio

### OPRIME <mark style="color:red;">**Colab Colaboratory**</mark> Se relaciona todos los cálculos realizados.

{% embed url="https://colab.research.google.com/drive/1yuv6CUyHP60Vgmr6KklY2k4odh8SbLi-#scrollTo=NNjVnRJPkiDa&line=1&uniqifier=1" %}

### Conclusiones

Este resultado muestra el promedio de tres tipos de retraso (salida, llegada y tiempo total de vuelo) para las 10 rutas con los mayores promedios combinados. Aquí está la interpretación para cada columna:

1. **ORIGIN y DEST:** Códigos de aeropuertos de origen y destino, respectivamente, para la ruta específica.
2. **promedio\_dep\_delay (Promedio de Retraso en Salida):** Representa el tiempo promedio de retraso en salida para vuelos en esa ruta. Un valor más alto indica un mayor promedio de retraso en salida.
3. **promedio\_arr\_delay (Promedio de Retraso en Llegada):** Indica el tiempo promedio de retraso en llegada para vuelos en esa ruta. Cuanto mayor sea el valor, más tiempo promedio de retraso en llegada experimentan los vuelos.
4. **promedio\_elapsed\_delay (Promedio de Retraso Total):** Representa el tiempo promedio total de vuelo, incluidos los retrasos en salida y llegada. Puede ser la suma de los dos anteriores o incluir otros factores. Un valor más alto indica un mayor tiempo promedio de retraso total.
5. **promedio\_combinado:** Es un promedio ponderado de los tres promedios anteriores, donde cada uno contribuye igualmente. Proporciona una medida combinada del rendimiento de la ruta en términos de retrasos. Un valor más alto indica una ruta con mayores promedios de retraso en general.

Este resultado te da una visión general de las rutas con mayores promedios de retraso en salida, llegada y tiempo total de vuelo, proporcionando un indicador combinado de la calidad de estas rutas en términos de puntualidad.
