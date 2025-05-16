# Default Prediction - Credit Card Clients (UCI Dataset)

Este proyecto aplica técnicas de machine learning para predecir si un cliente de tarjeta de crédito incurrirá en incumplimiento de pago (default), utilizando el dataset [Default of Credit Card Clients Dataset](https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients) de la UCI Machine Learning Repository.

## 📂 Estructura del Proyecto

```
├── data/                         # Carpeta sugerida para el dataset (descargar manualmente)
├── notebooks/
│   └── ml_project_DCCC.ipynb     # Notebook principal con todo el flujo de trabajo
├── requirements.yml              # Entorno Conda para replicar el proyecto
└── README.md                     # Este archivo
```

---

## ⚙️ Requisitos

- Python 3.10.17 (instalado desde archivo requirements.yml, esta version garantiza la compatibilidad de todos los paquetes)
- Conda (se recomienda usar [Miniconda](https://docs.conda.io/en/latest/miniconda.html) o Anaconda)
-     Importante al instalar conda marcar en la casilla  Add Miniconda3 to my PATH enviroment variable.
- Git (opcional, para clonar el repositorio)
- Instalar en Visual Code la extension Jupyter Notebook

---

## 🚀 Instalación y Ejecución

### 1. Clonar el repositorio (opcional)

```bash
git clone https://github.com/sgurdian/ml_default_credit_card_clients
cd ml_default_credit_card_clients
```

> O descarga el `.zip` desde GitHub y descomprímelo.

---

### 2. Crear el entorno Conda

```bash
conda env create -f requirements.yml
```

> Este comando instalará todas las dependencias necesarias, incluyendo `pandas`, `scikit-learn`, `lightgbm`, `catboost`, `pytorch`, entre otros.




---

### 3. Activar el entorno

```bash
conda activate ml_project_DCCC
```

---

### 4. Descargar el dataset

Descarga el dataset original desde [este enlace directo](https://archive.ics.uci.edu/static/public/350/default+of+credit+card+clients.zip), extráelo y colócalo en la carpeta `data/` con el nombre:

```
data/default_of_credit_card_clients.xls
```

---

### 5. Ejecutar el análisis

Abrir Visual Code y navega hasta la carpeta `notebooks/`:

Abre `ml_project_DCCC.ipynb` y ejecuta todas las celdas usando VSCode con Jupyter integrado.

---

## 📊 ¿Qué se incluye?

- Análisis exploratorio de datos (EDA)
- Preprocesamiento (imputación, encoding, escalamiento)
- Modelado con:
  - Logistic Regression
  - Random Forest
  - Gradient Boosting (LightGBM y CatBoost)
  - Redes Neuronales (MLP y TabNet)
- Manejo de desbalance con SMOTE y BalancedRandomForest
- Optimización de hiperparámetros con GridSearch, RandomizedSearch y BayesSearch
- Métricas: AUC, F1, accuracy, confusion matrix, precision-recall

---

## 🧠 Recomendaciones

- Usa un entorno virtual siempre que puedas.
- Si tienes GPU, verifica la instalación correcta de `torch` y `tensorflow`.
- Si experimentas errores con `pytorch-tabnet`, asegúrate de que `torch` esté instalado antes.

---


## 📝 Licencia

Este proyecto se entrega bajo la Licencia MIT.

---

## 💡 Autor
---
Ing. Salvador Gurdian
Ing. Omar Zuniga

---


