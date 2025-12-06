# Descripción del Dataset: Diabetes Health Indicators Dataset

The dataset for this competition (both train and test) was generated from a deep learning model trained on the Diabetes Health Indicators Dataset. Feature distributions are close to, but not exactly the same, as the original. Feel free to use the original dataset as part of this competition, both to explore differences as well as to see whether incorporating the original in training improves model performance. diagnosed_diabetes is the target, and for the testing data, you should predict the probability of diagnosed_diabetes

## Resumen General

Este dataset, creado por Mohan Krishna Thalla, contiene **100,000 registros de pacientes** y está diseñado para la **predicción de riesgo de diabetes**, análisis y aplicaciones de aprendizaje automático (*Machine Learning*). El conjunto de datos es limpio, preprocesado y listo para ser utilizado en tareas de clasificación, regresión y análisis exploratorio.

* **Filas:** 100,000
* **Columnas:** Más de 35
* **Archivo:** `diabetes_dataset.csv`

***

## Características del Dataset

El dataset incluye perfiles de pacientes con características clave basadas en:

1.  **Datos Demográficos:** Edad, género, origen étnico, nivel educativo y nivel de ingresos.
2.  **Estilo de Vida:** Estado de fumador, consumo de alcohol, minutos de actividad física semanal, puntuación de la dieta, horas de sueño y tiempo de pantalla.
3.  **Historial Médico:** Historial familiar de diabetes, hipertensión e historial cardiovascular.
4.  **Mediciones Clínicas:** IMC, relación cintura-cadera, presión arterial (sistólica/diastólica), frecuencia cardíaca, niveles de colesterol (total, HDL, LDL), triglicéridos, glucosa (en ayunas y post-comida), nivel de insulina y HbA1c.

### Columnas Clave

| Columna | Tipo de Dato | Descripción | Rango/Valores Ejemplos |
| :--- | :--- | :--- | :--- |
| **age** | Integer | Edad del paciente en años | 18 – 90 |
| **bmi** | Float | Índice de Masa Corporal (kg/m²) | 15 – 45 |
| **smoking_status** | String | Comportamiento de fumador | 'Never', 'Former', 'Current' |
| **family_history_diabetes** | Integer | Antecedentes familiares de diabetes | 0 = No, 1 = Sí |
| **systolic_bp** | Integer | Presión arterial sistólica (mmHg) | 90 – 180 |
| **hba1c** | Float | HbA1c (%) | 4 – 14 |
| **glucose_fasting** | Float | Glucosa en ayunas (mg/dL) | 70 – 250 |
| **diabetes_risk_score** | Integer | Puntuación de riesgo (calculada) | 0 – 100 |
| **diabetes_stage** | String | Etapa de la diabetes | 'No Diabetes', 'Pre-Diabetes', 'Type 1', 'Type 2', 'Gestational' |
| **diagnosed_diabetes** | Integer | **Objetivo (Target):** Diagnóstico de Diabetes | 0 = No, 1 = Sí |

***

## Calidad y Uso de los Datos

### Calidad de los Datos

* **Completo:** Sin valores faltantes ni duplicados.
* **Limpio:** Todos los valores caen dentro de rangos médicamente realistas.
* **Distribución del Objetivo:** Aproximadamente el 20-25% de los casos están diagnosticados con diabetes, lo que lo hace balanceado para la clasificación de Machine Learning.

### Casos de Uso Sugeridos

* **Clasificación Binaria:** Predecir `diagnosed_diabetes` (Sí/No).
* **Clasificación Multiclase:** Predecir `diabetes_stage`.
* **Regresión:** Predecir valores continuos como `glucose_fasting`, `hba1c` o `diabetes_risk_score`.
* **Análisis Exploratorio de Datos (EDA) y Visualización:** Explorar tendencias entre los indicadores de estilo de vida y las mediciones clínicas.
