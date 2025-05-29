# Caso de Estudio SQL: Análisis del Comportamiento de Lectores Durante la Pandemia
Descripción del proyecto:

Durante la pandemia por COVID-19, el cambio en los hábitos sociales impulsó el crecimiento del consumo de libros y el desarrollo de nuevas plataformas para lectores. En este proyecto, trabajé con una base de datos relacional de una startup del sector editorial que busca lanzar un nuevo producto digital para lectores y lectoras. A partir de los datos disponibles, el objetivo era identificar oportunidades de valor para esta propuesta.

## Objetivos del Proyecto
Explorar la base de datos para entender el comportamiento de lectura y calificación.

Ejecutar consultas SQL para extraer métricas clave sobre:

Publicaciones recientes

Participación de usuarios

Rendimiento de autores y editoriales

Generar insights que fundamenten decisiones de producto y estrategia.

## Descripción de la Base de Datos
La base de datos contenía cinco tablas principales:

Tabla	Contenido
books	Información sobre libros: título, fecha, páginas
authors	Autores/as
publishers	Editoriales
ratings	Calificaciones numéricas de los usuarios
reviews	Reseñas textuales de los usuarios

## Relaciones:

Cada libro está relacionado con un autor y una editorial.

Las calificaciones y reseñas están vinculadas a los libros mediante book_id.

## Tecnologías Utilizadas
SQL (PostgreSQL)

Jupyter Notebook

Python (Pandas solo para impresión de resultados)

## Consultas Realizadas y Hallazgos Clave
1. Libros publicados después del 1 de enero del 2000
Resultado: Se identificó un volumen creciente de publicaciones tras el año 2000, lo cual respalda la idea de que la plataforma puede enfocarse en títulos modernos.

2. Calificaciones promedio y número de reseñas por libro
Se agruparon datos por book_id para calcular el promedio de calificación y la cantidad de reseñas.

Resultado: Algunos títulos altamente calificados no eran los más populares en número de reseñas, lo que sugiere oportunidades para destacar “joyas ocultas”.

3. Editorial con más libros de más de 50 páginas
Filtro por libros con más de 50 páginas para excluir publicaciones cortas o folletos.

Resultado: Se identificó una editorial líder en publicaciones extensas, útil para alianzas comerciales o recomendaciones editoriales dentro de la app.

4. Autor con la mejor calificación promedio (mínimo 50 ratings)
Utilicé una subconsulta para filtrar libros con suficiente volumen de calificaciones.

Resultado: Se obtuvo un ranking confiable de autores con buena recepción crítica, ideal para destacar contenido de calidad.

5. Reseñas promedio por usuarios con más de 50 calificaciones
Se analizó el comportamiento de los usuarios más activos.

Resultado: Estos usuarios escriben más reseñas de texto que el promedio, por lo que podrían ser aprovechados como embajadores de la comunidad o creadores de contenido.

## Conclusiones Generales
La combinación de datos de reseñas, calificaciones y metadatos editoriales permite desarrollar estrategias efectivas para personalización de contenido.

Existen autores y libros con alto potencial de recomendación que aún no son ampliamente reconocidos.

Los usuarios más comprometidos generan un volumen significativo de contenido valioso (reseñas), y podrían ser clave para la fidelización.

## Valor para el Producto
Segmentación de contenido según editoriales líderes o autores de alto rendimiento.

Enfoque en usuarios activos para campañas de participación.

Curación de contenido basada en calidad percibida más que en volumen de calificaciones.
