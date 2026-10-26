
# Práctica 1: Aprendizaje No Supervisado (DengAI)

Este repositorio contiene el desarrollo y análisis de técnicas de **Aprendizaje No Supervisado** aplicado al problema de predicción y agrupación de casos de Dengue (**DengAI: Predicting Disease Spread**).

## 👤 Autor

* **Nombre:** Maicol Patiño Sierra

---

## 📌 Descripción del Proyecto

El objetivo principal es aplicar y comparar técnicas de aprendizaje no supervisado sobre datos climáticos y epidemiológicos para identificar patrones de transmisión del dengue en las ciudades de San Juan y Iquitos.

### Objetivos Clave:
1. **Exploración y Preprocesamiento de Datos:** Manejo de valores nulos, escalamiento de variables y análisis exploratorio de datos (EDA).
2. **Reducción de Dimensionalidad:** Aplicación de algoritmos como PCA (Análisis de Componentes Principales) para reducir la complejidad de las características climáticas.
3. **Agrupamiento (Clustering):** Identificación de estructuras ocultas y clusters mediante algoritmos como $K$-Means, Clustering Jerárquico o DBSCAN.
4. **Interpretación de Resultados:** Análisis epidemiológico y evaluación del impacto de las variables ambientales en la propagación del virus.

Algoritmo Jerárquico
<img width="1772" height="911" alt="image" src="https://github.com/user-attachments/assets/23a4b16a-c1fe-4eae-ad9e-36e6a4f0b022" />

Algoritmo Particionante K-Means
<img width="1384" height="563" alt="image" src="https://github.com/user-attachments/assets/745f3acd-6bf3-4011-a1a1-ee78f398b636" />

Algoritmo de densidad DB Scan
<img width="1784" height="563" alt="image" src="https://github.com/user-attachments/assets/ebc5a50e-b92c-44a0-a658-ad840c9506d2" />

Clustering probabilístico Gaussianas (GMM - Gaussian Mixture Models)
<img width="1784" height="563" alt="image" src="https://github.com/user-attachments/assets/26988c21-dfb2-4da0-a74f-71e806fdc87d" />

Algoritmo	N° Clusters	% Ruido	Silueta	Davies-Bouldin
0	Jerárquico (Ward, k=3)	3	0.0%	0.2910	1.2299
1	K-Means++ (k=3)	3	0.0%	0.3085	1.1873
2	DBSCAN (eps=2.8)	2	7.1%	0.3305	1.2845
3	GMM Full (k=3)	3	0.0%	0.2970	1.2322

---

## 📁 Estructura del Repositorio

```text
.
├── 07MBIDPractica1_MaicolPatino.ipynb   # Notebook principal con todo el desarrollo y análisis
├── dengue_features_train.csv           # (Opcional) Conjunto de datos climáticos
└── README.md                           # Documentación del proyecto
```

---

## 🛠️ Requisitos e Instalación

Para ejecutar y reproducir el análisis en tu entorno local, asegúrate de tener instalado Python (3.8 o superior) y las siguientes librerías principales:

### Librerías empleadas:
* `numpy`
* `pandas`
* `matplotlib`
* `seaborn`
* `scikit-learn`

### Pasos para ejecutar:
1. Clona este repositorio en tu máquina local:
   ```bash
   git clone https://github.com/TU_USUARIO/TU_REPOSITORIO.git
   ```
2. Navega al directorio del proyecto:
   ```bash
   cd TU_REPOSITORIO
   ```
3. Abre el archivo `.ipynb` en Visual Studio Code o Jupyter Notebook:
   ```bash
   jupyter notebook 07MBIDPractica1_MaicolPatino.ipynb
   ```
4. Ejecuta las celdas en orden secuencial.

---

## 📊 Resumen de Metodología y Técnicas

1. **Preprocesamiento:** Imputación de datos faltantes, normalización/estandarización de características temporales y meteorológicas.
2. **Reducción de Dimensionalidad:**
   * Evaluación de la varianza explicada acumulada.
   * Proyección de datos en componentes principales.
3. **Modelos de Agrupamiento:**
   * Determinación del número óptimo de clusters (Método del Codo / Coeficiente de Silueta).
   * Segmentación de períodos de alto y bajo riesgo epidemiológico.

---

## 📜 Licencia y Uso Academic
Este trabajo ha sido desarrollado exclusivamente con fines académicos para el máster/programa en la **Universidad Internacional de Valencia (VIU)**.
