# 04 · Clasificación de vehículos a partir de imágenes
*Vehicle classification from images*

**Área:** visión por computador · **Herramientas:** Python, TensorFlow, Keras, Matplotlib, Google Colab (GPU), Docker

## Problema
Una empresa de autos usados quería que sus clientes buscaran vehículos por marca y modelo sin cargar esos datos a mano. La prueba de concepto consistía en clasificar fotografías de **25 marcas y modelos** con una exactitud superior al **80 %** en el conjunto de prueba.

## Datos
Imágenes JPG etiquetadas por carpeta (marca y modelo), divididas en entrenamiento y prueba.

## Mi enfoque
1. Implementé el modelo en Keras sobre **ResNet50** preentrenada (transferencia de aprendizaje).
2. Agregué capas de *dropout* para reducir el sobreajuste.
3. Ajusté la tasa de aprendizaje y, en una segunda fase, hice ajuste fino de capas de la red base.
4. Entrené con GPU en Google Colab y comparé varias configuraciones.

## Resultados
Las primeras configuraciones alcanzaban alrededor de 30 % de exactitud. Tras el ajuste fino, el modelo final llegó a **80 % de exactitud en prueba** (1875 imágenes; F1 promedio de 0,80), con lo que cumplió el objetivo.

## Qué aprendí
Iterar con método: diagnosticar por qué un modelo no aprende, y cuándo conviene descongelar capas de una red preentrenada.
