# Project Charter - Entendimiento del Negocio

## Nombre del Proyecto

Estimación de series de tiempo basadas en el comportamiento de la demanda de un producto de consumo.

## Objetivo del Proyecto

El objetivo de este proyecto es entrenar, validar y desplegar un modelo de *deep learning* que use como insumo para la predicción de la demanda de cualquier productos del portafolio de la compañía.

## Alcance del Proyecto

### Incluye:

- **Descripción de los datos disponibles:**

Para el desarrollo del proyecto se utilizará el conjunto de datos que contiene el consumo histórico de los productos del portafolio de la compañia, nos enfocaremos en el comportamiento de la glicerina en Colombia, el origen de los datos es el ERP SAP de la compañía, datos de Enero 2021 a Abril 2023.

- **Criterios de éxito del proyecto**

 - Un modelo que generé predicciones con alta precisión.
 - Un servicio que procese los archivos que contienen la información de la demanda en el tiempo de los productos.
 
### Excluye:

- [Descripción de lo que no está incluido en el proyecto]

## Metodología

En este proyecto, emplearemos la metodología de Redes Neuronales Recurrentes (LSTM) para realizar predicciones de series de tiempo. Las LSTM son un tipo de red neuronal especialmente diseñada para capturar patrones a largo plazo en secuencias temporales. Mediante el entrenamiento de la red con datos históricos, buscamos generar predicciones precisas y confiables para futuros puntos en la serie. Este enfoque nos permitirá aprovechar la capacidad de las LSTM para modelar la dependencia temporal en los datos, brindando insights valiosos para la toma de decisiones basadas en pronósticos de series de tiempo.

## Cronograma

| Etapa | Duración Estimada | Fechas |
|------|---------|-------|
| Entendimiento del negocio y carga de datos | 2 semanas | del 5 de junio al 9 de junio |
| Preprocesamiento, análisis exploratorio | 4 semanas | del 12 de junio al 16 de junio |
| Modelamiento y extracción de características | 4 semanas | del 19 de junio al 23 de junio |
| Despliegue | 2 semanas | del 26 de julio al 3 de junio |
| Evaluación y entrega final | 3 semanas | del 3 de julio al 7 de julio |

Hay que tener en cuenta que estas fechas son una estimación.

## Equipo del Proyecto

- Edward Aguilar Quitian 
  
## Presupuesto

[Descripción del presupuesto asignado al proyecto]

## Stakeholders

- Junta directiva de la compañia, Universidad Nacional.
- El área de planeación infiere en el comportamiento de la demanda con la planificación de la demanda y la gestión de inventario de la compañía.
- La expectativa es contar con modelo que nos permite ejecutar un proceso de predicción para cualquier serie de tiempo.

## Aprobaciones

- Juan Malagón
- [Firma del aprobador]
- [Fecha de aprobación]
