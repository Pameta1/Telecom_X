# Proyecto de Análisis de Churn en Telecomunicaciones

## 📌 Descripción
Este proyecto tiene como objetivo analizar la evasión de clientes (*churn*) en una empresa de telecomunicaciones. 
Se utilizan técnicas de análisis exploratorio de datos (EDA) con **Python y pandas**, visualizaciones con **Seaborn y Matplotlib**, y métricas estadísticas para identificar patrones de cancelación de servicio.

## 🎯 Objetivos
- Explorar y limpiar el dataset de clientes.
- Identificar problemas en los datos (valores nulos, duplicados, inconsistencias).
- Transformar variables categóricas en numéricas para facilitar el análisis.
- Analizar la distribución de churn y su relación con variables como género, tipo de contrato y método de pago.
- Calcular correlaciones entre variables numéricas y churn.
- Generar métricas adicionales como **Cuentas Diarias** para entender mejor el comportamiento de los clientes.
- Proponer recomendaciones estratégicas para reducir la evasión.

## 🛠️ Tecnologías utilizadas
- Python 3.x  
- Pandas  
- NumPy  
- Seaborn  
- Matplotlib  
- Jupyter/Google Colab  

## 📊 Flujo de trabajo
1. **Exploración inicial**: revisión de columnas y tipos de datos.  
2. **Detección de problemas**: valores ausentes, duplicados, errores de formato.  
3. **Correcciones**: normalización de strings, conversión de variables numéricas.  
4. **Análisis descriptivo**: métricas estadísticas de las variables principales.  
5. **Visualización de churn**: distribución general y por variables categóricas.  
6. **Transformaciones**: creación de `Churn_bin` y `Cuentas_Diarias`.  
7. **Correlaciones**: análisis de relaciones entre variables numéricas y churn.  
8. **Conclusiones estratégicas**: recomendaciones para reducir la evasión.  

## 📈 Resultados clave
- El churn se concentra en clientes con **contratos mensuales** y **métodos de pago manuales**.  
- La **antigüedad (tenure)** es un factor protector contra la evasión.  
- Los clientes con **cargos mensuales más altos** muestran mayor tendencia a cancelar.  
- Promover **contratos largos y pagos automáticos** puede reducir significativamente el churn.  

## 📂 Estructura del repositorio
/data → datasets crudos y limpios /notebooks  → análisis exploratorio y pruebas /src → scripts de ETL y funciones auxiliares /reports → informes y visualizaciones README.md → descripción del proyecto
