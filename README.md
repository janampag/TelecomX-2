# Predicción de Churn - Telecom X

Este proyecto desarrolla un modelo de Machine Learning para predecir la cancelación de clientes (Churn) en una empresa de telecomunicaciones. El objetivo es identificar a los clientes con alta probabilidad de abandono y proponer estrategias de retención basadas en datos.

## 🛠️ Tecnologías y Librerías
* **Python** (Google Colab)
* **Pandas & NumPy** (Manipulación de datos)
* **Matplotlib & Seaborn** (Visualización)
* **Scikit-learn** (Modelado y Preprocesamiento)
* **Imbalanced-learn (SMOTE)** (Balanceo de clases)

## 📋 Estructura del Proyecto
1. **Preprocesamiento:** Limpieza de datos, eliminación de identificadores únicos y codificación de variables categóricas (One-Hot Encoding).
2. **Análisis Exploratorio (EDA):** Identificación de correlaciones y visualización de patrones de comportamiento entre variables clave.
3. **Tratamiento de Datos:** Balanceo de clases mediante SMOTE y estandarización de variables numéricas con `StandardScaler`.
4. **Modelado:** Implementación y comparación de Regresión Logística y Random Forest.
5. **Evaluación:** Análisis de métricas (Accuracy, Precision, Recall, F1-Score) y Matriz de Confusión.

## 🚀 Resultados del Modelo
El modelo seleccionado fue **Random Forest** debido a su capacidad para maximizar el **Recall**, crucial para detectar la mayor cantidad de cancelaciones posibles.

| Métrica | Resultado |
| :--- | :--- |
| **Accuracy** | ~85% |
| **Recall** | ~82% |
| **F1-Score** | 0.83 |



## 📈 Hallazgos Principales
* **Contratos Mensuales:** Representan el mayor riesgo de abandono.
* **Cargos Mensuales:** Los clientes con facturación superior al promedio tienden a desertar en los primeros meses.
* **Fidelización Temprana:** Los primeros 6 a 12 meses de contrato son el periodo crítico de fuga.

## 💡 Estrategias Sugeridas
* Migración dirigida de clientes con contrato mensual a contratos de mayor duración.
* Programas de soporte técnico prioritario durante el primer semestre de servicio.
* Ajustes de planes proactivos para clientes con cargos mensuales elevados.

## ⚙️ Cómo ejecutar
1. Clonar el repositorio.
2. Cargar el archivo `datos_tratados.csv` generado en la etapa de limpieza.
3. Ejecutar el notebook en Google Colab o un entorno Jupyter local.
