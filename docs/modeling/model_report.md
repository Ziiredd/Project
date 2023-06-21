# Reporte del Modelo Final

## Descripción del Problema

Dado los resultados anteriores de la red neuronal recurrente (RNN), vamos a definir una función de costo que penalice la falta de estructura y observaremos los resultados obtenidos.

La función de coste que utilizaremos tiene como objetivo medir la discrepancia entre la salida de la RNN y la estructura deseada. Penalizará aquellos casos en los que la salida no siga un patrón o no se ajuste adecuadamente a la estructura esperada.

Una vez definida esta función de coste, procederemos a evaluar los resultados de la RNN. Analizaremos cómo se comporta la red en términos de estructura y compararemos los resultados con nuestras expectativas.

Esta evaluación nos permitirá determinar si la RNN está aprendiendo correctamente la estructura deseada y si la función de coste está cumpliendo su propósito de penalizar la falta de estructura. A partir de estos resultados, podremos realizar ajustes y mejoras en el modelo, si es necesario.

## Descripción del Modelo

En este modelo se utilizan dos capas de LSTM para mejorar la capacidad de aprendizaje de la red neuronal y capturar patrones complejos en la serie temporal.

La primera capa LSTM devuelve una secuencia completa de salidas para cada paso de tiempo en la serie temporal, que luego se utiliza como entrada para la segunda capa LSTM. La segunda capa LSTM produce una única salida que se alimenta a la capa de salida Dense, que predice la venta en el siguiente paso de tiempo.

Al utilizar dos capas LSTM, la red neuronal puede aprender a representar patrones complejos en la serie temporal. La primera capa LSTM puede capturar patrones a nivel local, mientras que la segunda capa LSTM puede aprender patrones a nivel global. Esto puede aumentar la precisión del modelo al predecir la venta en el siguiente paso de tiempo en la serie temporal.

## Evaluación del Modelo

![image](https://github.com/Ziiredd/Project/assets/116692880/0192f7d2-f61a-4bff-ac52-777fff806ba1)

![image](https://github.com/Ziiredd/Project/assets/116692880/7cbf7155-9dcb-4612-b2f2-1c9d4ef2d011)


## Conclusiones y Recomendaciones

Para el proyecto en cuestión, se propone realizar una búsqueda exhaustiva de hiperparámetros mediante el método de GridSearch con el fin de mejorar aún más el modelo. Sin embargo, es importante tener en cuenta que debido a limitaciones de GPU, no se pudo ejecutar el código en el notebook. A continuación, se detallará el procedimiento que se habría seguido para llevar a cabo esta búsqueda:

Definición de los hiperparámetros: En primer lugar, se identificaron los hiperparámetros del modelo que se deseaban optimizar, como la tasa de aprendizaje, el número de capas ocultas, la función de activación, el tamaño del lote, entre otros.

Definición del rango de búsqueda: Se estableció un rango de valores para cada hiperparámetro que se consideró relevante. Este rango debía ser lo suficientemente amplio para explorar diversas configuraciones, pero al mismo tiempo, debía tener en cuenta las limitaciones computacionales.

Creación de la tabla de búsqueda: Se generó una tabla de búsqueda que contenía todas las combinaciones posibles de valores de hiperparámetros dentro de los rangos establecidos. Cada combinación representaba una configuración única del modelo.

Entrenamiento y validación del modelo: Para cada configuración de hiperparámetros en la grilla de búsqueda, se habría realizado el entrenamiento del modelo utilizando los datos de entrenamiento y se habría evaluado su rendimiento utilizando los datos de validación. Se habría utilizado una métrica de evaluación adecuada para comparar y seleccionar los mejores modelos.

Selección del mejor modelo: Una vez finalizada la búsqueda exhaustiva, se habría seleccionado el modelo que obtuvo el mejor rendimiento según la métrica establecida. Se habría tenido en cuenta tanto el rendimiento en los datos de entrenamiento como en los datos de validación para evitar problemas de sobreajuste.

Evaluación del modelo final: Para obtener una estimación más realista del rendimiento del modelo seleccionado, se habría evaluado utilizando un conjunto de datos independiente, como un conjunto de prueba o un conjunto de validación final.
