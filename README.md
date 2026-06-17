# Predicción y análisis de estrategias de carrera en Fórmula 1 mediante aprendizaje automático

Trabajo de Fin de Máster — Máster Universitario en Inteligencia Artificial
Universidad Internacional de La Rioja (UNIR)

**Autor:** Francisco José Moreno Bayona
**Director:** Inmaculada Tomeo Reyes
**Año:** 2026

## Descripción

Este repositorio contiene el código y los datos del TFM, que aborda la
predicción de las paradas en boxes en Fórmula 1 mediante una comparativa
sistemática de modelos de aprendizaje automático. Se formulan dos tareas:

- **Clasificación binaria:** predecir si se produce una parada en una vuelta dada.
- **Regresión:** predecir el número de vueltas restantes hasta la próxima parada.

Los datos provienen de las fuentes públicas FastF1 y Jolpica-F1, y abarcan
el periodo 2022-2025 (era reglamentaria de efecto suelo).

## Estructura del repositorio

El flujo de trabajo se organiza en notebooks Jupyter que deben ejecutarse
en orden:

| Notebook | Contenido |
|----------|-----------|
| `01_Recopilacion_Preprocesado.ipynb` | Recopilación de datos desde FastF1 y Jolpica-F1 |
| `02_Analisis_Preparacion.ipynb` | Análisis exploratorio y preparación de los datos |
| `03_Entrenamiento_Evaluacion.ipynb` | Modelos de la línea base |
| `04_Optimizacion_Hiperparametros.ipynb` | Optimización de hiperparámetros |
| `05_Ingenieria_Features_Avanzada.ipynb` | Ingeniería avanzada de características |
| `06_Modelos_Adicionales_SVM_LogReg.ipynb` | Ampliación con modelos lineales |
| `07_Correccion_Gaps.ipynb` | Validación por grupos (GroupKFold) |
| `08_Analisis_Shap.ipynb` | Análisis de interpretabilidad (SHAP) |

## Requisitos

- Python 3.9
- Las dependencias se indican en la memoria del TFM (Tabla 10). Las principales son:
  scikit-learn, XGBoost, LightGBM, SHAP, pandas, NumPy, FastF1, matplotlib y seaborn.

## Cómo reproducir los experimentos

1. Clonar el repositorio.
2. Instalar las dependencias.
3. Ejecutar los notebooks en el orden indicado en la tabla anterior.

## Datos

El dataset principal (`dataset_clasificacion.csv`) se incluye en la carpeta
`datasets/`. Los modelos entrenados y los resultados intermedios se generan
al ejecutar los notebooks.

## Licencia

[MIT, o el texto que corresponda según tu elección]
