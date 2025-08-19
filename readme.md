# 📊 Telecom X – Análisis de evasión de clientes (Churn)

Este proyecto forma parte de un desafío del programa **Alura ONE**, cuyo objetivo es identificar patrones de evasión de clientes para ayudar al equipo de Data Science de **Telecom X** a crear modelos predictivos y estrategias de retención.

---

## 🎯 Objetivo del proyecto
Aplicar un proceso **ETL** y un **Análisis Exploratorio de Datos (EDA)** para responder:
- ¿Qué características diferencian a los clientes que se quedan de los que se van?
- ¿Qué variables influyen más en la evasión?
- ¿Qué acciones podrían ayudar a reducir el churn?

---

## 📂 Estructura del repositorio
- `TelecomX_Data.json` → Datos originales en formato JSON.
- `TelecomX_diccionario.md` → Descripción de cada variable del dataset.
- `TelecomX_LATAM.ipynb` → Notebook principal con el proceso ETL, visualizaciones y análisis.
- `README.md` → Este documento.

---

## 🔄 Flujo de trabajo
1. **Extracción**  
   - Lectura de datos desde archivo JSON (simulación de extracción vía API).
   - Normalización de datos anidados con `pandas.json_normalize()`.

2. **Transformación**  
   - Limpieza de duplicados y valores nulos.
   - Conversión de tipos de datos.
   - Preparación de columnas clave (`tenure`, `MonthlyCharges`, `TotalCharges`).

3. **Carga**  
   - Uso de DataFrame limpio para análisis y visualizaciones.

4. **Análisis Exploratorio (EDA)**  
   - Gráficos de distribución y boxplots para comparar churn vs. variables clave.
   - Análisis por tipo de contrato, cargos mensuales y antigüedad.

---

## 📈 Principales insights
1. **Clientes con menor antigüedad (tenure)** presentan mayor churn.
2. **Cargos mensuales altos** están relacionados con más evasión.
3. Contratos **mes a mes** tienen tasas de churn mucho más elevadas.
4. Servicios adicionales como **TechSupport** y **DeviceProtection** parecen mejorar la retención.

---

## 🛠 Tecnologías usadas
- Python 3
- Pandas
- Matplotlib
- Seaborn

---

## ▶️ Cómo ejecutar el notebook
1. Abrir [Google Colab](https://colab.research.google.com/).
2. Subir el archivo `TelecomX_LATAM.ipynb`.
3. Subir también `TelecomX_Data.json` y `TelecomX_diccionario.md`.
4. Ejecutar las celdas en orden para reproducir el análisis.


---

## 👨‍💻 Autor
Desarrollado por *jimmy vasquez* como parte del desafío de análisis de datos en **Alura ONE**.
