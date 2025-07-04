# Análisis de Evasión de Clientes – Telecom X

Este repositorio contiene un análisis exploratorio de datos (EDA) aplicado al problema de evasión de clientes (churn) en Telecom X. El objetivo del proyecto es comprender los factores que influyen en la cancelación del servicio por parte de los clientes y proponer recomendaciones estratégicas basadas en datos.

## Objetivos del Proyecto

- Identificar patrones y correlaciones en los datos relacionados con la evasión.
- Analizar el impacto de variables como el tipo de contrato, servicios contratados y método de pago.
- Generar visualizaciones claras para la toma de decisiones.
- Preparar los datos para futuros modelos predictivos.

## Dataset

- Fuente: Archivo JSON con estructuras anidadas y doblemente anidadas.
- Contenido: Información demográfica, servicios utilizados, detalles de cuenta, facturación y estado de churn.
- Columnas destacadas: `customer`, `phone`, `internet`, `account`, `churn`, `monthly_charges`, `tenure`, etc.

## Limpieza y Transformación de Datos

- Normalización de nombres de columnas (minúsculas y uso de guion bajo).
- Desanidado de campos anidados (`customer`, `phone`, `internet`, `account`).
- Conversión de valores categóricos "yes"/"no" a formato binario (1/0).
- Conversión de columnas numéricas de tipo texto a tipo float (`total_charges`).
- Creación de nuevas variables derivadas como:
  - `n_servicios`: número de servicios adicionales contratados.
  - `cuentas_diarias`: estimación del gasto diario por cliente.

## Análisis Exploratorio (EDA)

- Distribución de churn mediante gráficos de torta y barras.
- Relación con variables categóricas como tipo de contrato, método de pago

![Correlation](https://github.com/user-attachments/assets/51353f9b-0c5a-440a-8c42-bedb70725e80)

![Grafico Torta](https://github.com/user-attachments/assets/8054dfe4-25fb-4bb3-81cc-1bbe2c57a1cd)



Instrucciones para ejecutar el notebook
Clona este repositorio:

git clone https://github.com/tu_usuario/telecom-churn-analysis.git
cd telecom-churn-analysis

Importa las librerías,
pip install pandas matplotlib seaborn numpy

Abre en un Collab
jupyter notebook Telecom_Churn_Analysis.ipynb

