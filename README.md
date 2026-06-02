# 🧬 Detección de Cáncer de Mama mediante Machine Learning

**Materia:** Modelos 2
**Autores:** Alejandro Orrego Roldan, Luis David, Leonardo

🔗 **[Enlace al Video de Sustentación (10 Minutos) - Haz clic aquí] (PON_TU_LINK_AQUI)**

## 📌 Descripción del Proyecto
Este proyecto de Machine Learning tiene como objetivo desarrollar un modelo predictivo capaz de clasificar tumores mamarios (Malignos/Benignos) maximizando la métrica de **Recall** (Sensibilidad) para evitar Falsos Negativos clínicos. 

Se implementó un pipeline completo que abarca desde la exploración de datos, análisis de valores atípicos mediante *Isolation Forest*, hasta un **Estudio Comparativo (Benchmarking)** de algoritmos clásicos y redes neuronales frente a diferentes escenarios de Ingeniería de Características (Filtro Manual, LASSO y PCA).

---

## 📂 Arquitectura del Repositorio
El proyecto está diseñado de forma modular para garantizar su reproducibilidad y correcta evaluación.

```text
📁 tu_proyecto_cancer/
│
├── 📁 data/                        # Base de datos original y exportaciones de escenarios
│
├── 📓 01_Exploracion_y_Limpieza.ipynb  # EDA, correlación y análisis clínico de Atípicos (Isolation Forest)
├── 📓 02_Filtros_y_Reduccion.ipynb     # Creación de escenarios (Manual, LASSO, PCA)
├── 📓 03_Estudio_Comparativo.ipynb     # Entrenamiento GridSearchCV y Auditoría del modelo ganador
│
├── 📁 reporte/
│   └── reporte_final.pdf           # Artículo científico del proyecto en formato IEEE
│
└── 📄 README.md                    # Guía de ejecución del proyecto