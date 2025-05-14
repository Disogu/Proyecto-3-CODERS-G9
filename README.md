# House Prices Prediction with Traditional Machine Learning

## 🎯 Objetivo del Proyecto
Predecir el precio de viviendas utilizando modelos clásicos de machine learning, con una metodología clara, reproducible y orientada a métricas de regresión.

## 📂 Descripción del Dataset
Se utiliza el dataset `California Housing` de `sklearn.datasets.fetch_california_housing`, que contiene información sobre viviendas en California, como número de habitaciones, ingresos medios, edad de las casas, etc., con el objetivo de predecir el valor medio de las casas por bloque.

## ⚖️ Decisiones Tomadas en el Modelado
- Selección de características con información mutua y comparación con otras técnicas como correlación.
- Comparación de algoritmos de regresión con LazyPredict.
- Métrica principal: Mean Squared Error (MSE), por penalizar fuertemente errores grandes.
- Registro de métricas y modelos con MLflow.

## 📈 Resultados y Métricas Principales
- Mejor modelo: GradientBoostingRegressor
- MSE: 0.25
- MAE: 0.39

## ⚙️ Instrucciones para Ejecutar el Proyecto

1. Clona este repositorio:
```bash
git clone https://github.com/tu_usuario/house_prices_regression_project.git
cd house_prices_regression_project
```

2. Instala las dependencias:
```bash
pip install -r requirements.txt
```

3. Ejecuta los notebooks en orden:
   - `1_EDA.ipynb`: análisis exploratorio del dataset.
   - `2_preprocessing.ipynb`: normalización y selección de características.
   - `3_train_validate_model.ipynb`: comparación de modelos con LazyPredict y logging con MLflow.
   - `4_evaluation_export.ipynb`: evaluación final y exportación del modelo.

4. Opcional: iniciar el servidor MLflow
```bash
mlflow ui
```
Accede en `http://localhost:5000` para visualizar los experimentos.

---

Proyecto desarrollado siguiendo el flujo de trabajo recomendado por Pau Labarta.
