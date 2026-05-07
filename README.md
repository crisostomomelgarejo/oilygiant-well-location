# Proyecto: Selección de Ubicación para Nuevos Pozos Petrolíferos (OilyGiant)

## Descripción del Proyecto
Este proyecto fue desarrollado para la compañía de extracción de petróleo **OilyGiant**. El objetivo principal es encontrar los mejores lugares para abrir 200 pozos nuevos de petróleo, evaluando tres regiones geológicas distintas mediante técnicas de Machine Learning y análisis de riesgos.

## Objetivos
1. **Predecir el volumen de reservas:** Construcción de un modelo de Regresión Lineal para estimar el volumen de reservas en nuevos pozos basándose en datos geológicos.
2. **Calcular la ganancia potencial:** Selección de los 200 pozos con los valores estimados más altos en cada región para maximizar el margen de beneficio.
3. **Evaluación de riesgos:** Uso de la técnica de remuestreo estadístico (*Bootstrapping*) para analizar la distribución del beneficio esperado y evaluar el riesgo financiero asociado, garantizando un riesgo de pérdida inferior al 2.5%.

## Estructura del Proyecto
El proyecto está contenido en un entorno de Jupyter Notebook e incluye las siguientes etapas:
1. Carga y limpieza avanzada de datos.
2. Caracterización y Análisis Exploratorio de Datos (EDA).
3. Entrenamiento y validación del modelo de Regresión Lineal.
4. Cálculo de beneficios y evaluación de riesgos mediante Bootstrapping.
5. Conclusiones y recomendaciones de negocio.

## Tecnologías y Herramientas Utilizadas
* **Lenguaje:** Python 3
* **Análisis y manipulación de datos:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn (LinearRegression, train_test_split, mean_squared_error)
* **Estadística:** Bootstrapping para cálculo de intervalos de confianza y riesgos.

## Datos (Datasets)
Los datos geológicos explorados abarcan tres regiones distintas. Cada conjunto de datos tiene las siguientes características:
* `id` — Identificador único del pozo.
* `f0`, `f1`, `f2` — Tres características geológicas de los pozos.
* `product` — Volumen de reservas en el pozo petrolífero (en miles de barriles).

> **Nota:** Los archivos de datos correspondientes son `geo_data_0.csv`, `geo_data_1.csv` y `geo_data_2.csv`.

## Conclusiones
A través del análisis y el uso de Bootstrapping, se logró identificar la región geológica más rentable que cumple con el criterio de negocio de mantener un riesgo de pérdida menor al 2.5%, recomendando así el sitio óptimo para el desarrollo de los nuevos pozos.
