# Data mining for the characterization of aquatic drowning incidents in Spain.

Este repositorio contiene un flujo completo de trabajo para el Trabajo de Fin de Master de Alejandro Ortega de Roman, ado431@alumnos.unican.es, conteniendo todo el codigo del proyecto en formato notebook .ipynb

El trabajo consiste en un estudio completo de datos sobre ahogamientos en España (2013–2024) usando técnicas de minería de datos para identificar los perfiles de riesgo. El objetivo es proponer estrategias preventivas eficaces adaptadas a cada grupo de edad y contexto geográfico.

## Estructura del Proyecto


### `preparacion.ipynb`
- **Descripción**: Unifica todas las tablas principales y secundarias de la base de datos Access.
- **Procesos realizados**:
  - Lectura y unificación de las tablas.
  - Renombrado y eliminación de variables.
  - Generación de un único archivo .csv para posterior procesamiento en OpenRefine.

### `buenos_graficos.ipynb`
- **Descripción**: Analiza visualmente los datos limpios.
- **Procesos realizados**:
  - Análisis exploratorio de datos (EDA).
  - Generación de gráficos de distribución.

###  `analisis_estadistico.ipynb`
- **Descripción**: Aplica técnicas estadísticas sobre los datos limpios.
- **Procesos realizados**:
  - Discretización de la variable "Edad".
  - Cálculo de correlaciones entre variables.

### `analisis_descriptivo_predictivo.ipynb`
- **Descripción**: Realiza técnicas de aprendizaje para el análisis descriptivo y predictivo.
- **Procesos realizados**:
  - Clustering para identificar patrones en los datos.
  - Reglas de asociación para descubrir relaciones entre variables.
  - Árboles de decisión y sus variantes para clasificación y predicción.

## Requisitos

Asegúrate de tener instaladas las siguientes librerías de Python:

```bash
pandas
numpy
matplotlib
seaborn
scikit-learn
mlxtend
pyodbc
