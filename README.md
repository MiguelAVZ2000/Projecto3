# Clasificación de Sentimientos con Reseñas de Amazon

Este proyecto utiliza técnicas de ciencia de datos y aprendizaje automático para clasificar el sentimiento de las reseñas de productos de Amazon (positivo o negativo) utilizando el conjunto de datos "Amazon Fine Food Reviews".

## Descripción

El objetivo principal de este proyecto es construir un modelo de clasificación de sentimientos que pueda predecir con precisión el sentimiento de una reseña de producto basándose en su texto. El proyecto sigue un flujo de trabajo típico de ciencia de datos, que incluye:

* Carga y exploración de datos.
* Preprocesamiento de texto (limpieza, tokenización, etc.).
* Vectorización de texto (TF-IDF).
* Entrenamiento de un modelo de aprendizaje automático (Regresión Logística).
* Evaluación del rendimiento del modelo.

## Conjunto de Datos

El conjunto de datos utilizado en este proyecto es "Amazon Fine Food Reviews", que se puede descargar de [aquí (coloca el enlace de donde lo descargaste)].

## Dependencias

Para ejecutar este proyecto, necesitarás las siguientes librerías de Python:

* pandas
* scikit-learn
* nltk
* swifter
* dask (opcional, si se usa para procesamiento distribuido)
* joblib o pickle

Puedes instalar estas dependencias usando el archivo `requirements.txt` incluido en este repositorio:

```bash
pip install -r requirements.txt
```
Instrucciones de Uso
Clona este repositorio:

```bash

git clone https://github.com/MiguelAVZ2000/Projecto3.git
```
Navega al directorio del proyecto:

```bash

cd [nombre del directorio]
```
```bash

python -m venv venv
source venv/bin/activate  # En Linux/macOS
venv\Scripts\activate  # En Windows
```
Instala las dependencias:

```bash

pip install -r requirements.txt
```
Ejecuta el notebook de Jupyter clasificacion_sentimientos.ipynb para seguir el flujo de trabajo del proyecto.

Los modelos entrenados (modelo y vectorizador) se guardan como archivos .joblib o .pkl para su posterior uso.

Estructura del Proyecto
├── data/
│   └── Reviews.csv       # Conjunto de datos original
├── notebooks/
│   └── clasificacion_sentimientos.ipynb # Notebook de Jupyter con el código del proyecto
├── models/
│   └── modelo_sentimientos.joblib # Modelo entrenado
│   └── vectorizador.joblib     # Vectorizador TF-IDF entrenado
├── requirements.txt      # Lista de dependencias
└── README.md             # Este archivo
Resultados
El modelo de Regresión Logística alcanzó una precisión de [precisión obtenida] en el conjunto de prueba. Puedes encontrar más detalles sobre el rendimiento del modelo en el notebook de Jupyter.

Posibles Mejoras
Explorar otros modelos de aprendizaje automático (Naive Bayes, SVM, etc.).
Realizar un ajuste de hiperparámetros más exhaustivo.
Utilizar técnicas de procesamiento de lenguaje natural más avanzadas (word embeddings, transformers).
Implementar una interfaz de usuario para permitir a los usuarios ingresar sus propias reseñas y obtener predicciones de sentimiento.