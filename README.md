# MOOCs (Massive Open Online Course)


## Index 
- [MOOCs (Massive Open Online Course)](#moocs-massive-open-online-course)
  - [Index](#index)
  - [Introducción](#introducción)
  - [Objetivos](#objetivos)
  - [ETL](#etl)
  - [EDA](#eda)
  - [Dashboard](#dashboard)
  - [KPIs](#kpis)
  
## Introducción

Este es mi proyecto de MOOCs de la carrera de Data Science de Henry. En proyecto nos pidieron situarnos en el rol de un Data Analyst. Por lo cual nos acercan un tickert de una startup de tecnología que está interesada en sumarse al mercado de cursos online, pero de una manera eficiente, por lo que compró datasets de posibles competidores (Coursera, Udemy, edX) para analizar y sacar conclusiones de los datos recolectados. Nuestro objetivo es generar un dashboard con nuestro análisis de los datos presentados

## Objetivos
- Realizar un análisis exploratorio de los datos en un notebook. 
- Generar un dashboard funcional y coherente con el storytelling.
- Generar un análisis y conclusiones a partir de los dataset entregados
- Sugerir 3 KPIs y mostrarse en el dashboard.

## ETL
Realicé un proceso de ETL sobre los Datasets proporcionados para prepararlo para el análisis, primero realicé las transformaciones que creí necesarias como eliminación de dulplicados, cambio de nombre de columna, normalización de datos, extracción de fechas y valores. También elimine las filas que no tuvieran datos para la columna numero de suscriptores ya que decidí basar mi análisis, principalmente, en la cantidad de alumnos. 
Luego tomé la decisión de generar un solo data set en conjunto con las tres plataformas para poder tener un análisis más general, por lo que agregué la columna plataforma para poder identificarlas luego. 
Generé también tres dataset por separado para poder generar análisis de cada uno de ellos.

## EDA
Utilicé los datos resultantes del proceso de Extracción, Transformación y Carga (ETL) para llevar a cabo el Análisis Exploratorio de Datos (EDA). Cada una de las columnas fue analizada con la asistencia de la herramienta ProfileReport de la biblioteca ydata_profiling.

Dicho análisis se encuentra disponible en el repositorio bajo el nombre de "profiling". A su vez, llevé a cabo el Análisis Exploratorio sobre las tres plataformas en conjunto, con el propósito de descubrir nueva información y generar conocimientos internos. Estos resultados pueden ser visualizados en el cuaderno EDA.

Entre los hallazgos más destacados se encuentran:
- La mayoría de los alumnos realizan cursos de nivel inicial y para todos los niveles
- Aunque en la distribución de la variable numérica se evidencia una mayor presencia de cursos pagos en comparación con los gratuitos, es importante destacar que la mayoría de los alumnos opta por realizar cursos gratuitos.
- Es interesante notar que la mayoría de las personas que eligen pagar por cursos con un precio de 200 USD se orientan hacia temáticas relacionadas con el desarrollo (development). Además, resulta llamativo que las categorías de los cursos más económicos pero más populares sean las mismas que las de los cursos más costosos. A pesar de esto, la temática de desarrollo continúa siendo la que genera mayores ingresos. Generandose un top 4 en ambas de desarrollo, diseño, finanzas y música
- Es interesante observar que los precios más comunes por los que la mayoría de las personas pagaron por el certificado de sus cursos fueron 49.0, 99.0, 199.0, 90.0 y 50.0. 
- Las temáticas con mayor número de estudiantes que pagan entre 49 y 200 USD por sus cursos son Computer Science, Business & Management, Humanities, Communication, Biology & Life Sciences, y Data Analysis & Statistics.
- La mayoría de los estudiantes optan por cursos en inglés y gratuitos. Sin embargo, cantidades similares de alumnos eligen cursos pagos en inglés y cursos gratuitos en español.
- Podemos observar que los cursos con una cantidad significativa de alumnos (por encima de 50.000) son mayormente gratuitos y se imparten en idiomas como Italiano, Francés, Japonés, Chino y Portugués. Esto demuestra el interés de los alumnos por cursos en esos idiomas específicos.

## Dashboard
Una vez concluido el Análisis Exploratorio de Datos (EDA), empleé la herramienta Power BI para elaborar una presentación con paneles de control (dashboards). Dicha presentación se encuentra disponible en el repositorio bajo el nombre de "Dashboard.pbix".

Es importante destacar que, si bien el EDA se realizó considerando las tres plataformas en conjunto, en la presentación se creó un panel de control individual para cada plataforma. Lamentablemente, debido a la falta de datos suficientes y relevantes, no pude incluir la plataforma Coursera en mi análisis. A pesar de utilizar los conjuntos de datos proporcionados y otros adicionales que encontré, no pude generar un conjunto de datos que contara con la cantidad necesaria de información para obtener un análisis significativo.

## KPIs
Generé cuatro propuestas de KPI s:
- Variación anual de recaudación por cursos publicados: Este KPI evalúa la variación porcentual de la recaudación generada a través de los cursos publicados en comparación con el año anterior.

- Promedio de rating anual: Este KPI calcula el promedio de las calificaciones recibidas por los cursos a lo largo de los años. Ayuda a comprender el rendimiento promedio de los cursos en términos de satisfacción de los estudiantes y calidad percibida.

- Tasa de conversión anual: La tasa de conversión anual es un indicador que mide el porcentaje de usuarios pagos sobre los usuarios gratuitos. 

- Variación de la tasa de conversión: Este KPI evalúa la variación porcentual de la tasa de conversión en comparación al año anterior.
  

Todos estos indicadores clave de rendimiento (KPIs) se encuentran disponibles para su visualización en la pestaña designada como "KPIs" en el panel de control (dashboard). Asimismo, dichos KPIs se complementan insights que orientan toda mi presentación.

Uno de los insights relevantes se relaciona con la dirección actual del negocio en el ámbito de las MOOCs. Se destaca la importancia de centrarse en cursos que brinden herramientas para abordar las demandas laborales del futuro. Específicamente, se enfatiza la relevancia de áreas como el desarrollo (Development), ciencias de la computación (Computer Science), análisis de datos (Data Analysis) y gestión empresarial (Business Management).

Estos insights evidencian la necesidad de adaptarse a las tendencias emergentes en el mercado laboral y resaltar la importancia de ofrecer programas educativos que estén alineados con las habilidades y conocimientos requeridos en los ámbitos mencionados.