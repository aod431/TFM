# Data mining for the characterization of aquatic drowning incidents in Spain

Este repositorio contiene el flujo completo de trabajo para el Trabajo de Fin de Máster de Alejandro Ortega de Roman (ado431@alumnos.unican.es), incluyendo todo el código del proyecto en formato notebook `.ipynb` y los datos asociados.

El estudio analiza datos sobre ahogamientos en España (2013–2024) aplicando técnicas de minería de datos para identificar perfiles de riesgo. El objetivo es proponer estrategias preventivas eficaces adaptadas a cada grupo de edad y contexto geográfico.

## Estructura del Proyecto

El proyecto está organizado en dos carpetas principales:

### 1. `scripts/`

Contiene los notebooks y el dataset:

- **Notebooks `.ipynb` principales:**

  - `preparacion.ipynb`  
    Unifica todas las tablas principales y secundarias exportadas de la base de datos Access.  
    Procesos realizados:  
    - Lectura y unificación de tablas.  
    - Renombrado y eliminación de variables.  
    - Generación de un único archivo `.csv` para procesamiento posterior.

  - `buenos_graficos.ipynb`  
    Análisis visual de los datos limpios.  
    Procesos realizados:  
    - Análisis exploratorio de datos (EDA).  
    - Generación de gráficos de distribución.

  - `analisis_estadistico.ipynb`  
    Aplicación de técnicas estadísticas sobre datos limpios.  
    Procesos realizados:  
    - Discretización de la variable "Edad".  
    - Cálculo de correlaciones entre variables.

  - `analisis_descriptivo_predictivo.ipynb`  
    Técnicas de aprendizaje para análisis descriptivo y predictivo.  
    Procesos realizados:  
    - Clustering para identificar patrones en los datos.  
    - Reglas de asociación para descubrir relaciones entre variables.  
    - Árboles de decisión y variantes para clasificación y predicción.

- **Archivos de datos en `scripts/`:**

  - 'ahogamientos_completo.csv` — Datos en estado original, antes de procesamiento.  
  - `ahogamientos-completo-procesado.csv` — Datos limpios y procesados para análisis.  
  - `Spain.json` y `Límites de las Comunidades Autónomas de España.geojson` — Archivos para mapas y gráficos geográficos de España.

---

### 2. `tablas/csv/`

Carpeta que contiene las tablas exportadas desde la base de datos Access en formato `.csv`, las cuales se unifican y procesan en `preparacion.ipynb`.

---

## Requisitos

Para ejecutar los notebooks y scripts, asegúrate de tener instaladas las siguientes librerías de Python:

```bash
pandas
numpy
matplotlib
seaborn
scikit-learn
mlxtend
pyodbc
