# Definición de los datos

## Origen de los datos

- En este proyecto, nos enfocaremos en analizar el comportamiento de la demanda histórica de productos de una multinacional de distribución de materias primas, centrándonos específicamente en un commoditie conocido como Glicerina. Obtendremos los datos necesarios directamente de las bases de datos del ERP SAP de la compañía. Estos datos proporcionarán información clave sobre las tendencias, patrones y variaciones en la demanda de Glicerina a lo largo del tiempo.

## Especificación de los scripts para la carga de datos

- Se utilizó un notebook de Python para llevar a cabo el análisis exploratorio de datos con el fin de determinar si era necesario realizar un preprocesamiento. El objetivo era preparar el conjunto de datos para su uso en un modelo de machine learning.

## Referencias a rutas o bases de datos origen y destino

- El conjunto de datos o base de datos utilizada fue descargada del sistema ERP SAP de la compañía.

### Rutas de origen de datos

- El dataset se encontraba en una base del ERP SAP.
- El dataset es en formato de excel.
- Se realizo la identificación y contabilización de valores faltantes o nulos, se realizo limpieza. Se eliminaron columnas no relevantes para el objetivo, reiniciamos indices, renombramos columnas, creamos columnas, generamos nuevo dataframe.

![image](https://github.com/Ziiredd/Project/assets/116692880/c15f7b6f-4823-479c-a36f-42f2762fcb11)

### Base de datos de destino

- [ ] Especificar la base de datos de destino para los datos.
- [ ] Especificar la estructura de la base de datos de destino.
- [ ] Describir los procedimientos de carga y transformación de los datos en la base de datos de destino.
