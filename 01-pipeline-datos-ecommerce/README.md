# 01 · Pipeline de datos de comercio electrónico
*E-commerce data pipeline*

**Área:** ingeniería de datos · **Herramientas:** Python, pandas, SQLite, SQL, API REST, Matplotlib, Seaborn, pytest

## Problema
Una de las mayores plataformas de comercio electrónico de Latinoamérica necesitaba comprender su desempeño entre 2016 y 2018 en dos dimensiones: **ingresos** (por año, por categoría de producto y por estado) y **entregas** (tiempos reales frente a los estimados, y su variación según el mes y los feriados).

## Datos
- Conjunto público y anonimizado de Olist (Brasil): unas 100 000 órdenes con información de pagos, fletes, productos, clientes y reseñas.
- API pública de feriados (`date.nager.at`) para cruzar las fechas de entrega con los feriados de Brasil.

## Mi enfoque
1. **Extracción** de los archivos CSV y de la API de feriados.
2. **Carga** en una base de datos SQLite (enfoque ELT).
3. **Transformación** con consultas SQL: ingresos anuales y por estado, categorías más y menos vendidas, tiempos de entrega reales frente a los estimados.
4. **Visualización** de los resultados para el análisis de negocio.
5. Validación con las pruebas unitarias del proyecto.

## Qué aprendí
Diseñar un flujo de datos reproducible que pueda ejecutarse cada mes o cada año, y separar con claridad las etapas de extracción, carga y transformación.
