# Clasificación de Diabetes con Support Vector Machine (SVM)

## Descripción del Proyecto
Este proyecto utiliza un conjunto de datos de pacientes con diabetes para entrenar y evaluar un modelo de clasificación. El objetivo es predecir si un paciente tiene diabetes basándose en ciertas características clínicas. Se ha seleccionado el algoritmo Support Vector Machine (SVM) para esta tarea debido a su capacidad para manejar problemas de clasificación binaria con márgenes máximos.

## Justificación del Algoritmo
Para este análisis, se ha seleccionado el algoritmo de Support Vector Machine (SVM) debido a su capacidad para manejar conjuntos de datos con clases balanceadas o desequilibradas de manera efectiva. Este algoritmo es conocido por su robustez y su habilidad para encontrar un hiperplano óptimo que maximiza el margen entre las diferentes clases, lo que lo hace particularmente adecuado para tareas de clasificación donde se requiere alta precisión.

## Descripción del Diseño del Modelo
El modelo se diseñó siguiendo estos pasos:

1. **Preprocesamiento:** Los datos fueron normalizados utilizando StandardScaler para asegurar que todas las características estuvieran en la misma escala.
2. **Selección de características:** Se mantuvieron todas las características disponibles debido a su relevancia para la predicción de la diabetes.
3. **Entrenamiento:** Se utilizó el algoritmo de Support Vector Machine (SVM) con un kernel RBF, ajustando los hiperparámetros clave utilizando GridSearchCV para encontrar los valores óptimos de `C` y `gamma`.

## Evaluación y Optimización del Modelo
El modelo fue evaluado utilizando la métrica de F1-score, que es especialmente útil en conjuntos de datos con clases desbalanceadas. Para optimizar el rendimiento, se aplicaron las siguientes técnicas:

- **Validación Cruzada:** Se realizó una validación cruzada de 10 pliegues para evitar el sobreajuste.
- **Ajuste de Hiperparámetros:** Los hiperparámetros fueron ajustados para maximizar el F1-score.

El modelo final logró una precisión del [valor]% en el conjunto de prueba.

## Instrucciones de Instalación
Para ejecutar este proyecto en tu máquina local, sigue estos pasos:

1. Clona el repositorio:
   ```bash
   git clone https://github.com/carlop13/analisis_DE__diabetes_indiana.git
