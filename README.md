# Machine Learning Engineering · Anyone AI (2024)
*Machine Learning Engineering · Anyone AI (2024)*

Proyectos que desarrollé durante el programa de **Machine Learning Engineering de Anyone AI**: siete proyectos de punta a punta en ingeniería de datos, aprendizaje automático clásico, visión por computador, procesamiento de lenguaje natural, aplicaciones con modelos de lenguaje (LLM) y despliegue de servicios.

*Projects I built during Anyone AI's **Machine Learning Engineering** program: seven end-to-end projects covering data engineering, classical ML, computer vision, NLP, LLM-powered apps and service deployment.*

> **Nota sobre el código / Note on code.** Los enunciados, la estructura base y los datos pertenecen a Anyone AI, por lo que **este repositorio no contiene código ni datos**. Cada carpeta describe el problema, mi enfoque, las herramientas y los resultados que obtuve. Con gusto converso sobre los detalles técnicos.
> *Assignments, starter code and data belong to Anyone AI, so this repository contains **no code or data**. Each folder describes the problem, my approach, the tools and my results. Happy to discuss the technical details.*

| # | Proyecto | Área | Resultado principal | Herramientas |
|---|---|---|---|---|
| 01 | [Pipeline de datos de comercio electrónico](01-pipeline-datos-ecommerce/README.md) | Ingeniería de datos | Pipeline ELT y consultas de ingresos y entregas | Python, pandas, SQLite, SQL, API REST |
| 02 | [Riesgo crediticio](02-riesgo-crediticio/README.md) | Clasificación binaria | AUC-ROC de validación de 0,73 (Random Forest) | pandas, scikit-learn |
| 03 | [API de clasificación de imágenes](03-api-clasificacion-imagenes/README.md) | Despliegue de modelos | Servicio de microservicios con CNN preentrenada | FastAPI, Redis, TensorFlow, Streamlit, Docker, Locust |
| 04 | [Clasificación de vehículos](04-clasificacion-vehiculos/README.md) | Visión por computador | Exactitud de 80 % en prueba (25 clases) | TensorFlow, Keras, Colab GPU |
| 05 | [Análisis de sentimiento](05-analisis-sentimiento/README.md) | NLP | Exactitud de 88 % en 25 000 reseñas | NLTK, spaCy, scikit-learn, Word2Vec |
| 06 | [App con LLM para búsqueda de empleo](06-app-llm-busqueda-empleo/README.md) | LLM y RAG | Asistente que cruza un CV con ofertas y redacta la carta | LangChain, ChromaDB, OpenAI, Chainlit |
| 07 | [Proyecto final: ElderCare](07-proyecto-final-eldercare/README.md) | ML aplicado a salud (en equipo) | Predicción de riesgo de hospitalización desplegada en la nube | scikit-learn (SVM), FastAPI, React, Docker, AWS EC2 |

## Competencias que integré

- **Datos:** extracción desde CSV y API, carga en bases de datos, consultas SQL, análisis exploratorio y limpieza de datos con alta dimensionalidad.
- **Modelado:** codificación de variables, imputación, escalado, validación, búsqueda de hiperparámetros y selección de métricas (AUC-ROC, exactitud, precisión, exhaustividad, F1).
- **Aprendizaje profundo:** transferencia de aprendizaje y ajuste fino de redes convolucionales (ResNet50).
- **Lenguaje natural:** normalización, tokenización, *stemming*, lematización, TF-IDF y *embeddings*.
- **LLM:** ingeniería de *prompts*, recuperación aumentada (RAG), bases vectoriales, agentes y memoria conversacional.
- **Producción:** API con FastAPI, colas con Redis, contenedores con Docker, pruebas con pytest, pruebas de carga con Locust y despliegue en AWS.
