# Telecom X – Parte 2: Predicción de Cancelación (Churn)

Proyecto de Machine Learning para predecir la probabilidad de **cancelación (churn)** en clientes de **Telecom X**.  
Incluye: preparación de datos, correlación/selección de variables, **SMOTE** para balanceo, modelos (Regresión Logística, KNN, Random Forest), evaluación y conclusiones.

---

## 📂 Estructura
```
telecomx-churn/
├── notebooks/
│ └── TelecomX_Parte2_Churn_EXT.ipynb
├── requirements.txt
├── LICENSE
└── README.md
```

---

## 🚀 Ejecutar en Google Colab

Abrí el notebook directo en Colab:  
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GabArg/telecomx-churn/blob/main/telecomx-churn/notebooks/TelecomX_Parte2_Churn_EXT.ipynb)



---

## 📥 Datos (públicos en Google Drive)

El CSV **`datos_tratados.csv`** está disponible públicamente.

**Descarga directa (recomendada):**
```python
import pandas as pd
csv_link = "https://drive.google.com/uc?export=download&id=1EcgqqmAklu6AHOxXGBDJscJJTP3nvrUt"
df = pd.read_csv(csv_link)
df.head()
Desde Google Drive en Colab:
from google.colab import drive
drive.mount('/content/drive')


df = pd.read_csv('[/content/drive/MyDrive/ruta/a/datos_tratados.csv](https://drive.google.com/file/d/1EcgqqmAklu6AHOxXGBDJscJJTP3nvrUt/view?usp=drive_link)')

⚙️ Instalación de dependencias
pip install -r requirements.txt
pip install -q imbalanced-learn


🎯 Objetivos del desafío
Preparación de datos (tratamiento, encoding, normalización si corresponde).

Correlación y selección de variables.

Modelado (al menos dos modelos) — Logística / KNN / Random Forest.

Evaluación (Accuracy, Precision, Recall, F1, ROC-AUC, Matriz de confusión).

Interpretación (importancia de variables / coeficientes) y conclusiones estratégicas.

📝 Notas
No se versionan datasets crudos en el repo.

El dataset se obtiene por enlace público de Drive (ver arriba).

El notebook incluye secciones extra: SMOTE, búsqueda de hiperparámetros y comparativa de modelos.


