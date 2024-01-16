Este proyecto está enfocado en la clasificación de imágenes utilizando dos arquitecturas de redes neuronales convolucionales (CNN): una implementada manualmente llamada CNNClassifier y otra basada en la arquitectura preentrenada MobileNetV2.

Preprocesamiento de Datos:

Se carga un conjunto de datos que contiene imágenes de caras reales y falsas. Estas imágenes se transforman mediante técnicas como redimensionamiento, volteo horizontal, rotación y normalización, y se dividen en conjuntos de entrenamiento y prueba.


Construcción del Modelo:

Se define la arquitectura de la red neuronal convolucional CNNClassifier. Esta red consta de dos capas convolucionales seguidas de capas de normalización y max pooling, y dos capas completamente conectadas (fully connected). La función de activación utilizada es ReLU.


Entrenamiento:

Se implementa una función de entrenamiento (train_epoch) que realiza el entrenamiento de la red en el conjunto de entrenamiento utilizando la pérdida de entropía cruzada y el optimizador Adam. El entrenamiento se realiza durante 15 épocas, con un programa de reducción de tasa de aprendizaje (scheduler).


Evaluación:

Se evalúa el rendimiento del modelo en el conjunto de prueba calculando la precisión (accuracy).


Visualización:

Se proporciona una función (visualize_predictions) para visualizar las predicciones del modelo en un subconjunto de imágenes del conjunto de prueba.



Autores: Gabriel Bernal Pinto y David García Díaz
