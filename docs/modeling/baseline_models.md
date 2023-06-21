# Reporte del Modelo Baseline

## Descripción del modelo

El modelo base que utilizaremos será una red neuronal recurrente LSTM (Long Short-Term Memory) es ampliamente utilizada en pronósticos de series de tiempo debido a su capacidad para capturar y modelar patrones complejos a lo largo del tiempo.

## Variables de entrada

Cómo variables de entrada tenemos los registros históricos de las ventas desde 2016 a 2023 del producto seleccionado del portafolio para pronosticar su demanda.

## Variable objetivo

La variable objetivo es el 7mo mes a partir de una ventana de tamaño 6.

## Evaluación del modelo

### Métricas de evaluación

Error medio absoluto (MAE, por sus siglas en inglés): El MAE es una métrica que calcula la diferencia promedio entre los valores pronosticados y los valores reales en términos absolutos. Es una medida de la precisión promedio del pronóstico y se calcula sumando las diferencias absolutas y dividiéndolas por el número total de muestras. Cuanto menor sea el MAE, mejor será el desempeño del modelo.

Error cuadrático medio (MSE, por sus siglas en inglés): El MSE es similar al MAE, pero en lugar de tomar la diferencia absoluta, calcula la diferencia al cuadrado entre los valores pronosticados y los valores reales. Luego, se promedia estas diferencias al cuadrado. El MSE penaliza los errores más grandes de manera más significativa que el MAE. Al igual que el MAE, se busca minimizar el MSE para obtener un mejor rendimiento.

Raíz del error cuadrático medio (RMSE, por sus siglas en inglés): El RMSE es simplemente la raíz cuadrada del MSE. Esta métrica tiene la misma unidad de medida que los datos originales, lo que la hace más interpretable y fácil de comparar con los valores reales. El RMSE también penaliza los errores grandes y se busca minimizarlo.

Porcentaje de error absoluto medio (MAPE, por sus siglas en inglés): El MAPE es una métrica que calcula el error porcentual promedio entre los valores pronosticados y los valores reales. Es especialmente útil cuando se desea evaluar el rendimiento del modelo en términos de precisión porcentual. Se calcula como el promedio de las diferencias porcentuales absolutas entre los valores pronosticados y los valores reales. Un MAPE más bajo indica una mejor precisión del modelo.

### Resultados de evaluación

![image](https://github.com/Ziiredd/Project/assets/116692880/02129236-91a0-4639-a813-d1a5e306814b)

Test Mean Squared Error: 	0.0205
Test Mean Absolute Error: 	0.1188
Test Mean squared log error: 	0.0101

## Análisis de los resultados

Es evidente que los resultados obtenidos no cumplen con las expectativas esperadas.

## Conclusiones

Dado los resultados anteriores de la red neuronal recurrente (RNN), vamos a definir una función de costo que penalice la falta de estructura y observaremos los resultados obtenidos.

La función de coste que utilizaremos tiene como objetivo medir la discrepancia entre la salida de la RNN y la estructura deseada. Penalizará aquellos casos en los que la salida no siga un patrón o no se ajuste adecuadamente a la estructura esperada.

Una vez definida esta función de coste, procederemos a evaluar los resultados de la RNN. Analizaremos cómo se comporta la red en términos de estructura y compararemos los resultados con nuestras expectativas.

Esta evaluación nos permitirá determinar si la RNN está aprendiendo correctamente la estructura deseada y si la función de coste está cumpliendo su propósito de penalizar la falta de estructura. A partir de estos resultados, podremos realizar ajustes y mejoras en el modelo, si es necesario.
