📌 Telecom X – Parte 2: Predicción de Cancelación (Churn)
🎯 Propósito del análisis
Este proyecto busca predecir la probabilidad de cancelación (churn) de clientes de Telecom X utilizando técnicas de Machine Learning.
El objetivo principal es identificar las variables más influyentes en la cancelación de clientes y construir modelos predictivos para anticipar y reducir la pérdida de clientes.

📂 Estructura del proyecto

```
telecomx-churn/
│── notebooks/
│   └── TelecomX_Parte2_Churn_EXT.ipynb
│── requirements.txt
│── LICENSE
│── README.md
```


- `notebooks/` → cuaderno principal con todo el análisis y modelado.  
- `requirements.txt` → librerías necesarias para ejecutar el proyecto.  
- `datos_tratados.csv` → dataset procesado (público en Google Drive).  
- `LICENSE` → licencia del proyecto.  
- `README.md` → documentación del proyecto.  


## 🛠️ Preparación de los datos

### 📌 Clasificación de variables
- **Categóricas:** `género`, `método_pago`, `tipo_contrato`, etc.
- **Numéricas:** `tenure`, `monthly_charges`, `total_charges`, etc.

### 🔄 Procesamiento
1. Tratamiento de valores nulos.
2. Codificación de variables categóricas (**One-Hot Encoding**).
3. Normalización de variables numéricas.
4. Balanceo de clases con **SMOTE**.

### 📂 Separación de datos
- 80% entrenamiento / 20% prueba.

---

## 📊 Ejemplos de visualizaciones e insights

### Comparativa ROC-AUC
El **Random Forest Optimizado** presenta una mejora significativa respecto al modelo base, aumentando el **ROC-AUC** de `0.78` a `0.81`.

![Comparativa ROC-AUC](ruta/a/imagen.png)

---

## 🧠 Modelado y justificación

Se entrenaron y evaluaron los siguientes modelos:

- **Regresión Logística**
- **K-Nearest Neighbors (KNN)**
- **Random Forest** (base y optimizado)

**Métricas evaluadas:**
- Accuracy
- Precisión
- Recall
- F1-Score
- ROC-AUC
- Matriz de confusión

**Conclusión:**  
El modelo **Random Forest Optimizado** fue el que obtuvo el mejor rendimiento en la métrica ROC-AUC, por lo que se selecciona como modelo final recomendado.
