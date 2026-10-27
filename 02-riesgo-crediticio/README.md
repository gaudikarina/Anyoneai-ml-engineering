# 02 · Riesgo crediticio (*Home Credit Default Risk*)
*Credit default risk*

**Área:** clasificación binaria · **Herramientas:** Python, pandas, scikit-learn, Matplotlib, Seaborn, Jupyter

## Problema
Predecir si una persona que solicita un crédito tendrá dificultades de pago (retraso en al menos una de las primeras cuotas). El modelo debía devolver probabilidades, y la métrica de evaluación fue el **área bajo la curva ROC (AUC-ROC)**.

## Datos
Archivos principales de solicitudes de crédito (entrenamiento y prueba), con variables demográficas, financieras y del historial del solicitante.

## Mi enfoque
1. Análisis exploratorio: distribución de la variable objetivo, valores faltantes y tipos de variables.
2. Preprocesamiento: codificación de variables categóricas (binaria y *one-hot*), imputación y escalado.
3. Modelo base con regresión logística.
4. Random Forest con ajuste de hiperparámetros, vigilando el sobreajuste (un modelo sin restricciones alcanzaba AUC de 1,0 en entrenamiento, pero no generalizaba).

## Resultados
| Modelo | AUC-ROC en validación |
|---|---|
| Regresión logística (base) | 0,68 |
| Random Forest ajustado | **0,73** |

## Qué aprendí
Leer la brecha entre entrenamiento y validación como señal de sobreajuste, y elegir una métrica que responda a la pregunta de negocio en lugar de la exactitud.
