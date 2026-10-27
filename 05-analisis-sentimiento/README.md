# 05 · Análisis de sentimiento en reseñas de películas
*Sentiment analysis on movie reviews*

**Área:** procesamiento de lenguaje natural · **Herramientas:** Python, NLTK, spaCy, scikit-learn, Gensim (Word2Vec), Jupyter

## Problema
Clasificar reseñas de películas como **positivas** o **negativas**. El énfasis del proyecto estaba en el preprocesamiento del texto, que es la parte más exigente de un problema de NLP.

## Datos
Reseñas en inglés etiquetadas, con un conjunto de prueba de **25 000** reseñas.

## Mi enfoque
1. **Normalización:** eliminación de HTML, acentos, caracteres especiales y contracciones; conversión a minúsculas.
2. **Tokenización** y eliminación de palabras vacías (*stopwords*).
3. **Stemming** (Porter) y **lematización** (spaCy).
4. **Representación** del texto con TF-IDF y con *embeddings* Word2Vec.
5. **Clasificación** con regresión logística y comparación de variantes.

## Resultados
| Representación | Exactitud en prueba |
|---|---|
| TF-IDF + regresión logística | **88 %** |
| Word2Vec + regresión logística | 84 % |

## Qué aprendí
Cuánto influye cada paso del preprocesamiento en el resultado, y que una representación sencilla y bien preparada puede superar a una más sofisticada.
