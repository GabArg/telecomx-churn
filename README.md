# Telecom X – Parte 2: Predicción de Cancelación (Churn)

Proyecto de Machine Learning para predecir la probabilidad de **cancelación (churn)** en clientes de **Telecom X**.  
Incluye: preparación de datos, correlación/selección de variables, **SMOTE** para balanceo, modelos (Regresión Logística, KNN, Random Forest), evaluación y conclusiones.

---

## 📂 Estructura


---

## 🚀 Ejecutar en Google Colab

Abrí el notebook directo en Colab:  
[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GabArg/telecomx-churn/blob/main/telecomx-churn/notebooks/TelecomX_Parte2_Churn_EXT.ipynb)

> Si cambiás el nombre o la ruta del notebook, actualizá este enlace.

---

## 📥 Datos (públicos en Google Drive)

El CSV **`datos_tratados.csv`** está disponible públicamente.

**Descarga directa (recomendada):**
```python
import pandas as pd
csv_link = "https://drive.google.com/uc?export=download&id=1EcgqqmAklu6AHOxXGBDJscJJTP3nvrUt"
df = pd.read_csv(csv_link)
df.head()
from google.colab import drive
drive.mount('/content/drive')

# Ajustá esta ruta si tu archivo está en otra carpeta
df = pd.read_csv('/content/drive/MyDrive/ruta/a/datos_tratados.csv')
pip install -r requirements.txt
pip install -q imbalanced-learn
