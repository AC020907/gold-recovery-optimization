# Gold Recovery Prediction using Machine Learning

## Descripción del proyecto

Este proyecto desarrolla una solución de Machine Learning para predecir la recuperación de oro en un proceso industrial de extracción minera.

La compañía Zyfra busca optimizar la producción mediante modelos predictivos capaces de estimar la eficiencia de recuperación del oro en distintas etapas del proceso de refinamiento. Para ello, se utilizaron datos reales provenientes de sensores y variables operativas de una planta minera.

El proyecto incluye limpieza de datos, análisis exploratorio, ingeniería de características, entrenamiento de modelos y evaluación mediante una métrica personalizada basada en sMAPE.

## Objetivo

Construir un modelo capaz de predecir con precisión la recuperación de oro durante las etapas de procesamiento y concentración, permitiendo mejorar la toma de decisiones operativas y optimizar la eficiencia productiva.

## Datos

Los datos contienen información sobre diferentes etapas del proceso de extracción minera, incluyendo:

- Parámetros de flotación.
- Concentraciones de metales.
- Variables operativas del proceso.
- Mediciones de recuperación de oro.
- Variables de entrada y salida en distintas fases de producción.

Se trabajó con conjuntos de entrenamiento y prueba proporcionados por la empresa.

## Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook

## Metodología

### 1. Preparación de los datos

- Inspección inicial de datasets.
- Tratamiento de valores ausentes.
- Eliminación de variables no disponibles en producción.
- Verificación de consistencia de datos.
- Alineación de conjuntos de entrenamiento y prueba.

### 2. Análisis exploratorio

Se analizaron:

- Distribuciones de variables clave.
- Concentraciones de metales en distintas etapas.
- Comportamiento de las recuperaciones.
- Valores atípicos y observaciones anómalas.

### 3. Ingeniería de características

- Selección de variables relevantes.
- Eliminación de columnas redundantes.
- Preparación de variables objetivo.
- Construcción de conjuntos finales de entrenamiento.

### 4. Entrenamiento de modelos

Se evaluaron diferentes algoritmos de regresión:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

Los modelos fueron comparados mediante validación cruzada.

### 5. Evaluación

La métrica principal utilizada fue:

**sMAPE (Symmetric Mean Absolute Percentage Error)**

Esta métrica permite medir el error porcentual de las predicciones considerando tanto valores altos como bajos de manera equilibrada.

Además, se implementó la métrica final utilizada por Zyfra para evaluar simultáneamente ambas etapas del proceso de recuperación.

## Resultados

Los modelos basados en árboles mostraron un mejor desempeño que la regresión lineal tradicional.

Tras la optimización de hiperparámetros y validación cruzada, se seleccionó el modelo con menor valor de sMAPE para su evaluación final.

Los resultados obtenidos demostraron que el modelo es capaz de capturar patrones relevantes del proceso industrial y producir estimaciones útiles para la operación minera.

## Conclusiones

- Fue posible construir un modelo predictivo para estimar la recuperación de oro en distintas etapas del proceso.
- El análisis exploratorio permitió detectar inconsistencias y variables críticas para la predicción.
- Los modelos de Machine Learning superaron los enfoques base utilizados como referencia.
- La métrica sMAPE permitió evaluar adecuadamente la calidad de las predicciones en un contexto industrial.
- El modelo seleccionado puede utilizarse como herramienta de apoyo para optimizar procesos de recuperación minera.

## Habilidades demostradas

- Limpieza y preparación de datos industriales.
- Análisis exploratorio de datos.
- Ingeniería de características.
- Modelado supervisado de regresión.
- Validación cruzada.
- Optimización de hiperparámetros.
- Implementación de métricas personalizadas.
- Evaluación de modelos de Machine Learning.
- Comunicación de resultados técnicos y de negocio.

## Estructura del repositorio

```text
gold-recovery-prediction-ml/
│
├── data/
│   ├── gold_recovery_train.csv
│   ├── gold_recovery_test.csv
│   └── gold_recovery_full.csv
│
├── notebooks/
│   └── proyecto_sprint_12.ipynb
│
├── README.md
└── requirements.txt
```

## Autor

**Alejandro Cotes**  
Data Science Student | Machine Learning | Analytics
