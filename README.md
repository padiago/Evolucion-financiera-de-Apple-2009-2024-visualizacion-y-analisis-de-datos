# 🍏 Apple Inc. Financial Evolution (2009–2024)

Este proyecto analiza la evolución financiera de **Apple Inc.** entre 2009 y 2024 utilizando **Python** para el procesamiento, limpieza y análisis de datos, y **Plotly / Folium / Seaborn** para la visualización interactiva.  
El objetivo es comprender cómo Apple ha gestionado su transición desde una etapa de expansión hacia una fase de madurez empresarial, manteniendo su rentabilidad, solidez financiera e innovación.

---

## ⚙️ Procesamiento y limpieza de datos con Python

El flujo de trabajo técnico se construyó de forma reproducible en **Jupyter Notebook**, con un enfoque modular:

### 1. Extracción y carga
- **Fuentes:** datos de *Macrotrends* y *Yahoo Finance* (financieros y bursátiles), además de un dataset manual de tiendas.  
- Archivos en formato `.csv` importados con `pandas.read_csv()` y combinados por año o país.

### 2. Limpieza y formateo
- Conversión de columnas con símbolos y texto a tipo numérico (`str.replace`, `pd.to_numeric`).
- Normalización de unidades (millones USD) y homogeneización de nombres de variables.
- Eliminación de duplicados, valores nulos y ajuste de tipos de datos (`astype`).
- Formateo de fechas y creación de columnas derivadas como **antigüedad de tiendas** (hasta 31/12/2024).

### 3. Ingeniería de variables
- Cálculo de indicadores clave:
  - **Márgenes (%)**: bruto, operativo y neto.
  - **Ratios financieros**: *Debt/EBITDA*, *Cash Ratio*, *Net Debt*, *P/E Ratio*.  
  - **CAGR (Compound Annual Growth Rate)** de ingresos y beneficios.
- Creación de métricas para el storytelling financiero (etapas de crecimiento, pandemia, consolidación).

### 4. Herramientas utilizadas

| Librería | Uso principal |
|-----------|----------------|
| **Pandas** | Limpieza y transformación de datos |
| **NumPy** | Cálculos numéricos y métricas financieras |
| **Plotly / Seaborn / Matplotlib** | Visualización (lineal, apilada e interactiva) |
| **Folium** | Mapa global de tiendas Apple |
| **Jupyter Notebook** | Desarrollo, documentación y análisis reproducible |

---

## 📈 Análisis financiero y visualización

Tras la depuración de los datos, el análisis se centró en **cuatro grandes bloques** para describir la evolución de Apple desde una perspectiva contable, bursátil y estratégica.

### 1. Rendimiento económico
- Evolución de **ingresos (Revenue)**, **EBITDA**, **beneficio bruto** y **neto**.  
- Estudio del **CAGR (2009–2024)** para medir el crecimiento medio anual.  
- Visualización: líneas de tendencia con hover interactivo.

### 2. Rentabilidad y retorno al accionista
- Análisis de **márgenes**: bruto, operativo y neto.  
- Evolución del **EPS (Earnings per Share)**.  
- Relación entre **Net Income y EPS** para evaluar la eficiencia del beneficio por acción.

### 3. Estructura financiera
- Comparativa **Cash on Hand vs. Long-Term Debt** mediante barras apiladas.  
- Cálculo y representación del ratio **Debt/EBITDA** como indicador de solvencia.  
- Análisis de la gestión prudente de deuda como palanca de crecimiento.

### 4. Valoración bursátil y contexto
- Relación entre el **precio ajustado de la acción** y el **P/E ratio** (Price-to-Earnings).  
- Inclusión de **eventos clave** (pandemia 2020, lanzamientos, stock splits) mediante anotaciones.  
- Visualización dual con ejes secundarios y hover para explorar la relación entre valor y resultados.

### 5. Expansión global
- Dataset con **países, fecha de primera tienda y número total de tiendas**.  
- Cálculo de la **antigüedad media** de las tiendas por país.  
- Mapa interactivo con **Folium** (color = edad media), mostrando la madurez geográfica de Apple.

---

## 📊 Principales visualizaciones

| Gráfico | Descripción |
|----------|-------------|
| **Ingresos y Beneficio Neto (2009–2024)** | Crecimiento sostenido y márgenes estables. |
| **Márgenes (%)** | Evolución de la rentabilidad por tipo de margen. |
| **Cash vs. Deuda a Largo Plazo** | Solidez financiera visualizada mediante barras apiladas. |
| **Debt/EBITDA Ratio** | Análisis de solvencia a lo largo del tiempo. |
| **Precio Acción vs. P/E Ratio** | Relación entre valoración de mercado y beneficios. |
| **Mapa Global de Tiendas Apple** | Expansión geográfica y antigüedad media por país. |

---

## 🧠 Conclusiones

- Apple mantiene una **trayectoria de crecimiento sólido** en ingresos, beneficios y capitalización bursátil.  
- Su **estructura financiera equilibrada** combina liquidez abundante con uso estratégico de la deuda.  
- La **pandemia de 2020** no fue un obstáculo, sino un **acelerador de transformación y rentabilidad**.  
- En 2024, Apple consolida su posición como una empresa **madura, rentable y resiliente**, sin perder su carácter innovador.
