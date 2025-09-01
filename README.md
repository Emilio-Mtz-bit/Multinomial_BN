# Análisis de Patrones de Movilidad Urbana mediante Redes Bayesianas

Este repositorio contiene el análisis de patrones de movilidad urbana utilizando redes bayesianas para modelar las relaciones causales entre características socioeconómicas, demográficas y decisiones de transporte en la Zona Metropolitana del Valle de México.

## Datos

- **Fuente**: Encuesta Origen-Destino 2017 de la Zona Metropolitana del Valle de México (INEGI)
- **Dataset original**: `tviaje.csv` con información detallada sobre viajes realizados
- **Datasets procesados**: Disponibles en `data/processed/` y `data/final/`

## Objetivos

Responder consultas probabilísticas específicas sobre comportamientos de movilidad:

1. **Query 1**: Probabilidad de uso de transporte no motorizado según estrato socioeconómico
2. **Query 2**: Patrones de uso de autobús por mujeres en diferentes localidades  
3. **Query 3**: Frecuencia de viajes en automóvil por estudiantes mujeres
4. **Query 4**: Comparación entre transporte motorizado y no motorizado según duración del viaje

##  Metodología

- **Modelos DAG**: Directed Acyclic Graph que capturan diferentes perspectivas de análisis
- **Herramientas**: R con paquetes `bnlearn` y `Rgraphviz`
- **Evaluación**: Criterios BIC y análisis de fortaleza de arcos

## 📁 Estructura del Proyecto

```
├── data/
│   ├── raw/           # Datos originales de la encuesta
│   ├── processed/     # Datasets procesados
│   └── final/         # Datasets finales para análisis DAG
├── code/
│   ├── preprocessing/ # Scripts de preprocesamiento de datos
│   ├── analysis/      # Análisis exploratorio y queries
│   └── models/        # Construcción de modelos DAG
├── docs/
    ├── articles/      # Artículo científico y documentación
```

## Principales Hallazgos

- **Factor determinante**: El estrato socioeconómico es el principal factor en las decisiones de movilidad
- **Transporte no motorizado**: Mayor uso en estratos bajos vs estratos altos
- **Transporte público**: Baja utilización (11%) en mujeres de localidades medias
- **Viajes cortos**: Distribución equitativa entre transporte motorizado (53%) y no motorizado (47%)

## Autores

- José Emilio Martínez Hernández (A01403100)
- Josué Tapia Hernández (A01621056)  
- Andrés Martínez Almazán (A01621042)
- Diego Arechiga Bonilla (A01621045)

## Uso

1. Los datos originales se encuentran en `data/raw/eod_2017_csv/`
2. Ejecutar scripts de preprocessing en `code/preprocessing/`
3. Realizar análisis con scripts en `code/analysis/` y `code/models/`
   
## Documentación

- **Artículo completo**: `docs/articles/articulo_bn_viajes.tex`
- **PDF**: `docs/articles/Análisis de patrones de movilidad urbana mediante redes bayesianas.pdf`

#
