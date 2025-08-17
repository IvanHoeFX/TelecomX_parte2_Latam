# 📊 Churn Prediction en TelecomX (Latam)

Este proyecto desarrolla un sistema de **predicción de churn** para clientes de TelecomX en Latinoamérica, utilizando modelos de **Machine Learning** y técnicas de **balanceo de clases** (SMOTE). El objetivo es identificar con precisión qué clientes tienen mayor probabilidad de abandonar el servicio y proveer un informe claro con resultados y visualizaciones.

---

## 🗂️ Estructura del repositorio

```
├── data/                  # Datos crudos o procesados (no incluidos por privacidad)
├── notebooks/             # Notebooks Jupyter con el desarrollo paso a paso
├── src/                   # Scripts Python reutilizables
├── docs/
│   └── report/            # Reportes en formato .md o .pdf
│       └── final_report.md
├── README.md              # Este archivo
└── requirements.txt       # Librerías necesarias
```

---

## ⚙️ Instalación

1. Clonar este repositorio:
   ```bash
   git clone https://github.com/tu_usuario/telecomx-churn-latam.git
   cd telecomx-churn-latam
   ```

2. Crear y activar un entorno virtual:
   ```bash
   python -m venv venv
   source venv/bin/activate   # En Linux/Mac
   venv\Scripts\activate      # En Windows
   ```

3. Instalar dependencias:
   ```bash
   pip install -r requirements.txt
   ```

---

## 📈 Metodología

1. **Preprocesamiento de datos**
   - Imputación de valores faltantes
   - Estandarización de variables numéricas
   - Codificación *One-Hot Encoding* para variables categóricas

2. **Modelos implementados**
   - `Logistic Regression`
   - `Random Forest`
   - `Logistic Regression + SMOTE` (para balancear clases)

3. **Evaluación de métricas**
   - Accuracy
   - Precision
   - Recall
   - F1-score
   - ROC-AUC
   - Matriz de confusión
   - Reporte de clasificación

4. **Visualizaciones**
   - Barplots comparativos
   - Heatmaps
   - Radar charts
   - Faceted distributions
   - Line plots de métricas

---

## 🏆 Resultados principales

- El modelo **Random Forest** ofreció mejor **recall** en test, útil para minimizar *false negatives* (clientes que sí abandonan pero no son detectados).
- La **Logistic Regression con SMOTE** mejoró el balance entre *precision* y *recall* en comparación con la versión estándar.
- Las visualizaciones permiten contrastar claramente el rendimiento *train vs test* y analizar posibles **overfitting**.

👉 El detalle completo está en [`docs/report/final_report.md`](docs/report/final_report.md).

---

## 🚀 Próximos pasos

- Optimización de hiperparámetros con **GridSearchCV** o **Optuna**.
- Inclusión de modelos adicionales (XGBoost, LightGBM).
- Implementar un **pipeline de ML en producción** (API con FastAPI o Flask).
- Dashboard interactivo en **Streamlit / Dash** para stakeholders.

---

## 📌 Requisitos

Archivo `requirements.txt` con las librerías clave:

```txt
numpy
pandas
scikit-learn
matplotlib
seaborn
imblearn
```

---

## 👨‍💻 Autor:

**Walter Alcántara S.**  
📧 ivan.alcantarasalazarl@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/ivan-alc%C3%A1ntara-0b17061b9/) | [GitHub](https://github.com/IvanHoeFX)

---