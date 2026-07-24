# sprint7-final-project
#  Análisis de Clientes y Uso de Servicios — ConnectaTel

##  Objetivo del proyecto

El objetivo de este proyecto es analizar el comportamiento de los clientes de **ConnectaTel**, una empresa de telecomunicaciones con operaciones en Latinoamérica.

A partir de información sobre clientes, planes contratados y uso de los servicios, se busca identificar patrones de consumo, detectar valores atípicos y segmentar a los usuarios según sus características y nivel de uso.

El análisis busca generar información útil para apoyar decisiones relacionadas con la oferta de planes, la segmentación de clientes y la mejora de la experiencia del usuario.

---

##  Datasets utilizados

El análisis utiliza tres fuentes de datos:

### `plans.csv`
Contiene información sobre los planes disponibles, incluyendo características como precio, minutos, mensajes y datos incluidos.

### `users_latam.csv`
Contiene información de los clientes, incluyendo:

- Identificador del usuario.
- Edad.
- Ciudad.
- Fecha de registro.
- Plan contratado.
- Información de cancelación del servicio.

### `usage.csv`
Contiene los registros de uso de los servicios de los clientes:

- Identificador del usuario.
- Tipo de actividad (`call` o `text`).
- Fecha.
- Duración de llamadas.
- Longitud de mensajes.

---

##  Etapas del análisis

El proyecto se desarrolló siguiendo las siguientes etapas:

1. **Carga y exploración de datos**
   - Importación de los datasets.
   - Revisión de filas, columnas y tipos de datos.
   - Exploración inicial de las variables.

2. **Identificación de problemas de calidad**
   - Revisión de valores nulos.
   - Detección de valores inválidos y sentinels.
   - Revisión de fechas fuera de rango.

3. **Limpieza de datos**
   - Corrección de valores sentinels.
   - Tratamiento de valores nulos.
   - Conversión y validación de fechas.
   - Revisión de datos inconsistentes.

4. **Análisis estadístico**
   - Creación de métricas de uso por usuario.
   - Cantidad de llamadas.
   - Cantidad de mensajes.
   - Total de minutos de llamadas.
   - Análisis estadístico de variables numéricas y categóricas.

5. **Visualización y detección de outliers**
   - Histogramas para analizar distribuciones.
   - Boxplots para identificar valores extremos.
   - Comparación del comportamiento según el plan contratado.
   - Evaluación de outliers mediante el método IQR.

6. **Segmentación de clientes**
   - Segmentación por nivel de uso.
   - Segmentación por edad.
   - Visualización de los grupos identificados.

7. **Insight ejecutivo**
   - Interpretación de los principales hallazgos.
   - Identificación de oportunidades comerciales.
   - Recomendaciones para mejorar la oferta de planes y estrategias de segmentación.

---

##  Cómo ejecutar el proyecto

El análisis se encuentra desarrollado en un **Jupyter Notebook** y puede ejecutarse utilizando **Google Colab** o **Jupyter Notebook**.

### Opción 1: Google Colab

1. Abrir el repositorio de GitHub.
2. Abrir el archivo `.ipynb` del proyecto.
3. Abrir el notebook en Google Colab.
4. Asegurarse de tener disponibles los archivos:
   - `plans.csv`
   - `users_latam.csv`
   - `usage.csv`
5. Ejecutar las celdas del notebook en orden.

### Opción 2: Jupyter Notebook

1. Clonar o descargar el repositorio.
2. Instalar las librerías necesarias.
3. Colocar los datasets en la carpeta correspondiente.
4. Abrir el notebook.
5. Ejecutar las celdas secuencialmente.

Las principales librerías utilizadas son:

```python
pandas
numpy
seaborn
matplotlib
