# TP Análisis de Datos

El objetivo del presente trabajo práctico es preparar y analizar los datos del UCDP Georeferenced Event Dataset (GED) con el fin de construir un conjunto de datos adecuado para el entrenamiento de un modelo de aprendizaje supervisado de clasificación, cuyo propósito será predecir el nivel de letalidad de los eventos de conflicto armado.

Cada registro del dataset representa un evento individual de violencia, por lo que la clasificación se realizará a nivel de evento y no de conflicto.

Para ello, se unificaron y depuraron las estimaciones de muertes (low, best, high) generando la variable best_est_cleaned, una medida continua, coherente y representativa de la cantidad estimada de víctimas por evento.
A partir de esta variable, se definieron tres rangos de letalidad que categorizan los eventos como de baja, media o alta letalidad.

De este modo, el modelo tendrá un enfoque clasificador, y no de regresión, utilizando la variable lethality_class (derivada de best_est_cleaned) como output o variable objetivo.
El objetivo final es dejar el dataset completamente preparado para el entrenamiento posterior de dicho modelo.

Los pasos realizados:
- Exploración y comprensión de los datos
- Aplicación de técnicas de visualización (pevio a la limpieza)
- Plantear un posible problema de ML supervisado a partir de los datos elegidos (Arriba)
- Creacion de la variable de tipo de violencia

Los pasos a seguir
- Realizar la limpieza del dataset:
* Identificar posible candidatos de variables para uso en el modelo y cuales no
* Determinar el tratamiento de los nulls de las vaiables candidatas
* Determinar el tratamiento de los outliers de las variables candidatas (usar tecnicas de estadisticas, rango intercuartil, simetria, usar curtosis para demostrar el acomodo)

* Division en train y test

----------
### VER MAS ADELANTE
* escalar y/o normalizar las variables
* Analizar balance/desbalance
* Reduccion de dimensionalidad