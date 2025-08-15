# 📊 Proyecto de Predicción de Demanda en Retail

Este repositorio contiene el desarrollo completo de una prueba técnica orientada a **analizar, visualizar y predecir la demanda** en un contexto de **industria retail**, utilizando un dataset realista con ventas, sucursales, categorías y datos de stock.

---

## 🚀 Objetivo

Optimizar el proceso de **abastecimiento y compras a proveedores** mediante un modelo de predicción de demanda soportado en análisis exploratorio, ingeniería de características, visualizaciones clave y pronósticos.

---

## 📂 Estructura del Proyecto

.
├── input/ # Dataset original y datos intermedios  
├── slides/ # Presentacion ejecutiva  
├── Documento/ # # PDF de propuesta y gobernanza  
├── output/ #Datasets limpios  
│ ├── images/ # Visualizaciones generadas  
├── notebooks/ #Análisis exploratorio y desarrollo de modelo  
│ ├── Preprocessingelec.ipynb # Limpieza y preparación de datos  
| ├── PreprocessingMascota.ipynb # Limpieza y preparación de datos  
│ ├── productos.ipynb # Limpieza de datos  
│ ├── locations.ipynb # Limpieza de datos  
│ |── ModelValidation.ipynb # Entrenamiento de modelos  
│ └── ModelValidationMascota.ipynb # Entrenamiento de modelos  
└── README.md # Este archivo  


---

## 🧠 Metodología

El desarrollo se estructuró en **8 etapas** siguiendo buenas prácticas de *data science pipeline*:

1. **Ingesta y limpieza de datos**
   - Conversión de fechas a formato `datetime`.
   - Control de nulos, duplicados y tipos de datos.
   - Normalización de nombres de columnas.

2. **Análisis exploratorio (EDA)**
   - Distribución de ventas por fecha, sucursal y categoría.
   - Top productos, top sucursales, y ventas desde otra ubicación.
   - Insight adicional: rentabilidad (`ganancia` y `margen`).

3. **Ingeniería de características**
   - Variables de estacionalidad: mes, día de la semana, feriados.
   - Agregaciones por mes/sucursal/categoría.
   - Feature de *lead time* para logística.

4. **Visualizaciones clave**
   - Series de tiempo (total, por sucursal y categoría).
   - Comparativas de sucursales top.
   - Volumen mensual desde otra ubicación.

5. **Modelado**
   - Modelos de pronóstico (ARIMA/SARIMAX, Prophet).
   - Validación temporal con *walk-forward*.

6. **Evaluación**
   - Métricas: MAE, MAPE.
   - Comparación vs. Data historica.

7. **Propuesta de implementación**
   - Integración al proceso de compras.
   - Automatización del pipeline.
   - Monitoreo de performance.

8. **Gobernanza de datos**
   - Políticas de calidad.
   - Actualización de modelos.
   - Roles y responsabilidades.

---

## 📊 Principales Visualizaciones

| Visualización                                   | Descripción |
|-------------------------------------------------|-------------|
| `serie_tiempo_total.png`                        | Volumen total diario. |
| `serie_tiempo_sucursal.png`                     | Series por sucursal. |
| `serie_tiempo_categoria.png`                    | Series por categoría. |
| `top5_dias_top3_sucursales_color_categoria.png` | Top 5 días de las 3 sucursales más vendidas, coloreado por categoría dominante. |
| `sucursales_mayor_volumen_mensual.png`          | Volumen mensual desde otra ubicación. |

---

## 📑 Documentación Entregada

- **[Propuesta de Implementación del Modelo de Predicción](output/reports/propuesta_modelo_prediccion_demanda.pdf)**  
  Documento que describe:
  - Integración del modelo al proceso de compras.
  - Automatización propuesta.
  - Monitoreo de performance.
  - Gobernanza de datos.

---

## 🛠️ Tecnologías utilizadas

- **Lenguaje**: Python 3.10
- **Librerías**: pandas, seaborn, matplotlib, statsmodels, prophet, scikit-learn
- **Control de versiones**: Git + GitHub
- **Documentación**: Markdown + PDF 
- **Visualizaciones**: Seaborn, Matplotlib

---

## 📈 Resultados clave

- Pronostico de los 3 siguientes meses de los productos vendidos.
- Potencial optimización del capital inmovilizado en inventario.
- Identificación de patrones estacionales y categorías más rentables.

---

## 📬 Contacto

**Autor**: *Marlon Segarra*  
**Email**: *marlon_sz@hotmail.es*  
* 