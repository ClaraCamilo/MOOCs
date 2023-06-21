Disclaimer:
caratecristicas de los dataset
precio
cantidad de cursos
numero de suscriptores


EDA:
Para el EDA tomé tres caminos diferentes, buscar que tipo de contenido generan las plataformas, cual es la temática con mayor cantidad de cursos, cuales de estos son pagos y cuales gratis, cual es el nivel de la myoria de los cursos.
Por otro lado fui por un enfoque de cantidad de suscriptores por curso 
Y por último el rating de los cursos 
Enlace de donde saque los dataset:
https://www.kaggle.com/datasets/anasmahmood000/coursera-courses-dataset?select=webautomation_coursera.csv
https://www.kaggle.com/datasets/hossaingh/udemy-courses?select=Comments.csv

Conclusiones EDA:
De este **análisis de distribución de variables categóricas**, puedo inferir que la mayoría de los cursos son para principiantes o de todos los niveles. Además, casi todos se dictan en inglés y el 60% son pagos. Esto se muestra así porque, de los datos proporcionados, el 60% pertenece a la plataforma Udemy. Sin embargo, no se sigue la relación real entre la cantidad de cursos por plataforma. Por ejemplo, Coursera tiene alrededor de 7000 cursos, pero en nuestros datos solo tenemos 500. Además, no tenemos información sobre los precios de los cursos. Por estas razones, el dataset queda desbalanceado y muestra una mayor cantidad de cursos de pago.

Por otro lado, la mayor cantidad de cursos se enfocan en desarrollo, finanzas, música y diseño. Esto también se refleja en la nube de palabras de los títulos de los cursos. Entre las palabras que más se repiten, encontramos "beginners" e "introduction", lo cual indica que la mayoría de los cursos son para principiantes. También se mencionan las palabras "trading", "design", "guitar", "piano" y "development", que hacen referencia a las temáticas con mayor cantidad de cursos.
- En el gráfico observamos que el idioma inglés predomina en la muestra de datos, lo cual nos lleva a realizar un análisis más detallado excluyendo este idioma. De esta forma, podremos comprender el comportamiento de los demás idiomas en relación a su condición de ser cursos pagos o gratuitos.
- Podemos ver que los cursos que se dictan en otros idiomas que no sean ingles o español son mayormente pagos
- Podemos observar que las categorías con mayor cantidad de cursos son predominantemente de pago, mientras que el resto de categorías ofrecen sus cursos de forma gratuita.
- Podemos observar que la gran mayoría de los cursos de nivel experto se imparten en inglés. Asimismo, los cursos que no están en inglés tienden a ser dirigidos a principiantes. Por lo tanto, se puede concluir que si se desea alcanzar un nivel experto en un determinado tema, es necesario tener conocimientos de inglés.
  
**El análisis de la relación entre las variables categóricas** me conduce a investigar la relación existente entre la cantidad de estudiantes que optan por realizar cursos en idiomas distintos al inglés. Esto nos ayudará a comprender si existe un mercado potencial en esa área. Además, buscamos examinar la relación entre los niveles de los cursos y la cantidad de alumnos que los eligen, con el fin de determinar si la creación de una cantidad significativa de cursos para principiantes resulta beneficiosa. También nos interesa explorar cómo se vincula esta información con los cursos pagos, con el propósito de evaluar si existe una estrategia en la cual los cursos para principiantes sean gratuitos y posteriormente los cursos de nivel intermedio o experto son pagos. 
Además, me lleva a investigar la relación existente entre la categoría de los cursos, el número de alumnos y su precio, a fin de determinar en qué temáticas resultaría más beneficioso generar una mayor cantidad de cursos.

- Hemos observado que la mayoría de los cursos presentan precios inferiores a 100 USD, tanto en lo que respecta al costo del curso en sí como al pago de la certificación en aquellos cursos que la ofrecen. Además, hemos notado un pico en el valor de 200 USD.
- Las observaciones que se pueden deducir de estos gráficos se explican por la presencia de cursos con un número reducido pero frecuente de alumnos, mientras que los cursos con una gran cantidad de estudiantes presentan una frecuencia más baja. Prestaremos especial atención a los cursos con una gran cantidad de alumnos, a pesar de que su frecuencia de repetición sea menor.
- La gran mayoría de los cursos obtienen una calificación superior a 3.5 puntos. Entiendo que esto ocurre debido a que cuando un estudiante comienza un curso que no le agrada, lo abandona después de algunas clases, es decir, no logra completarlo y busca otro curso. Esto hace que solo se califiquen aquellos cursos que se completan, es decir, aquellos que son del agrado o interés de los alumnos.
- En este gráfico podemos observar dos categorías distintas de duración. Por un lado, encontramos cursos con duraciones inferiores a 80 horas, mientras que por otro lado, encontramos cursos que abarcan desde 500 hasta 3000 horas. Esta diferencia se debe a dos modalidades de trabajo diferentes: la primera corresponde a la plataforma Udemy, donde los cursos suelen tener una duración más corta, y la otra corresponde a la plataforma edX, donde los cursos se extienden a lo largo de semanas.

**A partir del análisis de la distribución de las variables numéricas**, me surge la necesidad de investigar la relación existente entre los precios de los cursos y la cantidad de alumnos que los eligen, con el objetivo de identificar posibles temáticas por las cuales los alumnos estén dispuestos a pagar un mayor precio. Asimismo, me resulta de interés indagar sobre qué categorías no reciben calificación, así como también los de mayor rating, con el propósito de tomarlo en consideración al momento proponer la generación de diferentes cursos.
Por último, investigaré si existe alguna relación entre la duración de los cursos y los alumnos inscriptos, con el propósito de determinar si la duración del curso tiene alguna influencia en la cantidad de estudiantes que lo eligen.

**Correlaciones** 

Las categorías con más de 1 millón de alumnos son las siguientes: "Biology & Life Sciences", "Business & Management", "Business Essentials", "Communication", "Computer Science", "Data Analysis", "Data Analysis & Statistics", "Development", "Engineering", "Finance & Accounting", "Humanities", "Language", "Social Sciences" y "Software Development".

La mayoría de los alumnos realizan cursos de nivel inicial y para todos los niveles

Aunque en la distribución de la variable numérica se evidencia una mayor presencia de cursos pagos en comparación con los gratuitos, es importante destacar que la mayoría de los alumnos opta por realizar cursos gratuitos.

He realizado un segundo gráfico que muestra la cantidad de alumnos que realizan cursos gratuitos pero tienen la opción de obtener un certificado pago. En dicho gráfico se observa que la gran mayoría de los alumnos que optan por cursos gratuitos también tienen la posibilidad de adquirir certificados pagos.

Se observa un pico notable en los montos que los alumnos pagan por curso. La mayoría de los cursos pagos tienen un valor de 200 USD, seguido de otro pico significativo en 20 USD.

Es interesante notar que la mayoría de las personas que eligen pagar por cursos con un precio de 200 USD se orientan hacia temáticas relacionadas con el desarrollo (development). Además, resulta llamativo que las categorías de los cursos más económicos pero más populares sean las mismas que las de los cursos más costosos. A pesar de esto, la temática de desarrollo continúa siendo la que genera mayores ingresos. Generandose un top 4 en ambas de desarrollo, diseño, finanzas y música

Es interesante observar que los precios más comunes por los que la mayoría de las personas pagaron por el certificado de sus cursos fueron 49.0, 99.0, 199.0, 90.0 y 50.0. Para obtener una mejor comprensión de si existe alguna relación entre estos precios y las categorías de los cursos, realizaré un análisis agrupando los datos por categorías.

Las temáticas con mayor número de estudiantes que pagan entre 49 y 200 USD por sus cursos son Computer Science, Business & Management, Humanities, Communication, Biology & Life Sciences, y Data Analysis & Statistics.

La mayoría de los estudiantes optan por cursos en inglés y gratuitos. Sin embargo, cantidades similares de alumnos eligen cursos pagos en inglés y cursos gratuitos en español.

Podemos observar que los cursos con una cantidad significativa de alumnos (por encima de 50.000) son mayormente gratuitos y se imparten en idiomas como Italiano, Francés, Japonés, Chino y Portugués. Esto demuestra el interés de los alumnos por cursos en esos idiomas específicos.