
# 📊 Informe Final del Proyecto de Clasificación

## 1. Introducción
El presente informe resume el desarrollo, análisis y resultados de un proyecto de clasificación supervisada utilizando **Regresión Logística** y **Random Forest**.  
El objetivo principal fue evaluar el rendimiento de ambos modelos sobre un conjunto de datos estructurados con variables numéricas y categóricas, aplicando técnicas de preprocesamiento, balanceo de clases (SMOTE) y comparación de métricas.

---

## 2. Preparación de los Datos
- **Variables numéricas:** imputación de valores faltantes con la mediana y escalado con *StandardScaler*.
- **Variables categóricas:** imputación de la moda y codificación con *OneHotEncoder*.
- **Pipeline de preprocesamiento:** garantizó consistencia entre *train* y *test*.

Adicionalmente, se probó la técnica **SMOTE** para mitigar el desbalance de clases.

---

## 3. Modelos Entrenados
- **Regresión Logística (LR):**
  - Algoritmo lineal, interpretable, con coeficientes y *odds ratio*.
  - Se aplicó también con SMOTE para mejorar el equilibrio de clases.
- **Random Forest (RF):**
  - Modelo de ensamble basado en árboles de decisión.
  - Permite calcular la importancia relativa de cada variable.

---

## 4. Evaluación de Modelos
Se utilizaron las siguientes métricas en *train* y *test*:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**
- **ROC AUC**

### 4.1 Resultados principales
- Ambos modelos alcanzaron un rendimiento competitivo en *Accuracy* y *ROC AUC*.
- La **Regresión Logística** ofrece interpretabilidad mediante coeficientes y *odds ratios*.
- El **Random Forest** mostró mejor desempeño en Recall y F1, aprovechando su capacidad de modelar relaciones no lineales.
- El uso de **SMOTE** mejoró el Recall, reduciendo falsos negativos, aunque con ligero sacrificio en Precision.

---

## 5. Visualización de Resultados
Se generaron múltiples gráficas para comparar modelos y métricas:

- **Barras agrupadas:** comparación directa de métricas entre LR y RF (Train vs Test).
- **Heatmap:** mapa de calor con todas las métricas en una sola vista.
- **Radar Charts:** comparaciones gráficas radiales entre métricas de cada modelo.
- **Line plots:** evolución de métricas entre los diferentes experimentos.
- **Distribuciones facetadas:** exploración de la variabilidad de métricas.

---

## 6. Interpretación de Variables
- **Regresión Logística:** análisis de coeficientes y *odds ratio* permitió identificar qué variables aumentan o disminuyen la probabilidad de la clase positiva.
- **Random Forest:** análisis de *feature importances* destacó las variables más influyentes en las predicciones.

---

## 7. Conclusiones
1. Ambos modelos resultan útiles para el problema de clasificación.
2. **Random Forest** ofrece mayor capacidad predictiva, especialmente en Recall y F1.
3. **Regresión Logística** es preferida cuando se requiere interpretabilidad del modelo.
4. La técnica de **SMOTE** contribuyó a mejorar la capacidad de detección de la clase minoritaria.
5. Las visualizaciones facilitaron la interpretación de métricas y desempeño comparativo.

---

## 8. Recomendaciones
- Utilizar **Random Forest** en escenarios donde el Recall sea crítico (ej. detección de fraude o enfermedades).
- Usar **Regresión Logística** cuando la prioridad sea explicar los factores que influyen en la clasificación.
- Seguir evaluando con técnicas adicionales de balanceo y ajuste de hiperparámetros.
- Documentar y versionar los experimentos para mejorar la reproducibilidad.

---

## 9. Archivos Generados
- `README.md`: guía general del proyecto.
- `informe_final.md`: este documento con explicación detallada.
- Scripts en Python para entrenamiento, evaluación y visualización.

---

✍️ **Autor:** WALTER IVAN ALCANTARA SALAZAR  
📅 **Fecha:** AGOSTO - 2025
