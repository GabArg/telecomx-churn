📌 Telecom X – Parte 2: Predicción de Cancelación (Churn)
🎯 Propósito del análisis
Este proyecto busca predecir la probabilidad de cancelación (churn) de clientes de Telecom X utilizando técnicas de Machine Learning.
El objetivo principal es identificar las variables más influyentes en la cancelación de clientes y construir modelos predictivos para anticipar y reducir la pérdida de clientes.

📂 Estructura del proyecto
'''
telecomx-churn/
│── notebooks/
│   └── TelecomX_Parte2_Churn_EXT.ipynb
│── requirements.txt
│── LICENSE
│── README.md
'''

notebooks/ → cuaderno principal con todo el análisis y modelado.

requirements.txt → librerías necesarias para ejecutar el proyecto.

datos_tratados.csv → dataset procesado (público en Google Drive).

🛠️ Preparación de los datos
Clasificación de variables

Categóricas: género, método_pago, tipo_contrato, etc.

Numéricas: tenure, monthly_charges, total_charges, etc.

Procesamiento

Tratamiento de valores nulos.

Encoding de variables categóricas (One-Hot Encoding).

Normalización de variables numéricas.

Balanceo de clases con SMOTE.

Separación de datos

80% entrenamiento / 20% prueba.

📊 Ejemplos de visualizaciones e insights
Comparativa ROC-AUC

El Random Forest Optimizado presenta una mejora significativa respecto al modelo base, aumentando el ROC-AUC de 0.78 a 0.81.

🧠 Modelado y justificación
Se entrenaron y evaluaron los siguientes modelos:

Regresión Logística

K-Nearest Neighbors (KNN)

Random Forest (base y optimizado)

Se seleccionó Random Forest Optimizado como modelo final debido a su mejor balance entre Recall y ROC-AUC, métricas clave para problemas de churn.

🚀 Ejecución del cuaderno
1️⃣ Instalar dependencias
pip install -r requirements.txt
pip install imbalanced-learn

2️⃣ Cargar datos tratados
Desde Google Drive: 📄 datos_tratados.csv

En Colab:
from google.colab import drive
drive.mount('/content/drive')

import pandas as pd
df = pd.read_csv('/content/drive/MyDrive/ruta/a/datos_tratados.csv')
df.head()
3️⃣ Abrir en Google Colab


📌 Notas
Los datos tratados se encuentran en un enlace público de Google Drive.

El notebook incluye análisis exploratorio (EDA), preparación de datos, búsqueda de hiperparámetros y comparativa de modelos.

Este README cumple con la documentación solicitada, facilitando la comprensión y ejecución del proyecto.

📷 Cómo agregar imágenes al README
En tu repo, crea una carpeta llamada img (en la raíz del proyecto).

Guarda dentro la(s) imagen(es) que quieras mostrar (ejemplo: roc_auc_comparativa.png).

En el README, para mostrar la imagen usa:
![Texto alternativo](img/roc_auc_comparativa.png)


