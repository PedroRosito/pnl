<img src="https://github.com/PedroRosito/pnl/blob/master/img/pnl.png">

# Procesamiento del Lenguaje Natural

Repositorio creado para la materia **Procesamiento natural del lenguaje** de la **Carrera de especialización en inteligencia artificial de la UBA**.

El repositorio contiene los 6 trabajos prácticos realizados durante el cursado de la materia que van introduciendo al procesamiento del lenguaje utilizando modelos de inteligencia artificial. Los mismos van aumentando en complejidad, comenzando por la vectorización de documentos y finalizando con la creación de un chatbot.

# Recomendaciones

Se recomienda utilizar un [entorno virtual de python](https://docs.python.org/3/library/venv.html) para correr los proyectos contenidos en este repositorio de forma local.

De lo contrario se puede utilizar [google colab](https://colab.research.google.com/?hl=es) de forma gratuita e ilimitada siempre y cuando no se requiera el uso de gpu.

# Contenido

## Ejercicio 1 - Vectorización de documentos

En este ejercicio de acercamiento se trabaja con la vectorización de palabras, utilizando la librería Numpy y librerías base de python.

- Se comienza con un corpus conformado por 3 oraciones o documentos.
- Se lo separa para obtener las palabras que conforman el corpus.
- Se utiliza OneHotEncoding para representar las palabras contenidas en cada documento.
- Se crea una matriz para ver la frecuencia de cada palabra en cada documento.
- Se genera una matriz con la representación TFIDF.
- Se realiza una comparación entre los documentos utilizando la similitud coseno.

## Ejercicio 2 - Bot

En este ejercicio se entrena un bot de preguntas y respuestas básico.

- Se utiliza un dataset generado a mano de preguntas y respuestas con las clases representativas de cada tema.
- Se le realiza un preprocesamiento al dataset.
- Se entrena una red neuronal sencilla con 3 capas densas combinadas con dropout.
- Se observa el desempeño del modelo.

## Ejercicio 3 - Custom Embeddings 

En este ejercicio se generan embeddings custom a partir del primer libro de Harry Potter en inglés.

- Se utiliza gensim para entrenar la capa de embeddings.
- Se visualizan los resultados probando las relaciones obtenidas entre algunas palabras presentes en el documento de entrada.

## Ejercicio 4 - Predicción de próxima palabra

En este ejercicio se busca realizar un modelo capaz de predecir la siguiente palabra que aparecerá dada una entrada.

- Se utiliza como corpus el primer libro de Harry Potter para crear embeddings de palabras basado en ese contexto utilizando la layer Embedding de Keras.
- Se utilizan los embeddings generados junto con capas LSTM para predecir la próxima posible palabra.
- Se genera secuencias nuevas a partir de una entrada de texto.

## Ejercicio 5 - Predicción de críticas

En este ejercicio se utiliza como dataset un archivo que contiene críticas de compradores de ropa y se busca predecir la evaluación del comprador
y su crítica para un determinado producto.

- Se realiza una limpieza de los datos.
- Se realiza un balanceo del dataset utilizando SMOTETomek.
- Se entrena un modelo con embeddings custom + LSTM.
- Se entrena un modelo con embeddings fasttext + LSTM.
- Se evalúan los modelos obtenidos.

## Ejercicio 6 - ChatBot

En este ejercicio se crea un chatbot utilizando el dataset ConvAI2 (Conversational Intelligence Challenge 2) de conversaciones en inglés.

- Se realiza una tokenización de las palabras de entrada.
- Se utilizan los embeddings de fasttext para transformar los tokens de entrada en vectores.
- Se entrena el modelo utilizando LSTM + capas densas y dropout.
- Se prueba el chatbot observando como responde a ciertas entradas de texto simples.
