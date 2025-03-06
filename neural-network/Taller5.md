# Taller 5
[Inicio](/README.md)
- [Clasificación de Gatos y Perros](/neural-network/Taller%205%20Clasificacion%20de%20Gatos%20y%20Perros.ipynb)
- [Red Neuronal con pesos aleatorios](/neural-network/Taller%205%20Red%20Neuronal%20con%20Pesos%20Aleatorios.ipynb)

Para la construccion de los codigos de Algoritmo Genetico se emplearon las siguientes librerias: 

1. TensorFlow (tensorflow)
Biblioteca de código abierto para machine learning y deep learning.
Proporciona herramientas para construir y entrenar redes neuronales.
Se usa para manejar datasets (tf.data.Dataset), construir modelos (tf.keras.models.Sequential), y optimizar el entrenamiento con tf.data.AUTOTUNE.

2. TensorFlow Datasets (tensorflow_datasets o tfds)
Proporciona acceso a conjuntos de datos listos para usar, como CIFAR-10 y Cats vs. Dogs.
Permite cargar datasets en estructuras tf.data.Dataset con tfds.load().

3. Matplotlib (matplotlib.pyplot o plt)
Biblioteca para la visualización de gráficos e imágenes.
Se emplea para mostrar imágenes de los datasets y las predicciones de la red neuronal.

4. OpenCV (cv2)
Biblioteca de procesamiento de imágenes y visión por computadora.
Se usa para redimensionar (cv2.resize()) y convertir imágenes a escala de grises (cv2.cvtColor()).

5. NumPy (numpy o np)
Biblioteca para la manipulación de arreglos y operaciones matemáticas eficientes.
Se emplea para normalizar imágenes y estructurar los datos de entrada/salida en la red neuronal.

6. Requests (requests)
Biblioteca para hacer solicitudes HTTP en Python.
Se utiliza para descargar imágenes de Internet con requests.get().

7. Keras Preprocessing (tensorflow.keras.preprocessing.image)
Submódulo de TensorFlow que facilita la carga y preprocesamiento de imágenes.
Se emplea image.load_img() y image.img_to_array() para transformar imágenes en datos utilizables en redes neuronales.

Tomando como referencia las siguientes paginas para comprender mejor las librerias y adaptarlas al codigo deseado: 

- TensorFlow. Tutorial de clasificación de imágenes con CNNs. TensorFlow. Recuperado de https://www.tensorflow.org/tutorials/images/cnn

- TensorFlow. Introducción a TensorFlow Datasets. TensorFlow. Recuperado de https://www.tensorflow.org/datasets/overview

- TensorFlow. Documentación sobre Data Augmentation en Keras. TensorFlow. Recuperado de https://www.tensorflow.org/api_docs/python/tf/keras/layers/RandomFlip

- TensorFlow. Clasificación de imágenes de gatos y perros con CNNs. TensorFlow. Recuperado de https://www.tensorflow.org/tutorials/images/classification

- PyImageSearch. Procesamiento de imágenes con OpenCV y TensorFlow. PyImageSearch. Recuperado de https://pyimagesearch.com/