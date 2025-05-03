# 🎧 Clasificación Supervisada con Datos de Spotify

Este proyecto aplica técnicas de aprendizaje supervisado para clasificar canciones utilizando un conjunto de datos de características de audio de Spotify. Se evalúan diferentes modelos de machine learning con un enfoque práctico y técnico.

---

## 📌 Objetivo

Explorar, preprocesar y entrenar modelos de clasificación que permitan predecir si una canción es popular o no, basándose en variables como `acousticness`, `danceability`, `energy`, entre otras.

---

## 🧠 Modelos Evaluados

Se entrenaron y compararon los siguientes modelos de clasificación:

- **Regresión Logística**
- **Árbol de Decisión**
- **K-Nearest Neighbors (KNN)**
- **Random Forest**

---

## 🛠️ Flujo del Proyecto

1. **Análisis Exploratorio de Datos (EDA)**  
   - Distribución de variables
   - Correlaciones
   - Detección de valores atípicos

2. **Preprocesamiento**  
   - Imputación de valores faltantes (si aplica)  
   - Normalización de variables numéricas  
   - Codificación One-Hot para variables categóricas

3. **Entrenamiento y Validación**  
   - División entrenamiento/test
   - Validación cruzada (Stratified K-Fold)
   - Métricas: Accuracy, F1-Score, ROC AUC

4. **Comparación de Resultados**  
   - Evaluación conjunta de modelos en test y validación cruzada
   - Visualización de métricas

---

## 📊 Resultados Finales

## 📊 Resultados Finales

```
+----------------------+----------------+----------------+-----------+------------------+------------------+------------+
| Modelo               | Accuracy (CV)  | F1-Score (CV)  | AUC (CV)  | Accuracy (Test)  | F1-Score (Test)  | AUC (Test) |
+----------------------+----------------+----------------+-----------+------------------+------------------+------------+
| Logistic Regression  |     0.653      |     0.653      |  0.654    |      0.686       |      0.686       |   0.731    |
| Decision Tree        |     0.721      |     0.721      |  0.721    |      0.678       |      0.677       |   0.754    |
| KNN                  |     0.698      |     0.696      |  0.699    |      0.720       |      0.720       |   0.793    |
| Random Forest        |     0.777      |     0.777      |  0.777    |      0.755       |      0.755       |   0.840    |
+----------------------+----------------+----------------+-----------+------------------+------------------+------------+
```
> El modelo de **Random Forest** tuvo el mejor desempeño general, superando al resto en todas las métricas de validación y prueba.

---

## 🧪 Conclusiones

- El uso de pipelines permitió un preprocesamiento reproducible y eficiente.
- Random Forest demostró ser el modelo más robusto, tanto en entrenamiento como en test.
- KNN ofreció un buen rendimiento, particularmente en la métrica AUC.
- Este proyecto demuestra el potencial de aplicar modelos de machine learning a contextos musicales, útil para sistemas de recomendación o análisis de tendencias.

---

## 📚 Dataset

**Spotify Classification Dataset**  
Fuente: [Kaggle - Spotify Classification](https://www.kaggle.com/datasets/geomack/spotifyclassification)

---

## 👩‍💻 Autor

Proyecto realizado por Manuela Botero Buitrago

