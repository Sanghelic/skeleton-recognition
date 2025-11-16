Skeleton Action Recognition — Deep Learning

Este proyecto implementa un modelo de deep learning para clasificar acciones humanas utilizando el dataset UCF101 en su versión de esqueletos 2D (ucf101_2d.pkl). El enfoque se basa en procesar secuencias de keypoints y entrenar un modelo sencillo aplicando técnicas vistas en clase.

Contenido del repositorio

deeplearning.ipynb — Notebook principal con todo el pipeline:

Carga y exploración del dataset

Construcción del Dataset y DataLoader

Definición del modelo

Entrenamiento

Evaluación y resultados

Dataset requerido

El notebook utiliza el archivo:

ucf101_2d.pkl


Debido a su tamaño, no está incluido en GitHub.
Para descargar la versión de esqueletos de UCF101, consulta:

https://mmaction2.readthedocs.io/en/latest/dataset_zoo/skeleton.html

Una vez obtenido el archivo, colócalo en la ubicación que prefieras y edita la siguiente línea en el notebook:

SKELETON_PKL_PATH = "ruta/al/archivo.pkl"

Cómo ejecutar

Abrir el notebook en Google Colab.

Si el archivo se encuentra en Google Drive, montar Drive.

Editar la ruta del archivo en la primera celda.

Ejecutar todas las celdas en orden.

El modelo entrenará durante varias épocas y mostrará métricas de loss y accuracy para entrenamiento y validación.

Resultados

El modelo alcanza aproximadamente entre 0.55 y 0.60 de accuracy en validación usando 100 épocas.
Se aplicaron técnicas básicas de regularización y ajustes simples de hiperparámetros para mejorar el desempeño.
