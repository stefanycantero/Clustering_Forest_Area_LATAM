# Análisis de Clustering de Áreas Forestales en Países Latinoamericanos y del Caribe

## Descripción

Este proyecto es un trabajo en equipo realizado por tres estudiantes de Ingeniería de Sistemas e Informática para la asignatura Introducción a la Inteligencia Artificial en la Universidad Nacional de Colombia. Se centra en el análisis de datos forestales para países latinoamericanos y del Caribe utilizando el dataset **forest_area**, que incluye el ranking de HDI en 2018, el nombre del país y datos de área forestal entre 1990 y 2016. Se realiza un análisis detallado empleando técnicas de clustering para identificar patrones y agrupamientos en los datos. El proceso incluye la creación de variables nuevas para medir el cambio neto en el porcentaje de área forestal y el promedio del área forestal para cada país, seguido por un análisis de clustering.

## Proceso del Análisis

### Preprocesamiento y Exploración de Datos

- **Creación de Variables Nuevas**: Se generan dos nuevas variables:
  - **Cambio Neto en % de Área Forestal**: Representa la variación en el porcentaje de área forestal entre 1990 y 2016.
  - **Promedio de Área Forestal**: Promedio del área forestal en los años disponibles.

- **Limpieza de Datos**: Se realiza la limpieza de datos para manejar valores faltantes, convertir tipo de datos y corregir inconsistencias.
- **Exploración de Datos**: Análisis descriptivo de las variables para comprender la distribución y las características de los datos.

### Selección de Número de Clústeres

- **Curva de Codo**: Se utiliza para determinar el número óptimo de clústeres evaluando la suma de errores cuadráticos (SSE) en función del número de clústeres.
- **Estadístico de Gap**: Método para evaluar la cantidad de variación dentro de los clústeres comparado con una referencia aleatoria.
- **Análisis de Silueta**: Evalúa la cohesión y separación de los clústeres obtenidos, proporcionando una medida de la calidad del clustering.

### Implementación de Clustering

- **K-Means Clustering**: Se implementa el algoritmo K-Means utilizando las variables HDI Rank, cambio neto en área forestal, y promedio de área forestal. Se evalúan los clústeres formados y se interpretan los resultados.
- **Agrupamiento Jerárquico**: Se prueba el clustering jerárquico utilizando dendrogramas con los métodos single y Ward para comparar y validar los resultados obtenidos con K-Means.

### Análisis de Resultados

- **Evaluación de Clústeres**: Se analizan las características más representativas para cada uno de los tres clústeres identificados. Se realiza un análisis detallado para entender las diferencias y similitudes entre los países en cada clúster.

## Tecnologías y Librerías Utilizadas

- **Librerías de Python**:
  - `matplotlib` y `seaborn`: Para la visualización de datos y gráficos.
  - `numpy` y `pandas`: Para manipulación y análisis de datos.
  - `sklearn`: Para la implementación de K-Means y análisis de silueta.

## Resultados Esperados

- **Identificación de Clústeres**: Clasificación de los países en grupos homogéneos basados en HDI Rank, cambio neto y promedio de área forestal.
- **Interpretación de Clústeres**: Descripción de las características predominantes en cada clúster y recomendaciones para la gestión forestal en los países analizados.
- **Visualización de Datos**: Gráficos y dendrogramas que ilustran los resultados del clustering y facilitan la interpretación.
