# 03 · API de clasificación de imágenes
*Image classification API*

**Área:** despliegue de modelos · **Herramientas:** Python, FastAPI, Redis, TensorFlow, Streamlit, Docker, docker-compose, Locust, pytest

## Problema
Una empresa con una gran colección de imágenes necesitaba clasificarlas automáticamente en más de 1000 categorías. La solución debía incluir una interfaz web para subir imágenes y una API que sirviera una red convolucional (CNN) preentrenada.

## Arquitectura
- **Interfaz web** (Streamlit): inicio de sesión, carga de la imagen, predicción y envío de retroalimentación sobre el resultado.
- **API** (FastAPI): recibe la imagen, la valida y encola la tarea; devuelve la clase predicha en JSON y maneja los errores con mensajes claros.
- **Servicio del modelo:** consume la cola de Redis, preprocesa la imagen (redimensión y normalización) y ejecuta la CNN.
- **Base de datos** para usuarios y retroalimentación.

## Mi enfoque
1. Completé los Dockerfile multietapa (entorno de pruebas y de despliegue) de cada servicio.
2. Implementé los *endpoints* de la API y la comunicación entre microservicios mediante Redis.
3. Validé cada módulo con pruebas unitarias y el flujo completo con pruebas de integración.
4. Medí el comportamiento bajo carga con Locust.

## Qué aprendí
Pasar de un modelo en un cuaderno a un servicio: separar responsabilidades en microservicios, desacoplarlos con una cola y probar el sistema completo y no solo el modelo.
