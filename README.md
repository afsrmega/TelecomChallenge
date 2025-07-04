# TelecomChallenge
Challenge Telecom

Análisis de Evasión de Clientes – Telecom X
Este repositorio contiene un análisis exploratorio de datos (EDA) aplicado al problema de evasión de clientes (churn) en Telecom X. El objetivo del proyecto es comprender los factores que influyen en la cancelación del servicio por parte de los clientes y proponer recomendaciones estratégicas basadas en datos.

Objetivos del Proyecto
Identificar patrones y correlaciones en los datos relacionados con la evasión.

Analizar el impacto de variables como el tipo de contrato, servicios contratados y método de pago.

Generar visualizaciones claras para la toma de decisiones.

Preparar los datos para futuros modelos predictivos.

Dataset
Fuente: Archivo JSON con estructuras anidadas y doblemente anidadas.

Contenido: Información demográfica, servicios utilizados, detalles de cuenta, facturación y estado de churn.

Columnas destacadas: customer, phone, internet, account, churn, monthly_charges, tenure, etc.

Limpieza y Transformación de Datos
Normalización de nombres de columnas (minúsculas y uso de _).

Desanidado de campos anidados (customer, phone, internet, account).

Conversión de valores categóricos yes/no a formato binario (1/0).

Conversión de columnas numéricas de tipo texto a tipo float (total_charges).

Creación de nuevas variables derivadas como:

n_servicios: número de servicios adicionales contratados.

cuentas_diarias: estimación del gasto diario por cliente.

Análisis Exploratorio (EDA)
Distribución de churn: gráficos de torta y barras.

Relación con variables categóricas: tipo de contrato, método de pago, género, ciudadanía senior, etc.

Distribución de variables numéricas: análisis de tenure, monthly_charges, total_charges por estado de churn.

Correlación: matriz de correlación y gráfico de barras destacando los predictores más relevantes.

Crosstab avanzado: combinación de variables como contract × payment_method para identificar combinaciones de alto riesgo.

Hallazgos Clave
Los clientes con contrato mes a mes presentan mayor tasa de churn.

La falta de servicios como seguridad online, soporte técnico y respaldo se asocia fuertemente con evasión.

Los cargos mensuales más altos tienen una correlación positiva moderada con churn.

El método de pago mediante electronic check tiene la mayor tasa de cancelación.

Los contratos de dos años con pago por cheque físico tienen la menor tasa de evasión.

Análisis Adicional (Opcional)
Exploración del número de servicios contratados y su relación con churn.

Análisis cruzado de variables categóricas que identifican perfiles de riesgo.

Preparación para modelado predictivo con regresión logística o árboles de decisión.

📎 Requisitos
bash
Copiar
Editar
pandas
matplotlib
seaborn
numpy
Instalar con:

bash
Copiar
Editar
pip install pandas matplotlib seaborn numpy
Estructura del Proyecto
bash
Copiar
Editar
├── TelecomX_Data.json             # Archivo original
├── Telecom_Churn_Analysis.ipynb   # Cuaderno principal
├── README.md                      # Descripción del proyecto
🔜 Próximos Pasos
Crear modelos de clasificación para predecir churn.

Implementar dashboard interactivo con Streamlit o Dash.

Integrar datos externos del mercado para análisis más completo.

Autor
Andrés Sereno
LinkedIn · GitHub
