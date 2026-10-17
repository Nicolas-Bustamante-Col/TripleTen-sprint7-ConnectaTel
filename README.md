# 📌 Análisis de Consumo de Clientes - ConnectaTel
El siguiente repositorio contiene los datasets y el notebook utilizados para el análisis de comportamiento de los clientes de la compañía de telecomunicaciones ConnectaTel, correspondiente al Sprint 7 de la formación en Ciencia de Datos de TripleTen. El proyecto busca identificar patrones demográficos y de consumo que permitan evaluar el desempeño de los planes comerciales y generar recomendaciones orientadas a la toma de decisiones.

El estudio se enfoca en analizar la base de usuarios de la compañía de telecomunicaciones ConnectaTel para evaluar el rendimiento de sus planes comerciales actuales y descubrir patrones de comportamiento que impulsen la toma de decisiones estratégicas.

## 🎯 Objetivo del Proyecto
Identificar el perfil demográfico y los hábitos de consumo de los clientes de ConnectaTel para evaluar el desempeño de los planes comerciales actuales, con especial atención en el Plan Premium, y detectar oportunidades de mejora en el portafolio de servicios.

## 📊 Datasets Utilizados
El análisis integra tres datasets relacionados mediante el identificador único `user_id`:
*   `users`: Información demográfica de los clientes incluyendo edad, ciudad, fecha de registro y fecha de cancelación del servicio.
*   `usage`: Registros detallados de consumo incluyendo eventos de llamada, duración en minutos y longitud de mensajes de texto enviados.
*   `plans`: Catálogo de planes comerciales, con sus parámetros, características y tarifas base para los planes Básico y Premium.

## ⚙️ Etapas del Análisis Realizadas
1.  **Preprocesamiento y Limpieza de Datos:** Tratamiento de datos faltantes, corrección de fechas con incosistencias temporales, tratamiento de valores *sentinel* (-999) en la edad de los usuarios y validación estadística de datos MAR (Missing At Random) en variables de consumo.
2.  **Análisis Exploratorio de Datos (EDA):** Análisis de las distribuciones, tendencias y patrones de las principales variables de consumo mediante visualizaciones estadísticas.
3.  **Detección de Outliers:** Identificacion de valores atípicos con el método de Rango Intercuartílico (IQR), para diagnosticar la presencia de valores extremos en la distribución de las variables.
4.  **Segmentación Demográfica y de Uso:** Clasificación de usuarios por rangos de edad y niveles de uso para analizar diferentes perfiles de clientes.
5.  **Diagnóstico Ejecutivo y Recomendaciones:** Interpretacion de los resultados obtenidos y formulacion de recomendaciones estratégicas orientadas al negocio y su crecimiento económico.

## 🚀 Cómo Ejecutar el Notebook
Puedes visualizar y ejecutarl el análisis de forma inmediata en Gooble Colab:

1. Descarga el archivo `.ipynb` de este repositorio.
2. Ve a [Google Colab](https://colab.research.google.com/) e inicia sesión con tu cuenta de Google.
3. Selecciona Archivol → Subir notebook y carga el archivo descargado.
4. Ejecuta las celdas en orden, utilizando el botón de ejecución de cada celda o Shift + Enter.

## 🔄 Guía de Reproducción (Ejecución Local)
Si deseas replicar todo el flujo de trabajo en tu entorno local (Jupyter Notebook / VS Code), sigue estos pasos:

1. **Clonar el repositorio:**
   ```
   git clone [https://github.com](https://github.com/Nicolas-Bustamante-Col/TripleTen-sprint7-ConnectaTel/edit/main/README.md)
   cd TripleTen-sprint7-ConnectaTel
   ```
2. **Instalar dependecias:** Instala las librerías necesarias ejecutando en tu terminal:
   ```
   pip install pandas matplotlib seaborn
   ```
3. **Cargar los datos:** Verifica que los archivos `.csv` estén en las rutas esperadas por el notebook.
4. **Ejecutar secuencialmente:** Abre el entorno de Jupyter y ejecuta las celdas en orden secuencial (**Shift + Enter**) para mantener el flujo correcto de las variables en la memoria de Python.
