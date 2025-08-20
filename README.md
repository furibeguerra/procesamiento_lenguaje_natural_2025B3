# Procesamiento Lenguaje Natural 2025B3

Este es el repositorio para el planteamiento y desarrollo de los ejercicios propuestos en la asignatura de Procesamiento de Lenguaje Natural de la Universidad de Buenos Aires.
El repositorio de la clase se encuentra completamente disponible en el link adjunto: https://github.com/FIUBA-Posgrado-Inteligencia-Artificial/procesamiento_lenguaje_natural/tree/main 

## Desafio 1

1. Vectorizar documentos. Tomar 5 documentos al azar y medir similaridad con el resto de los documentos. Estudiar los 5 documentos más similares de cada uno analizar si tiene sentido la similaridad según el contenido del texto y la etiqueta de clasificación.

2. Entrenar modelos de clasificación Naïve Bayes para maximizar el desempeño de clasificación (f1-score macro) en el conjunto de datos de test. Considerar cambiar parámteros de instanciación del vectorizador y los modelos y probar modelos de Naïve Bayes Multinomial y ComplementNB.

3. Transponer la matriz documento-término. De esa manera se obtiene una matriz término-documento que puede ser interpretada como una colección de vectorización de palabras. Estudiar ahora similaridad entre palabras tomando 5 palabras y estudiando sus 5 más similares. La elección de palabras no debe ser al azar para evitar la aparición de términos poco interpretables, elegirlas "manualmente".

## Desafio 2

Se empleó Gensim para entrenar un modelo de vectores de palabras (word embeddings) utilizando un dataset asociado con Text Spam. El propósito fue generar y analizar las representaciones vectoriales de palabras para entender sus relaciones semánticas.

Desarrollo
Carga y Preprocesamiento de Datos: Se cargó un nuevo dataset y se prepararon los datos de texto. Esto incluyó la tokenización (dividir el texto en palabras individuales), la limpieza de puntuación y la eliminación de stopwords.

Entrenamiento del Modelo Gensim: Se entrenó un modelo de vectores de palabras (Word2Vec) utilizando el corpus preprocesado. Este proceso creó representaciones vectoriales para cada palabra, donde la distancia y dirección entre los vectores reflejan la similitud semántica y sintáctica de las palabras.

Análisis de Similitudes:

Se consultó el modelo para encontrar los términos más cercanos a una o varias palabras de interés (por ejemplo, buscar las palabras más similares a "Free").

Se analizó y se explicó por qué ciertas palabras resultaron ser similares en el espacio de embeddings, basándose en su contexto de aparición en el dataset.

Visualización de Embeddings:

Se utilizó una técnica de reducción de dimensionalidad como t-SNE o PCA para proyectar los vectores de alta dimensión en un espacio 2D.

Se graficaron los embeddings resultantes, lo que permitió visualizar grupos de palabras semánticamente relacionadas.

Conclusiones
El ejercicio demostró que el modelo entrenado con Gensim es capaz de capturar relaciones semánticas y sintácticas entre las palabras. La visualización de los embeddings confirmó que palabras con significados similares tienden a estar más cerca en el espacio vectorial. La capacidad del modelo para resolver analogías, aunque no perfecta, validó la lógica subyacente de las operaciones vectoriales para representar relaciones. 
