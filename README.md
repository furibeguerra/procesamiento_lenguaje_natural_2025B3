# Procesamiento Lenguaje Natural 2025B3



Este es el repositorio para el planteamiento y desarrollo de los ejercicios propuestos en la asignatura de Procesamiento de Lenguaje Natural de la Universidad de Buenos Aires.
El repositorio de la clase se encuentra completamente disponible en el link adjunto: https://github.com/FIUBA-Posgrado-Inteligencia-Artificial/procesamiento_lenguaje_natural/tree/main 

## Estructura del repositorio 

```desafio-1/: Vectorización, Similitud y Clasificación de Texto ```

```desafio-2/: Word Embeddings usando Word2Vec```

```desafio-3/: Modelo de Lenguaje con Tokenización por Caracteres```

```desafio-4/: Bot de Preguntas y Respuestas (QA) con Encoder/Decoder```

## Desafio 1 - Vectorización, Similitud y Clasificación de Texto ✨

El objetivo es Vectorizar documentos. Tomar 5 documentos al azar y medir similaridad con el resto de los documentos. Estudiar los 5 documentos más similares de cada uno analizar si tiene sentido la similaridad según el contenido del texto y la etiqueta de clasificación.

Para su desarrollo, se optimizó un modelo de clasificación Naïve Bayes probando las variantes Multinomial y ComplementNB, con el objetivo de maximizar el f1-score macro en un conjunto de prueba. Finalmente, se exploró la similitud entre palabras al transponer la matriz documento-término a una matriz término-documento, lo que permitió analizar las 5 palabras más similares a 5 términos seleccionados manualmente, validando así la proximidad contextual de las representaciones vectoriales.

## Desafio 2 - Word Embeddings usando Word2Vec 🔢 

El objetivo es emplear Gensim para entrenar un modelo de vectores de palabras (word embeddings) utilizando un dataset asociado con Text Spam. Se propuso generar y analizar las representaciones vectoriales de palabras para entender sus relaciones semánticas.

Se desarrolló un modelo de Word2Vec con la arquitectura Skip-gram para generar representaciones semánticas de palabras. El proceso incluyó el preprocesamiento del corpus de texto de Gutenberg y el entrenamiento del modelo para capturar relaciones contextuales. El resultado final fue la obtención de embeddings que permiten analizar las relaciones de significado entre palabras en un espacio vectorial, demostrando el concepto de semántica distribuida.

## Desafío 3 - Modelo de Lenguaje con Tokenización por Caracteres 💻

Para este desafio el objetivo principal es entrenar un modelo de lenguaje básico carácter por carácter.

Para su desarrollo, se entrenó una red neuronal LSTM para la generación de texto a nivel de carácter. El proceso incluyó la tokenización de un dataset de texto, la preparación de secuencias de entrada y salida, y el entrenamiento del modelo. La red, compuesta por una capa de Embedding y una capa LSTM, fue capaz de aprender la estructura y las dependencias del texto para predecir y generar nuevos caracteres de forma autónoma a partir de una secuencia inicial.


## Desafío 4 - Bot de Preguntas y Respuestas (QA) con Encoder/Decoder 🤖

El objecto es utilizar datos disponibles del challenge ConvAI2 (Conversational Intelligence Challenge 2) de conversaciones en inglés. Se construirá un BOT para responder a preguntas del usuario (QA).

Se creó un sistema de preguntas y respuestas empleando una arquitectura seq2seq (sequence-to-sequence). El proceso consistió en el preprocesamiento de pares de preguntas y respuestas, seguido de la implementación de un modelo Encoder-Decoder. Para optimizar el entrenamiento, se utilizó la técnica de teacher forcing. El resultado fue un sistema capaz de generar automáticamente respuestas coherentes a partir de preguntas, demostrando la capacidad del modelo para la compresión de contexto y la generación secuencial de texto.

## Estudiante:
:octocat: Fabian Andres Uribe Guerra

