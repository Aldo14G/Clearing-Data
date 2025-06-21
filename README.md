# Portafolio de Data Analytics: “History of Philosophy”

## Descripción del Proyecto
Este repositorio contiene el análisis exploratorio y la limpieza del dataset **History of Philosophy**, que recopila más de 300 000 oraciones extraídas de más de 50 textos clásicos de 10 escuelas filosóficas. El objetivo es demostrar capacidades de limpieza de datos, análisis de texto y visualizaciones en Python (pandas, Matplotlib, Seaborn).

## Fuente de Datos
- **Origen**: Kaggle — https://www.kaggle.com/datasets/kouroshalizadeh/history-of-philosophy  
- **Formato**: CSV  
- **Columnas principales**:  
  - `title`, `author`, `school`  
  - `sentence_str` (oración original)  
  - `original_publication_date`, `corpus_edition_date`  
  - `sentence_length`, `sentence_lowered`  
  - `tokenized_txt`, `lemmatized_str`

## Estructura del Notebook
1. **Configuración**  
   - Instalación y configuración de la API de Kaggle  
   - Descarga y descompresión del dataset  
2. **Carga y EDA Inicial**  
   - Lectura del CSV en un DataFrame  
   - Resumen de columnas, tipos y estadísticas descriptivas  
3. **Limpieza y Formateo**  
   - Conversión de fechas (años BCE como enteros, años CE a `datetime`)  
   - Detección y manejo de valores nulos y duplicados  
4. **Análisis Exploratorio**  
   - Histograma de longitud de oraciones  
   - Top 5 autores y escuelas  
   - Cálculo y visualización de las oraciones más repetidas (“citas más citadas”)  
5. **Visualizaciones**  
   - Barras estilizadas para autores y escuelas (Matplotlib + estilos predefinidos)  
   - Histogramas con curva de densidad (Seaborn)  
   - Opciones interactivas con Plotly (opcional)  

## Resultados Clave
- **Autores más frecuentes**:  
  1. Aristotle – 48 779 oraciones  
  2. Plato – 38 366  
  3. Hegel – 22 700  
  4. Foucault – 15 240  
  5. Heidegger – 15 239  

- **Escuelas más representadas**:  
  1. Analytic – 55 425 oraciones  
  2. Aristotle – 48 779  
  3. German Idealism – 42 136  
  4. Plato – 38 366  
  5. Continental – 33 779  

- **Citas más citadas** (top 10):  
  ```text
  54 veces → “Example Sentence A…”
  42 veces → “Example Sentence B…”
  …  
