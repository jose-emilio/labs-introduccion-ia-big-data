# Laboratorios: Introducción a la IA y al Big Data

Colección de notebooks Jupyter organizados en tres bloques temáticos: análisis exploratorio de datos, preprocesamiento y entrenamiento de modelos de machine learning.

## Estructura

```
.
├── eda/                          # Análisis Exploratorio de Datos
│   ├── Matplotlib/               # Visualizaciones con Matplotlib
│   │   └── world-happiness.ipynb
│   ├── Seaborn/                  # Visualizaciones con Seaborn
│   │   └── world-happiness.ipynb
│   └── Plotly/                   # Visualizaciones interactivas con Plotly
│       ├── Gapminder/
│       │   └── gapminder_visualizations.ipynb
│       └── CO2PerCapita/
│           └── co2-per-capita.ipynb
│
├── preprocesamiento/             # Preprocesamiento de datos
│   ├── automoviles/
│   │   └── automoviles.ipynb
│   └── calidad-aire/
│       └── calidad_aire_solucion.ipynb
│
└── training/                     # Entrenamiento de modelos
    ├── cancer-mama/
    │   └── clasificacion_binaria_cancer_mama.ipynb
    ├── series-temporales/
    │   ├── temperaturas.ipynb
    │   └── vuelos.ipynb
    ├── telco-churn/
    │   └── telco-churn.ipynb
    └── trafico/
        └── trafico.ipynb
```

## Laboratorios

### EDA — Análisis Exploratorio de Datos

| Notebook | Dataset | Librería | Descripción |
|----------|---------|----------|-------------|
| [world-happiness.ipynb](eda/Matplotlib/world-happiness.ipynb) | World Happiness Report 2015–2021 | Matplotlib | Gráficos de líneas, barras, histogramas, tartas y dispersión para analizar la felicidad por país |
| [world-happiness.ipynb](eda/Seaborn/world-happiness.ipynb) | World Happiness Report 2015–2021 | Seaborn | Mismo análisis con la capa estadística de Seaborn |
| [gapminder_visualizations.ipynb](eda/Plotly/Gapminder/gapminder_visualizations.ipynb) | Gapminder | Plotly | Visualizaciones interactivas de desarrollo mundial (PIB, esperanza de vida, población) |
| [co2-per-capita.ipynb](eda/Plotly/CO2PerCapita/co2-per-capita.ipynb) | CO₂ per cápita | Plotly | Análisis geográfico e histórico de emisiones de CO₂ |

### Preprocesamiento

| Notebook | Dataset | Descripción |
|----------|---------|-------------|
| [automoviles.ipynb](preprocesamiento/automoviles/automoviles.ipynb) | Automóviles | Limpieza, valores faltantes, codificación y normalización de datos tabulares |
| [calidad_aire_solucion.ipynb](preprocesamiento/calidad-aire/calidad_aire_solucion.ipynb) | Calidad del aire | Preprocesamiento de datos ambientales con manejo de outliers y transformaciones |

### Entrenamiento de Modelos

| Notebook | Dataset | Técnica | Descripción |
|----------|---------|---------|-------------|
| [clasificacion_binaria_cancer_mama.ipynb](training/cancer-mama/clasificacion_binaria_cancer_mama.ipynb) | Breast Cancer Wisconsin | Regresión Logística, Árbol de Decisión | Clasificación binaria con métricas de evaluación (accuracy, precision, recall, AUC-ROC) |
| [temperaturas.ipynb](training/series-temporales/temperaturas.ipynb) | Temperaturas mínimas Melbourne 1981–1990 | Promedio móvil | Introducción a series temporales, estacionalidad y predicción con MAE/RMSE |
| [vuelos.ipynb](training/series-temporales/vuelos.ipynb) | Datos de vuelos | Series temporales | Análisis y predicción de series temporales en el contexto de tráfico aéreo |
| [telco-churn.ipynb](training/telco-churn/telco-churn.ipynb) | Telco Customer Churn | LightGBM, XGBoost, CatBoost, Optuna | Predicción de abandono de clientes con modelos de gradient boosting y ajuste de hiperparámetros |
| [trafico.ipynb](training/trafico/trafico.ipynb) | Imágenes de tráfico | YOLOv11 | Detección de infracciones de tráfico mediante visión por computador |

## Requisitos

Se recomienda usar un entorno virtual. Cada notebook incluye una celda `%pip install` con sus dependencias. Para el laboratorio de telco-churn:

```bash
pip install -r training/telco-churn/requirements.txt
```

Dependencias principales utilizadas en los laboratorios:

- `pandas`, `numpy` — manipulación de datos
- `matplotlib`, `seaborn`, `plotly` — visualización
- `scikit-learn` — modelos clásicos de ML
- `lightgbm`, `xgboost`, `catboost` — gradient boosting
- `optuna` — optimización de hiperparámetros
- `ultralytics` (YOLOv11) — visión por computador
