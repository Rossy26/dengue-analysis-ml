# Dengue Analysis - Modelado y Predicción (SIVIGILA 2022-2024)

Resumen
-------
Este repositorio contiene un análisis exploratorio y modelos predictivos para estimar la incidencia de casos de dengue en Colombia usando los registros del SIVIGILA (2022–2024). El trabajo principal se encuentra en el notebook `dengue_notebook.ipynb`, que realiza la carga de datos, limpieza, agregación temporal y la comparación de diversos modelos de regresión y redes neuronales para pronosticar la evolución temporal (diarios) de los casos.

Contenido del repositorio
-------------------------
- `dengue_notebook.ipynb`  
  Notebook principal que documenta todo el flujo: inspección de variables, preprocesamiento, ingeniería de características, entrenamiento y evaluación de modelos (Regresión lineal, Árbol de decisión, Random Forest, MLP y redes profundas), y visualizaciones.
- `data/dengue_dataset.csv`  
  CSV consolidado con los registros de dengue (resultante de unir los años 2022, 2023 y 2024 desde los archivos del SIVIGILA). Este archivo es el que usa el notebook para ejecutar el análisis.
- `requirements.txt` 
  Lista de dependencias 

Acerca del dataset
------------------
- Fuente: Sistema de Vigilancia en Salud Pública (SIVIGILA), Instituto Nacional de Salud (INS), Colombia.  
- Periodo: 2022–2024.  
- Formato: CSV .  


Objetivo
--------
Proyectar la tendencia de casos diarios de dengue (problema de regresión sobre series de tiempo) mediante:
- Modelos lineales como baseline.
- Modelos no lineales (Decision Tree, Random Forest).
- Modelos de redes neuronales (MLP y DNN).
- Evaluación usando TimeSeriesSplit y métricas como MAE, RMSE y R².
