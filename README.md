# 🧬 Modelo2-final: Detección de Cáncer de Mama mediante Machine Learning

**Materia:** Modelos 2
**Autores:** Alejandro Orrego Roldan, Luis David, Leonardo

🔗 **[Enlace al Video de Sustentación (10 Minutos) - Haz clic aquí] (PON_TU_LINK_AQUI)**

## 📌 Descripción del Proyecto
Este proyecto de Machine Learning tiene como objetivo desarrollar un modelo predictivo capaz de clasificar tumores mamarios (Malignos/Benignos) maximizando la métrica de **Recall** (Sensibilidad) para evitar Falsos Negativos clínicos. 

Se implementó un pipeline completo que abarca desde la exploración de datos y el análisis de valores atípicos mediante *Isolation Forest*, hasta un **Estudio Comparativo Analítico** de cinco algoritmos (Regresión Logística, Random Forest, SVM, KNN y Redes Neuronales) frente a diferentes escenarios de Ingeniería de Características (Filtro Manual, LASSO y PCA).

---

## 📂 Arquitectura del Repositorio
El proyecto está diseñado de forma modular para garantizar su reproducibilidad y correcta evaluación paso a paso.

```text
📁 Modelo2-final/
│
├── 📁 data/                        # Base de datos original y exportaciones de escenarios
│
├── 📓 01_Exploracion_y_Limpieza.ipynb  # EDA, correlación y análisis clínico de Atípicos (Isolation Forest)
├── 📓 02_Filtros_y_Reduccion.ipynb     # Creación de escenarios (Filtro Manual, LASSO, PCA)
├── 📓 03_Estudio_Comparativo.ipynb     # Evaluación detallada con Matrices de Confusión y Benchmarking final
│
├── 📁 reporte/
│   └── reporte_final.pdf           # Artículo científico del proyecto en formato IEEE
│
└── 📄 README.md                    # Guía de ejecución del proyecto