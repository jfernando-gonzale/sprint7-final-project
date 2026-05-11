# sprint7-final-project

# 📊 Análisis ConnectaTel

## 📌 Objetivo del proyecto

El objetivo de este proyecto es analizar el comportamiento de los clientes de ConnectaTel, una empresa de telecomunicaciones en Latinoamérica, utilizando información de usuarios, planes y uso real del servicio.

A través del análisis se busca:

- Detectar problemas de calidad de datos.

- Identificar valores atípicos (outliers).

- Analizar patrones de llamadas y mensajes.

- Crear segmentaciones de clientes por edad y nivel de uso.

- Generar insights de negocio y recomendaciones comerciales.

---

## 📂 Datasets utilizados

El proyecto utiliza tres archivos CSV:

### 1. `plans.csv`

Contiene información sobre los planes disponibles:

- precio

- minutos incluidos

- GB incluidos

- costos adicionales

### 2. `users_latam.csv`

Información de los usuarios:

- edad

- ciudad

- fecha de registro

- plan contratado

- churn

### 3. `usage.csv`

Información del uso real del servicio:

- llamadas

- duración de llamadas

- mensajes

- fechas de actividad

---

## ⚙️ Etapas del análisis realizadas

### 1. Carga y exploración de datos

- Importación de librerías.

- Lectura de archivos CSV.

- Exploración inicial con `.head()`, `.shape()` y `.info()`.

### 2. Identificación de problemas de calidad

- Revisión de valores nulos.

- Detección de sentinels.

- Validación de fechas.

- Revisión de columnas categóricas y numéricas.

### 3. Limpieza de datos

- Reemplazo de sentinels (`-999`).

- Conversión de fechas.

- Manejo de valores faltantes.

- Corrección de valores inválidos.

### 4. Estadísticas y agregaciones

- Agrupación de uso por usuario.

- Creación de métricas agregadas:

  - cantidad de mensajes

  - cantidad de llamadas

  - minutos totales

### 5. Visualización y detección de outliers

- Histogramas.

- Boxplots.

- Identificación de distribuciones sesgadas.

- Detección de valores extremos con IQR.

### 6. Segmentación de clientes

- Segmentación por edad.

- Segmentación por nivel de uso.

- Creación de variables categóricas usando `np.where()`.

### 7. Insights ejecutivos

- Interpretación de resultados.

- Recomendaciones de negocio.

- Identificación de oportunidades comerciales.

---

## ▶️ Cómo ejecutar el notebook

### Opción 1 — Google Colab

1. Abrir el notebook `.ipynb` en Google Colab.

2. Subir los archivos CSV a la carpeta `/datasets/`.

3. Ejecutar las celdas en orden.

### Opción 2 — Jupyter Notebook

1. Instalar dependencias:

```bash

pip install pandas numpy matplotlib seaborn
