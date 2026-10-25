# 🛒 Proyecto Integrador Final: Segmentación de Clientes y Sistema de Recomendación

**Diplomatura en Data Science y Analítica de Datos — UTN FRBA**  
**Autora:** Angela Cardozo  
**Fecha de Entrega:** Octubre de 2026  

---

## 📋 Descripción del Proyecto
Este proyecto implementa una solución integral de Machine Learning aplicada a un entorno de comercio electrónico (*Online Retail*), estructurada bajo la metodología **CRISP-DM**. El desarrollo comprende:
1. **Segmentación de Clientes (K-Means):** Creación de variables RFM (Recencia, Frecuencia, Monetario), transformación logarítmica y agrupación en 4 clústeres comerciales clave (*VIP, Leales, Prometedores y En Riesgo*).
2. **Sistema de Recomendación (Filtrado Colaborativo):** Motor de recomendación Usuario-Usuario basado en similitud de coseno para superar las limitaciones de los métodos genéricos de *Top-Sellers*.
3. **Evaluación de Impacto y Validación Temporal:** Validación mediante un corte temporal estricto (*Holdout 9m/3m*) para evitar *data leakage*, midiendo métricas de negocio ($Precision@5$, $Recall@5$ y $MRR$) y estimación de ROI.

---

## 📂 Estructura del Repositorio
* `Proyecto_Integrador_EntregaFinal.ipynb` — Notebook principal con todo el código de análisis, EDA, modelado y métricas ejecutado en **Google Colab**.
* `informe_final.pdf` — Informe escrito formal del proyecto (Formato institucional UTN).
* `presentacion.pdf` — Presentación visual en formato de diapositivas para la defensa oral (12 páginas).

---

## ⚙️ Instrucciones de Ejecución (Google Colab)

Dado que todo el pipeline fue desarrollado y probado en **Google Colab**, podés reproducirlo de manera inmediata siguiendo estos pasos:

1. Hacé clic directamente sobre el archivo `.ipynb` en este repositorio de GitHub y seleccioná la opción de abrir con Google Colab.
2. El notebook descarga de forma automatizada el dataset oficial y aplica el pipeline de preprocesamiento.
3. Se han fijado semillas aleatorias (`random_state = 42`) en todos los algoritmos de Machine Learning para garantizar la **reproducibilidad exacta** de los resultados y métricas presentados en el informe.
4. Ejecutá las celdas de manera secuencial (`Runtime -> Run all` / `Ejecutar todas`).
