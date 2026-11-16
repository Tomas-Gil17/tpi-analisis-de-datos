# Análisis de cancelación de clientes — Telco Customer Churn

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Tomas-Gil17/tpi-analisis-de-datos/blob/main/notebooks/TPI_Analisis_de_Datos.ipynb)

Trabajo Práctico Integrador de Introducción al Análisis de Datos — División 343.

## Problema de negocio

Una empresa de telecomunicaciones pierde clientes todos los meses (churn). Este proyecto analiza el historial de 7.043 clientes para identificar qué características se asocian a la cancelación del servicio y proponer acciones de retención. Además, se entrena un modelo de regresión lineal para estimar la facturación acumulada de cada cliente (TotalCharges).

Principales hallazgos:
- La tasa de cancelación general es del 26,5%.
- Los clientes con contrato mes a mes cancelan un 42,7%, contra 2,8% del contrato a dos años.
- El riesgo se concentra en el primer año de antigüedad y en quienes pagan con cheque electrónico.
- El modelo de regresión múltiple explica el 90% de la variación de la facturación acumulada (R² = 0,90).

## Integrantes
- Ibarra, Gimena Abril - @GimenaIbarra
- Rodríguez, Lucas - @Lucas1Rodriguez
- Gil, Tomás Antonio - @Tomas-Gil17

Docente: Enzo Martín Zotti - División: 343

## Tecnologías utilizadas

- Python: Lenguaje principal
- Pandas: Carga, limpieza, manipulación y agregación de datos
- NumPy: Operaciones numéricas y columnas calculadas
- Matplotlib y Seaborn: Visualización de datos
- Scikit-Learn: Preprocesamiento (One-Hot Encoding, StandardScaler), partición train/test y regresión lineal
- Google Colab: Entorno de ejecución reproducible
- Git / GitHub: Control de versiones y publicación

## Estructura del repositorio
- tpi-analisis-de-datos/
   - data/
      - raw/Dataset original (WA_Fn-UseC_-Telco-Customer-Churn.csv)
      - processed/Dataset depurado y transformado
   
   - notebooks/
      - TPI_Analisis_de_Datos.ipynb: Notebook ejecutable en Google Colab
   
   - docs/
      - INFORME_EJECUTIVO.pdf: Informe técnico-ejecutivo
      
   - README.md

## Cómo explorar el proyecto

1. Hacé clic en el botón Open in Colab de arriba.
2. En Colab, andá a Entorno de ejecución → Ejecutar todas. El dataset se carga automáticamente desde este repositorio, no hace falta subir ningún archivo.
3. El notebook está organizado en secciones:
   - A. Fundamentos y clasificación de variables
   - B. Limpieza y calidad de datos
   - C. Manipulación de datos
   - D. Análisis exploratorio y visualización
   - E. Preprocesamiento y modelo de regresión
   - F. Conclusiones y recomendaciones
4. Para una lectura ejecutiva de los resultados, consultá el informe en [`docs/INFORME_EJECUTIVO.pdf`](docs/INFORME_EJECUTIVO.pdf).

## Dataset
Telco Customer Churn (IBM), disponible en [Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn). Contiene 7.043 clientes y 21 variables: datos sociodemográficos, servicios contratados, facturación y estado de cancelación (Churn).