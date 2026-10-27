# 06 · Aplicación con LLM para búsqueda de empleo
*LLM-powered job search app*

**Área:** modelos de lenguaje y recuperación aumentada (RAG) · **Herramientas:** Python, LangChain, OpenAI, ChromaDB, Chainlit, PyPDF2, pytest

## Problema
Crear una aplicación conversacional que lea el perfil de una persona (su CV en PDF), encuentre ofertas de empleo compatibles y redacte un mensaje personalizado para el reclutador.

## Arquitectura
- **Interfaz conversacional** con Chainlit.
- **ETL:** lectura del conjunto de ofertas, división en fragmentos (*chunking*) y generación de *embeddings* almacenados en ChromaDB.
- **Cadenas de LangChain:**
  - asistente conversacional general;
  - resumen del CV;
  - búsqueda de ofertas que combina la consulta del usuario con el resumen del CV (RAG);
  - agente con herramientas y memoria que redacta la carta de presentación.

## Mi enfoque
1. Extracción del texto del CV en PDF.
2. Diseño de las plantillas de *prompt* para cada cadena.
3. Construcción de la base vectorial y del recuperador.
4. Integración del agente con memoria conversacional.
5. Validación con pruebas unitarias del *backend*.

## Qué aprendí
Ingeniería de *prompts*, *chunking* y recuperación con *embeddings*, y cómo combinar cadenas, herramientas y memoria en un agente. Esta base se conecta con mi trabajo actual en evaluación de modelos de lenguaje y uso de herramientas por agentes.
