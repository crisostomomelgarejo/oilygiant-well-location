# OilyGiant Well Location / Selección de Ubicación de Pozos (OilyGiant)

[🇺🇸 English](#english) | [🇪🇸 Español](#espanol)

---

<a name="english"></a>
## 🇺🇸 English

### Project Description
This project was developed for the oil extraction company **OilyGiant**. The main objective is to find the best places to open 200 new oil wells, evaluating three different geological regions using Machine Learning techniques and risk analysis.

### Objectives
1. **Predict reserve volume:** Construction of a Linear Regression model to estimate the reserve volume in new wells based on geological data.
2. **Calculate potential profit:** Selection of the 200 wells with the highest estimated values in each region to maximize the profit margin.
3. **Risk evaluation:** Use of the statistical resampling technique (*Bootstrapping*) to analyze the distribution of expected profit and evaluate the associated financial risk, guaranteeing a loss risk of less than 2.5%.

### Project Structure
The project is contained in a Jupyter Notebook environment and includes the following stages:
1. Advanced data loading and cleaning.
2. Characterization and Exploratory Data Analysis (EDA).
3. Training and validation of the Linear Regression model.
4. Profit calculation and risk evaluation using Bootstrapping.
5. Conclusions and business recommendations.
*Note: This repository contains two versions of the notebook (`notebooks/OilyGiant_EN.ipynb` and `notebooks/OilyGiant_ES.ipynb`) for your convenience.*

### Technologies and Tools Used
* **Language:** Python 3
* **Data analysis and manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn (LinearRegression, train_test_split, mean_squared_error)
* **Statistics:** Bootstrapping for calculation of confidence intervals and risks.

### Data (Datasets)
The geological data explored covers three different regions. Each dataset has the following characteristics:
* `id` — Unique identifier of the well.
* `f0`, `f1`, `f2` — Three geological characteristics of the wells.
* `product` — Volume of reserves in the oil well (in thousands of barrels).

> **Note:** The corresponding data files are located in the `datasets/` folder (`geo_data_0.csv`, `geo_data_1.csv`, and `geo_data_2.csv`).

### Conclusions
Through analysis and the use of Bootstrapping, it was possible to identify the most profitable geological region that meets the business criterion of maintaining a loss risk of less than 2.5%, thus recommending the optimal site for the development of new wells.

---

<a name="espanol"></a>
## 🇪🇸 Español

### Descripción del Proyecto
Este proyecto fue desarrollado para la compañía de extracción de petróleo **OilyGiant**. El objetivo principal es encontrar los mejores lugares para abrir 200 pozos nuevos de petróleo, evaluando tres regiones geológicas distintas mediante técnicas de Machine Learning y análisis de riesgos.

### Objetivos
1. **Predecir el volumen de reservas:** Construcción de un modelo de Regresión Lineal para estimar el volumen de reservas en nuevos pozos basándose en datos geológicos.
2. **Calcular la ganancia potencial:** Selección de los 200 pozos con los valores estimados más altos en cada región para maximizar el margen de beneficio.
3. **Evaluación de riesgos:** Uso de la técnica de remuestreo estadístico (*Bootstrapping*) para analizar la distribución del beneficio esperado y evaluar el riesgo financiero asociado, garantizando un riesgo de pérdida inferior al 2.5%.

### Estructura del Proyecto
El proyecto está contenido en un entorno de Jupyter Notebook e incluye las siguientes etapas:
1. Carga y limpieza avanzada de datos.
2. Caracterización y Análisis Exploratorio de Datos (EDA).
3. Entrenamiento y validación del modelo de Regresión Lineal.
4. Cálculo de beneficios y evaluación de riesgos mediante Bootstrapping.
5. Conclusiones y recomendaciones de negocio.
*Nota: Este repositorio contiene dos versiones del notebook (`notebooks/OilyGiant_EN.ipynb` y `notebooks/OilyGiant_ES.ipynb`) para tu comodidad.*

### Tecnologías y Herramientas Utilizadas
* **Lenguaje:** Python 3
* **Análisis y manipulación de datos:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn (LinearRegression, train_test_split, mean_squared_error)
* **Estadística:** Bootstrapping para cálculo de intervalos de confianza y riesgos.

### Datos (Datasets)
Los datos geológicos explorados abarcan tres regiones distintas. Cada conjunto de datos tiene las siguientes características:
* `id` — Identificador único del pozo.
* `f0`, `f1`, `f2` — Tres características geológicas de los pozos.
* `product` — Volumen de reservas en el pozo petrolífero (en miles de barriles).

> **Nota:** Los archivos de datos correspondientes están en la carpeta `datasets/` (`geo_data_0.csv`, `geo_data_1.csv` y `geo_data_2.csv`).

### Conclusiones
A través del análisis y el uso de Bootstrapping, se logró identificar la región geológica más rentable que cumple con el criterio de negocio de mantener un riesgo de pérdida menor al 2.5%, recomendando así el sitio óptimo para el desarrollo de los nuevos pozos.
