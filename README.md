# Ejercicios de Procesamiento de Lenguaje Natural (NLP)

Este repositorio contiene una serie de ejercicios prácticos en el área de Procesamiento de Lenguaje Natural (NLP). A través de estos ejercicios, se exploran diferentes técnicas y modelos aplicados a datos textuales, incluyendo la vectorización de texto, modelos de clasificación, embeddings, LSTM y QA Bots. Cada ejercicio está diseñado para abordar un aspecto específico del NLP y mejorar la comprensión y habilidades en este campo.

## Ejercicio 1: Vectorización de texto y modelo de clasificación Naïve Bayes con el dataset 20 newsgroups

En este ejercicio se vectorizan documentos utilizando `TfidfVectorizer` y se entrena un modelo de clasificación Naïve Bayes para predecir las categorías de noticias.

### Pasos:

1. **Carga de datos**: Se cargan los datos del dataset 20 newsgroups.
2. **Vectorización**: Se vectorizan los documentos utilizando `TfidfVectorizer`.
3. **Medición de similaridad**: Se miden las similaridades de documentos utilizando la similitud coseno.
4. **Entrenamiento de modelos Naïve Bayes**: Se entrenan modelos de clasificación `MultinomialNB` y `ComplementNB`.
5. **Evaluación**: Se evalúa el desempeño de los modelos utilizando la métrica F1-score.

### Conclusiones:
Se logra vectorizar y clasificar los documentos de manera efectiva, obteniendo una buena precisión en la clasificación utilizando el modelo Naïve Bayes.

## Ejercicio 2: Construcción de un Bot basado en el ejemplo del traductor

### Pasos:

1. **Carga y preprocesamiento de datos**: Se utiliza un dataset de conversaciones en inglés.
2. **Entrenamiento del modelo**: Se construye y entrena un modelo LSTM para generar respuestas automáticas.
3. **Evaluación**: Se realizan preguntas al bot y se registran las respuestas para evaluar su desempeño.

### Conclusiones:
El bot de QA es capaz de generar respuestas coherentes a preguntas predefinidas, demostrando la viabilidad de utilizar modelos LSTM en aplicaciones de preguntas y respuestas.

## Ejercicio 3: Entrenamiento de embeddings con Gensim

Se entrena un modelo Word2Vec con un dataset de noticias falsas y se analizan las similitudes entre palabras en el espacio de embeddings.

### Pasos:

1. **Preprocesamiento de datos**: Se limpian y tokenizan los textos del dataset.
2. **Entrenamiento del modelo Word2Vec**: Se entrena un modelo Word2Vec con los textos preprocesados.
3. **Análisis de similitudes**: Se analizan las palabras similares en el espacio de embeddings.
4. **Visualización**: Se visualizan los embeddings utilizando PCA.

### Conclusiones:
El modelo Word2Vec permite capturar relaciones semánticas entre palabras, mostrando la eficacia de los embeddings en representar similitudes y diferencias entre términos.

## Ejercicio 4: Predicción de la próxima palabra con LSTM

Utilizando un dataset de tramas de películas, se entrena un modelo LSTM para la predicción de la próxima palabra en una secuencia.

### Pasos:

1. **Preprocesamiento de datos**: Se limpian y tokenizan las tramas de las películas.
2. **Creación de secuencias de entrenamiento**: Se crean secuencias de texto y se transforman en números.
3. **Entrenamiento del modelo LSTM**: Se entrena un modelo LSTM para predecir la próxima palabra.
4. **Evaluación y predicción**: Se evalúa el modelo y se realizan predicciones de nuevas secuencias.

### Conclusiones:
El modelo LSTM entrenado es capaz de predecir la próxima palabra en una secuencia con una precisión razonable, demostrando la capacidad de los LSTM para modelar secuencias de texto.

## Ejercicio 5: Clasificación de críticas de compradores de ropa utilizando Embeddings + LSTM

Se entrena un modelo para clasificar críticas de productos de ropa, utilizando embeddings preentrenados y entrenados desde cero.

### Pasos:

1. **Preprocesamiento de datos**: Se limpian y tokenizan las críticas de los compradores.
2. **Creación de embeddings**: Se crean embeddings entrenados desde cero y se utilizan embeddings preentrenados.
3. **Entrenamiento del modelo LSTM**: Se entrena un modelo LSTM con ambos tipos de embeddings.
4. **Evaluación**: Se evalúa el desempeño de ambos modelos.

### Conclusiones:
El uso de embeddings preentrenados mejora significativamente la precisión del modelo en la clasificación de críticas, destacando la importancia de los embeddings preentrenados en tareas de NLP.

## Ejercicio 6: Construcción de un Bot de QA basado en LSTM

Se construye un Bot de QA utilizando un modelo LSTM y un dataset de preguntas y respuestas.

### Pasos:

1. **Carga y preprocesamiento de datos**: Se limpia y tokeniza el dataset de preguntas y respuestas.
2. **Preparación de los embeddings**: Se utilizan embeddings de FastText para transformar los tokens de entrada.
3. **Construcción del modelo**: Se construye un modelo basado en el esquema encoder-decoder utilizando LSTM.
4. **Entrenamiento del modelo**: Se entrena el modelo con los datos generados.
5. **Inferencia y evaluación**: Se realizan preguntas al bot y se evalúa su desempeño.

### Conclusiones:
El bot de QA es capaz de generar respuestas coherentes a preguntas predefinidas, demostrando la viabilidad de utilizar modelos LSTM en aplicaciones de preguntas y respuestas.

### Conclusiones generales:

A través de estos ejercicios, se ha demostrado la eficacia de diferentes técnicas y modelos de NLP en tareas como clasificación de texto, predicción de palabras y respuestas automáticas. Cada modelo presenta sus propias ventajas y desafíos, y la selección de técnicas adecuadas depende del contexto y los objetivos específicos de la tarea.
