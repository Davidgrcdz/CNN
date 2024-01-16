## Proyecto de Clasificación de Imágenes con Redes Neuronales Convolucionales (CNN)

Este proyecto se centra en la clasificación de imágenes utilizando dos arquitecturas de redes neuronales convolucionales (CNN): una implementada manualmente llamada CNNClassifier y otra basada en la arquitectura preentrenada MobileNetV2.

### Preprocesamiento de Datos

Se inicia cargando un conjunto de datos que contiene imágenes de caras reales y falsas. Estas imágenes se someten a diversas transformaciones, como redimensionamiento, volteo horizontal, rotación y normalización. Luego, se dividen en conjuntos de entrenamiento y prueba.

### Construcción del Modelo

La arquitectura de la red neuronal convolucional CNNClassifier se define en esta sección. La red consta de dos capas convolucionales seguidas de capas de normalización y max pooling, y dos capas completamente conectadas (fully connected). La función de activación utilizada es ReLU.

### Entrenamiento

La función de entrenamiento (`train_epoch`) se encarga de entrenar la red en el conjunto de entrenamiento utilizando la pérdida de entropía cruzada y el optimizador Adam. El proceso de entrenamiento se lleva a cabo durante 15 épocas, con un programa de reducción de tasa de aprendizaje (scheduler).

### Evaluación

Se evalúa el rendimiento del modelo en el conjunto de prueba calculando la precisión (accuracy).

### Visualización

Para facilitar la comprensión, se proporciona una función (`visualize_predictions`) que permite visualizar las predicciones del modelo en un subconjunto de imágenes del conjunto de prueba.

### Autores

- Gabriel Bernal Pinto
- David García Día
