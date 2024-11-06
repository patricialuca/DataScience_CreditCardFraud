# Proyecto de Detección de Fraudes con Tarjetas de Crédito

Este proyecto es el trabajo final de la Certificación del Programa de Inteligencia Artificial de IBM. El objetivo es aplicar técnicas de aprendizaje automático para la detección de fraudes en transacciones de tarjetas de crédito. A lo largo del proyecto, se sigue un flujo de análisis y desarrollo orientado a la clasificación de transacciones como fraudulentas (clase 1) o no fraudulentas (clase 0).
## Dataset
- **Fuente**: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Descripción**: El dataset contiene un conjunto de transacciones con un marcado desbalance entre transacciones fraudulentas (0.16%) y no fraudulentas.

## Pasos del Proyecto

### 1. **Carga y Limpieza de Datos**
   - Se importaron las bibliotecas necesarias, y el dataset fue cargado en un `DataFrame`.
   - Se eliminaron filas duplicadas, y se verificó que no hubiera valores nulos.

### 2. **Análisis Exploratorio de Datos (EDA)**
   - **Distribución de Fraudes**: Se visualizó la proporción de transacciones fraudulentas y no fraudulentas.
   - **Distribución del Monto en Transacciones Fraudulentas**: Se exploró mediante un histograma, destacando los patrones de gasto en transacciones sospechosas.

### 3. **Desarrollo de Modelos**
   - Los datos se dividieron en conjuntos de entrenamiento y prueba (80%-20%).
   - Se entrenó un modelo de clasificación usando **Random Forest** con hiperparámetros ajustados para mejorar el rendimiento en datos desbalanceados.
   
### 4. **Evaluación del Modelo**
   - **Métricas de Rendimiento**: Las principales métricas evaluadas fueron:
      - **Precisión** para medir la proporción de transacciones predichas correctamente.
      - **Recall** para evaluar la capacidad del modelo de detectar fraudes (minimizar falsos negativos).
      - **F1-Score** como métrica de balance entre precisión y recall.
   - **Matriz de Confusión**: La matriz de confusión mostró excelentes resultados en la clasificación de transacciones no fraudulentas, y resultados buenos en las fraudulentas, con una precisión general del modelo de 99.95%.

## Conclusiones
El modelo Random Forest demostró ser altamente eficaz para detectar transacciones fraudulentas, aunque se sugiere trabajar en técnicas de mejora para minimizar los falsos negativos en la detección de fraudes.

## Requisitos
Para reproducir el análisis y el modelo:
- Python 3.x
- Bibliotecas: `pandas`, `numpy`, `seaborn`, `matplotlib`, `scikit-learn`

## Ejecución
1. Clona este repositorio.
2. Ejecuta el notebook paso a paso para entrenar y evaluar el modelo en el dataset de detección de fraude.

## Autoría
Este proyecto fue realizado por [Patricia Luengo Carretero](https://www.linkedin.com/in/patricialuca/) y también lo puedes encontrar en kaggle en [Proyecto Final -Programa de IA de IBM](https://www.kaggle.com/code/patrilc/proyecto-final-programa-de-ia-de-ibm) Puedes ver más sobre mi trabajo en mi [sitio web personal](https://www.patricialuca.es).
