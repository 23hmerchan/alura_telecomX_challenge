
# 📊 Análisis de Evasión de Clientes (Churn) – TelecomX

Este proyecto tiene como objetivo identificar los principales factores que influyen en la evasión de clientes (churn) en una empresa de telecomunicaciones, a partir del análisis de un conjunto de datos de 7,032 clientes.

---

## 🧾 Descripción del proyecto

A través de técnicas de análisis exploratorio de datos (EDA), se examinan variables contractuales, de facturación y de uso de servicios digitales para comprender los patrones de comportamiento que conducen a la pérdida de clientes. El análisis se apoya en visualizaciones claras, estadísticas descriptivas y cruces de variables para extraer conclusiones útiles para estrategias de retención.

---

## 📁 Estructura del análisis

1. **Carga y transformación de datos**
   - Limpieza de datos nulos
   - Conversión de tipos de datos (str, category, float, bool)
   - Agregado de columnas derivadas (como `has_internet`)

2. **Análisis general de churn**
   - Porcentaje global de evasión
   - Distribución por tipo de contrato

3. **Análisis por características del cliente**
   - `customer_Dependents`
   - `customer_Partner`
   - `customer_SeniorCitizen`

4. **Análisis de servicios digitales**
   - `internet_OnlineBackup`
   - `internet_TechSupport`
   - `internet_OnlineSecurity`
   - Gráficos de barras apiladas con porcentajes

5. **Análisis financiero**
   - Comparación de cargos mensuales y totales (`account_Charges_Monthly`, `account_Charges_Total`)
   - Gráficos de distribución (KDE y Boxplots) por `Churn`

---

## 📈 Resultados clave

- De 7,032 clientes, **1,869 abandonaron el servicio** (**26.6% de churn**).
- La **modalidad “Month-to-month” concentra el 42.7% del churn**, muy por encima de contratos anuales (11.5%) o bienales (3.4%).
- Los clientes **sin dependientes** tienen una tasa de churn del **31.6%**, frente a **16.7%** en quienes sí los tienen.
- La **falta de servicios digitales**, como `OnlineBackup`, incrementa el churn al **39.9%**, comparado con **21.6%** entre quienes sí lo tienen.
- Los cargos mensuales más altos están asociados con mayor probabilidad de evasión.

---

## 💡 Conclusión

El churn está fuertemente relacionado con la **inestabilidad contractual** y la **falta de adopción de servicios complementarios**. Para reducir la evasión, se recomienda:

- Incentivar **contratos a largo plazo**
- Promover el uso de **servicios digitales** (OnlineBackup, TechSupport, etc.)
- Enfocar estrategias de retención en clientes sin dependientes o con cargos altos

---

## 🔧 Requisitos técnicos

- Python 3.x  
- Bibliotecas:
  - `pandas`
  - `matplotlib`
  - `seaborn`

---

## 📂 Archivos

- `telecomx_transformado_total.csv`: conjunto de datos transformado
- `analisis_churn.ipynb`: notebook con el análisis paso a paso
- `README.md`: este documento
