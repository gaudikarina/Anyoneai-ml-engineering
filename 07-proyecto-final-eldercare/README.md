# 07 · Proyecto final: ElderCare, riesgo de hospitalización en adultos mayores
*Capstone: ElderCare, elderly hospitalization risk*

**Área:** aprendizaje automático aplicado a la salud · **Modalidad:** proyecto en equipo · **Herramientas:** Python, pandas, scikit-learn (SVM), FastAPI, React, Docker, docker-compose, AWS EC2

## Problema
Estimar la probabilidad de que una persona mexicana mayor de 50 años sea hospitalizada, a partir de factores demográficos, de salud y de estilo de vida. La herramienta busca apoyar a profesionales de la salud en la detección temprana y la asignación de recursos.

## Datos
Estudio Nacional de Salud y Envejecimiento en México (MHAS), encuesta pública y anonimizada. La versión de trabajo tenía unas **17 000 personas y más de 870 variables**, de modo que el principal reto fue la alta dimensionalidad. *No se publican datos.*

## Arquitectura
- **Preprocesamiento:** limpieza, selección de variables y reducción de dimensionalidad para quedarse con pocas variables relevantes.
- **Modelo:** máquina de vectores de soporte (SVM) con búsqueda de hiperparámetros (`GridSearchCV`: núcleo, `C` y `gamma`, con validación cruzada de 5 pliegues).
- **API** con FastAPI y base de datos.
- **Interfaz web** en React y TypeScript: formulario de evaluación en varios pasos, panel de visualización y reportes en PDF.
- **Despliegue** con contenedores Docker en un servidor AWS EC2.

## Mi contribución
- **Análisis exploratorio** de los datos de la encuesta: calidad de los datos, valores faltantes, distribución de la variable objetivo y relaciones entre variables.
- **Selección de variables con métodos de filtrado**, para reducir más de 870 variables a un subconjunto relevante con el cual entrenar el modelo.

## Qué aprendí
Trabajar en equipo sobre un problema real de salud con datos de muy alta dimensionalidad, y llevar el modelo hasta una aplicación desplegada y usable.
