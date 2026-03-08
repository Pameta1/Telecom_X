# 📑 Proyecto de Análisis de Evasión de Clientes (Churn)

![Estado del proyecto](https://img.shields.io/badge/estado-en%20progreso-yellow)
![Lenguaje](https://img.shields.io/badge/python-3.12-blue)
![Notebook](https://img.shields.io/badge/jupyter-notebook-orange)
![Licencia](https://img.shields.io/badge/licencia-MIT-green)
![Autor](https://img.shields.io/badge/autora-Pamela-purple)

## 🔹 Introducción
Este proyecto tiene como objetivo analizar el comportamiento de los clientes en relación con la **evasión (Churn)**, es decir, la cancelación del servicio.  
La evasión de clientes es un desafío crítico para las empresas de telecomunicaciones, ya que impacta directamente en los ingresos y en la sostenibilidad del negocio.  
El análisis busca identificar patrones y factores asociados al churn, con el fin de diseñar estrategias de retención más efectivas.

---

## 🔹 Limpieza y Tratamiento de Datos
1. **Importación de datos**: Se cargó el dataset original en un DataFrame de Pandas.  
2. **Revisión de columnas**: Se identificaron variables categóricas y numéricas.  
3. **Conversión de tipos**:
   - `MonthlyCharges`, `TotalCharges` y `tenure` fueron convertidas de texto a valores numéricos.  
4. **Creación de nuevas variables**:
   - `Cuentas_Diarias` = `MonthlyCharges / 30`  
   - `Gasto_Diario_Historico` = `TotalCharges / (tenure * 30)`  
5. **Normalización de categorías**:
   - Se aplicó One-Hot Encoding a la variable objetivo `cancelacion`, generando `cancelacion_Yes` y `cancelacion_No`.  
   - Se seleccionó **`cancelacion_Yes`** como variable principal para el análisis.  
6. **Homogeneización de nombres de columnas**: Se renombraron columnas para mantener consistencia y evitar errores.

---

## 🔹 Análisis Exploratorio de Datos (EDA)
### Distribución de la variable objetivo
- Gráficos de barras y circulares para visualizar la proporción de clientes que cancelaron vs. los que permanecieron.

### Variables categóricas
- Análisis de evasión según género, tipo de contrato, método de pago y servicio de internet.  
- Visualizaciones con `countplot` y tablas porcentuales.

### Variables numéricas
- Boxplots y histogramas comparativos para `MonthlyCharges`, `TotalCharges`, `tenure` y `Cuentas_Diarias`.  
- Se identificaron patrones de cancelación asociados a cargos altos y menor tiempo de contrato.

### Correlaciones (opcional)
- Matriz de correlación entre variables numéricas.  
- Ranking de correlaciones respecto a `cancelacion_Yes`.  
- Gráficos de dispersión para explorar relaciones específicas.

---

## 🔹 Conclusiones e Insights
- La evasión está más concentrada en clientes **nuevos** (bajo tenure).  
- Los clientes con **cargos mensuales altos** muestran mayor propensión a cancelar.  
- El gasto diario (`Cuentas_Diarias`) también se asocia con mayor churn.  
- La variable `cancelacion_Yes` es la más adecuada para modelar y entender el comportamiento de los clientes.

---

## 🔹 Recomendaciones Estratégicas
1. **Fidelización temprana**: ofrecer beneficios a clientes en sus primeros meses.  
2. **Planes flexibles**: diseñar opciones más atractivas para clientes con cargos altos.  
3. **Monitoreo continuo**: implementar dashboards para seguir la evolución del churn en tiempo real.  
4. **Campañas personalizadas**: segmentar acciones según contrato, método de pago y servicio de internet.  
5. **Modelos predictivos**: entrenar un modelo de machine learning con `cancelacion_Yes` como variable objetivo.

---

## 🔹 Próximos pasos
- Implementar un modelo de clasificación (ej. regresión logística, random forest) para predecir churn.  
- Validar el modelo con métricas como **accuracy, precision, recall y F1-score**.  
- Integrar el análisis en un pipeline automatizado para monitoreo continuo.

---

👩‍💻 **Autora**: Pamela Tapia Desarrolladora web en formación, apasionada por la accesibilidad, la lógia interactiva y el aprendizaje colaborativo.

pamelatapiaptp@gmail.com

https://www.linkedin.com/in/pamelatapiaponce/

📅 **Fecha**: Marzo 2026  
