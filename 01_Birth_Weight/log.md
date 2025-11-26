## Readiness
Cambiado a local ahora mismo para

## Train/Validation Split
Evaluar el modelo con los mismos datos con los que se entrena es un error gravísimo que lleva a overfitting.

Dividir train.csv en dos conjuntos

- X_train, y_train: Entrenamiento modelo 80%
- X_val, y_val: Validar y calcular métrica de error 20%

train_test_split de sklearn.model.selection con random_state=42

## Data Cleaning
GIGO (Garbage In Garbage Out)

**Manejo de NaN (valores ausentes)**
inputs usando media o mediana de conjunto de entrenamiento

Calcular media con X_train y usarlo para rellenar X_train, X_val y test.csv (evitar data leakage)

**Variables categóricas**
one-hot encoding o si son complejas eliminarlas completamente

## Baseline setting
antes de entrenar modelo, necesitas saber rendimiento mínimo aceptable

RMSE (Raíz del Error Cuadrático Medio) asumiendo que predices siempre el peso promedio de los bebés del y_train. Cualquier modelo que entrenes después debe tener un error menor a este para ser considerado útil.

## Linear Regression
modelado de peso (X) y bebes (y)
