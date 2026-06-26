# 🏦 Credit Scoring Avanzado & Arquitectura MLOps
**Círculo de Ciencia de Datos y Econometría (CCDE) - UNMSM**  
*Área de Proyectos de Ciencia de Datos*

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.3%2B-orange?logo=scikit-learn&logoColor=white)
![Optuna](https://img.shields.io/badge/Optuna-Bayesian_Optimization-blueviolet)
![Status](https://img.shields.io/badge/Status-Completado-success)

## 📌 Descripción del Proyecto
Este es el proyecto inaugural del área de Ciencia de Datos del CCDE. Nuestro objetivo no es solo entrenar un modelo predictivo, sino simular el flujo de trabajo riguroso de un analista cuantitativo en el sector financiero. 

Hemos desarrollado un sistema de clasificación para la aprobación de créditos (Credit Scoring) comparando el estándar regulatorio de la banca tradicional (Regresión Logística + Weight of Evidence) frente a un algoritmo de Machine Learning de mayor complejidad (Random Forest Classifier).

## 🚀 Puntos Fuertes de Ingeniería (Tech Highlights)
A diferencia de los enfoques académicos tradicionales, este proyecto implementa estándares de la industria (MLOps Base):
* **Prevención Absoluta de Data Leakage:** Uso de `Pipeline` y `ColumnTransformer` de Scikit-Learn para aislar los conjuntos de entrenamiento y prueba.
* **Transformadores Personalizados:** Creación de clases propias heredando de `BaseEstimator` y `TransformerMixin` para automatizar la generación de ratios financieros y la sumatoria de activos.
* **Algoritmia WoE (Weight of Evidence):** Implementación de un codificador dinámico que selecciona variables basado en el *Information Value (IV)*.
* **Optimización Bayesiana:** Búsqueda eficiente de hiperparámetros utilizando la librería `Optuna` bajo validación cruzada estratificada.

## 📊 Nota Analítica: El "Problema" de las Métricas Perfectas
Al ejecutar este notebook, los modelos alcanzan un ROC-AUC superior a **0.99**. En el mundo real del riesgo crediticio, esto es una señal de alerta. 

A través de nuestro Análisis Exploratorio de Datos (EDA), diagnosticamos la causa: el conjunto de datos (proveniente de Kaggle) es de naturaleza sintética. La variable `cibil_score` (historial crediticio) fue generada con una regla de separación casi determinista (scores < 550 garantizan rechazo). **La lección aquí es metodológica:** la arquitectura del código es impecable y está lista para producción, pero el analista de datos siempre debe cuestionar la naturaleza de su materia prima.

## 📁 Estructura del Repositorio
```text
01_proy_cd_credit_scoring/
│
├── loan_approval_dataset.csv       # Dataset original (Kaggle)
├── loan_prediction_final.ipynb     # Notebook con EDA, Ingeniería de Variables y Modelos
├── credit_scoring_pipeline.joblib  # Pipeline final serializado (Listo para Producción)
└── README.md                       # Documentación del proyecto
