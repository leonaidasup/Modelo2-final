# 🧬 Modelo2-final: Detección de Cáncer de Mama mediante Machine Learning

**Materia:** Modelos 2  
**Autores:** Alejandro Orrego Roldan, Luis David Martinez Estudiante, Leonardo Jose Amaris Dominguez Estudiante  

🔗 **[Enlace al Video de Sustentación (10 Minutos) - Haz clic aquí] (PON_TU_LINK_AQUI)**

## 📌 Descripción del Proyecto
Este proyecto de Machine Learning tiene como objetivo desarrollar un modelo predictivo capaz de clasificar tumores mamarios (Malignos/Benignos) maximizando la métrica de **Recall** (Sensibilidad) para evitar Falsos Negativos clínicos. 

Se implementó un pipeline de datos robusto que abarca la exploración y detección de valores atípicos mediante *Isolation Forest*, culminando en un **Estudio Comparativo Analítico** de cinco algoritmos (Regresión Logística, Random Forest, SVM, KNN y Redes Neuronales). 

Para determinar la arquitectura más eficiente, los modelos fueron entrenados y evaluados sistemáticamente a través de **6 escenarios de reducción de dimensionalidad e Ingeniería de Características**:
1. **Crudo (Línea Base):** 30 variables originales.
2. **Filtro Manual:** Reducción basada en correlación estadística lineal.
3. **Método Incrustado (LASSO):** Regularización L1 para selección intrínseca.
4. **Filtro No Lineal (Mutual Information):** Captura de dependencias entrópicas complejas.
5. **Método Wrapper (RFE):** Eliminación recursiva impulsada por modelado predictivo.
6. **Transformación Espacial (PCA):** Análisis de Componentes Principales.

---

## 📂 Arquitectura del Repositorio
El proyecto está diseñado de forma modular secuencial para garantizar su reproducibilidad técnica y correcta evaluación paso a paso.

```text
📁 Modelo2-final/
│
├── 📁 data/                            # Base de datos original y exportaciones de los 6 escenarios
│
├── 📓 01_Exploracion_y_Limpieza.ipynb  # EDA, correlación y análisis clínico de Atípicos (Isolation Forest)
├── 📓 02_Filtros_y_Reduccion.ipynb     # Pipeline de los 6 escenarios (Manual, LASSO, MI, RFE, PCA)
├── 📓 03_Estudio_Comparativo.ipynb     # Entrenamiento, matrices de confusión y Benchmarking gráfico
│
├── 📁 reporte/
│   └── reporte_final.pdf               # Artículo científico del proyecto en formato IEEE
│
└── 📄 README.md                        # Guía de ejecución del proyecto