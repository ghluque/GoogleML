
 # Introduccion al aprendizaje automatico


El aprendizaje automatico es el proceso de entrenar un software llamada modelo para que sea util generar predicciones o contenido a partir de datos no estructurados.

Con un enfoque de AA, le daríamos a un modelo de AA enormes cantidades de datos hasta que el modelo de AA finalmente aprendió la relación matemática entre los patrones para un determinado fin. Es decir, algo que querramos predecir. 

Por ultimo, agregariamos datos reales a nuestro modelo para contrastar con los datos generados anteriormente para aumentar la eficacia de nuestro software. De esta manera estariamos entrenando nuestro modelo para disminuir errores de nuestra prediccion.

***Un modelo es una relación matemática derivada de datos que un AA que el sistema usa para hacer predicciones.***


## Tipos de sistemas de AA

### Aprendizaje supervisado

Los modelos pueden hacer predicciones despues de analizar muchos datos correctos anteriores y descubrir las conexiones entre si, Es decir, si yo mañana tengo que tomarme un bondi a las 9 am y tengo los registros de los bondis que pasaron entre las 8:45 y las 9:15 en el ultimo año, puedo prever a que hora salir de casa para no perdermelo. La persona le brinda al software los datos conocidos para poder predecir. 

Dos de los casos de uso más comunes del aprendizaje supervisado son la regresión y clasificación.


#### Regresion 

Un modelo de regresion predice un valor numerico.

----
| Situacion  | Posibles datos de entrada  | Prediccion numerica |
| :------------ |:---------------:| -----:|
| Precio de la casa a futuro      | En metros cuadrados, código postal, cantidad de habitaciones y baños, tamaño del lote tasa de interés hipotecaria, tasa impositiva a la propiedad, costos de construcción y la cantidad de viviendas en venta en el área. | El precio de la casa |
| Tiempo de viaje futuro      | Condiciones históricas de tráfico (obtenidas de smartphones, tráfico transporte privado a pedido y otras aplicaciones de navegación), la distancia desde destino y las condiciones climáticas.        |   Es el tiempo en minutos y segundos que tarda en llegar a un destino. 

----

El aprendizaje automático esta compuesto por: 

- Datos
- Modelo
- Capacitación
- Evaluación
- Inferencia

Los conjuntos de datos se componen de ejemplos individuales que contienen atributos y etiqueta. Los atributos son los datos que usa un modelo supervisado para predecir la etiqueta. La etiqueta es aquello que queremos predecir. 

### Matriz de datos

![](https://github.com/ghluque/GoogleML/blob/main/Imagenes/MatrizDatos.png)

Generalmente los datos vienen representados en matrices, como usualmente vemos en las planillas de cálculo. En ellas se organiza la información para diversos fines, es muy facil de entender y agrupar la información. 

En el las columnas podemos encontrar los diferentes atributos y etiquetas. Graficamente representarian el eje Y. En las filas encontramos los casos, individuales. Graficamente representarian el eje X. 

***Los datos son el insumo principal de cualquier investigación. Mientras tengamos la mayor cantidad de atributos y casos disponibles de acuerdo a lo que queremos investigar, mayor será el acierto de la misma. Nuestro analisis concluirá siendo más exhaustivo***

### Modelo

Es una construcción matemática que teniendo datos de entrada y al procesarlos, se obtienen datos de salida. En todos los ámbitos de la vida obtenemos datos, todo el tiempo. Pero los datos en bruto no nos sirven de mucho si no los procesamos. Para hacerlo necesitamos un modelo que no es más ni menos que un conjunto de parámetros y estructura necesarios para que un sistema realice predicciones. En el aprendizaje automático supervisado, un modelo toma un ejemplo como entrada y deduce una predicción como resultado.

### Capacitación

Antes de que un modelo pueda hacer predicciones debe entrenarse. Dandole un conjunto de datos con ejemplos etiquetados podemos determinar la mejor solución para predecir las etiquetas a partir de los atributos. El modelo encuentra la mejor solución mediante la comparación del valor predicho con el valor real de la etiqueta.En función de la diferencia entre los valores predichos y reales, definidos como la pérdida, el modelo actualiza su solución de forma gradual. Es decir, el modelo aprende la relación matemática entre los atributos y la etiqueta para mejorar futuras predicciones. Ej: 

La primera predicción del sistema me dió que hoy iba a llover 50 ml 

Pero contrastandolo, hoy en realidad llovió 100 ml

Entonces, agregando al sistema el dato real de que hoy llovió 100 ml. En una proxima predicción me dirá que llovera 75 ml, acercandose asi cada vez al valor real, segun el promedio de los datos ingresados. Como dijimos anteriormente, mientras mas datos afines tengamos para poder analizar, mayor será el acierto de la predicción del sistema.


