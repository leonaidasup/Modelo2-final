# Modelo2-final: Detección de Cáncer de Mama mediante Machine Learning

**Materia:** Modelos 2  
**Autores:** Alejandro Orrego Roldán, Luis David, Leonardo  

https://youtu.be/RX8XugLHQyA

## Descripción del Proyecto
Este proyecto de Machine Learning tiene como objetivo desarrollar un modelo predictivo capaz de clasificar tumores mamarios (Malignos/Benignos) maximizando la métrica de **Recall** (Sensibilidad) para evitar Falsos Negativos clínicos. 

Se implementó un pipeline de datos robusto que abarca la exploración, limpieza y un **Estudio Comparativo Analítico** de cinco arquitecturas algorítmicas (Regresión Logística, Random Forest, SVM, KNN y Redes Neuronales). 

Para determinar el subespacio dimensional más eficiente, los modelos fueron entrenados y evaluados sistemáticamente a través de **6 escenarios de Ingeniería de Características y Transformación Espacial**:

1. **Crudo (Línea Base):** 30 variables morfológicas originales estandarizadas.
2. **Selección LASSO (Método Incrustado):** Regularización L1 para combatir multicolinealidad y seleccionar variables lineales robustas.
3. **Mutual Information (Filtro No Lineal):** Captura de dependencias entrópicas y geométricas complejas.
4. **RFE (Método Wrapper):** Eliminación recursiva de características impulsada por modelado predictivo.
5. **PCA (Transformación No Supervisada):** Reducción ortogonal conservando el 95% de la varianza explicada.
6. **Discriminante de Fisher - LDA (Transformación Supervisada):** Proyección del espacio hiperdimensional a 1 único componente maximizando la separación de las clases.

---

## Arquitectura del Repositorio
El proyecto está diseñado de forma modular secuencial para garantizar su reproducibilidad técnica y correcta evaluación paso a paso.

```text
Modelo2-final/
│
├── data/                            # Base de datos original y exportaciones de los 6 escenarios
│
├── 01_Exploracion_y_Limpieza.ipynb  # EDA, correlación bivariada y análisis clínico de atípicos
├── 02_Filtros_y_Reduccion.ipynb     # Pipeline de los 6 escenarios, auditoría de variables y Scree Plot (PCA)
├── 03_Estudio_Comparativo.ipynb     # Entrenamiento, matrices de confusión y benchmarking gráfico final
│
├── reporte/
│   └── reporte_final.pdf               # Artículo científico del proyecto en formato IEEE
│
└── README.md                        # Documentación del proyecto
