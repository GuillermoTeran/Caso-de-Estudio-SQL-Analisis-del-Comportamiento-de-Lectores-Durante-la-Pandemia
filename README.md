# Caso de Estudio SQL: Análisis del Comportamiento de Lectores Durante la Pandemia

## ES Español

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

Creación de contenido basada en calidad percibida más que en volumen de calificaciones.


# SQL Case Study: Analysis of Reader Behavior During the Pandemic

## US ENglish

Project description:

During the COVID-19 pandemic, changes in social habits drove growth in book consumption and the development of new platforms for readers. In this project, I worked with a relational database from a startup in the publishing sector that is looking to launch a new digital product for readers. Using the available data, the goal was to identify valuable opportunities for this proposal.

## Project Objectives
Explore the database to understand reading and rating behavior.

Run SQL queries to extract key metrics on:

Recent publications

User Engagement

Author and publisher performance

Generate insights to inform product and strategy decisions.

## Database Description
The database contained five main tables:

Table    Content
books    Information about books: title, date, pages
authors    Authors
publishers    Publishers
ratings    Numerical ratings from users
reviews    Textual reviews from users

## Relationships:

Each book is related to an author and a publisher.

Ratings and reviews are linked to books via book_id.

## Technologies Used
SQL (PostgreSQL)

Jupyter Notebook

Python (Pandas only for printing results)

## Queries Performed and Key Findings
1. Books published after January 1, 2000
Result: An increasing volume of publications was identified after 2000, which supports the idea that the platform can focus on modern titles.

2. Average ratings and number of reviews per book
Data was grouped by book_id to calculate the average rating and number of reviews.

Result: Some highly rated titles were not the most popular in terms of the number of reviews, suggesting opportunities to highlight “hidden gems.”

3. Publisher with the most books over 50 pages
Filtered by books with more than 50 pages to exclude short publications or pamphlets.

Result: A leading publisher of extensive publications was identified, useful for commercial partnerships or editorial recommendations within the app.

4. Author with the best average rating (minimum 50 ratings)
Used a subquery to filter books with a sufficient volume of ratings.

Result: A reliable ranking of authors with good critical reception was obtained, ideal for highlighting quality content.

5. Average reviews by users with more than 50 ratings
The behavior of the most active users was analyzed.

Result: These users write more text reviews than average, so they could be leveraged as community ambassadors or content creators.

## General Conclusions
The combination of review data, ratings, and publisher metadata allows for the development of effective strategies for content personalization.

There are authors and books with high recommendation potential that are not yet widely recognized.

The most engaged users generate a significant volume of valuable content (reviews) and could be key to building loyalty.

## Value for the Product
Content segmentation is based on leading publishers or high-performing authors.

Focus on active users for engagement campaigns.

Content creation is based on perceived quality rather than volume of ratings.
