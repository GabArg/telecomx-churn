# Telecom X – Parte 2: Predicción de Cancelación (Churn)

Este repositorio contiene el pipeline para predecir **churn** en **Telecom X** (Parte 2).  
Incluye preparación de datos, correlación/selección de variables, modelos (Logística, KNN, Random Forest), SMOTE y evaluación.

## 📁 Estructura
```
.
├─ notebooks/
│  └─ TelecomX_Parte2_Churn_EXT.ipynb   # Notebook principal (Colab-friendly)
├─ src/                                  # (opcional) Código reutilizable
├─ data/                                  # Archivos de datos (ignorado por git)
│  └─ README.md                           # Instrucciones para obtener datos
├─ reports/
│  └─ figures/                            # Gráficos para el informe
├─ requirements.txt
├─ .gitignore
├─ LICENSE
└─ README.md
```

## 🚀 Cómo ejecutar en Colab
1. Sube el notebook `notebooks/TelecomX_Parte2_Churn_EXT.ipynb` a Colab.  
2. Monta Google Drive y apunta a tu `datos_tratados.csv`.  
3. (Si hace falta) instala dependencias: `pip install -q imbalanced-learn`.

## 🧱 Requisitos (para ejecución local)
```bash
pip install -r requirements.txt
```

## 🗂️ Datos
- Los datasets no se versionan en git por tamaño y privacidad.  
- Coloca los CSV en `data/` (la carpeta está ignorada por git).  
- Sigue las instrucciones en `data/README.md`.
