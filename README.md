# Caso de Estudio SQL: Análisis del Comportamiento de Lectores Durante la Pandemia

## ES Español

**Rol:** Analista de Datos  
**Tecnologías:** SQL (PostgreSQL), Python (Pandas), Jupyter Notebook

### Descripción del proyecto  
Durante la pandemia por COVID-19, el cambio en los hábitos sociales impulsó el crecimiento del consumo de libros y el desarrollo de nuevas plataformas para lectores. En este proyecto, trabajé con una base de datos relacional de una startup del sector editorial que busca lanzar un nuevo producto digital para lectores y lectoras. El objetivo fue identificar oportunidades de valor para esta propuesta a partir del análisis de los datos.

### Objetivos del Proyecto  
- Explorar la base de datos para entender el comportamiento de lectura y calificación.  
- Ejecutar consultas SQL para extraer métricas clave sobre:  
  - Publicaciones recientes  
  - Participación de usuarios  
  - Rendimiento de autores y editoriales  
- Generar insights que fundamenten decisiones de producto y estrategia.

### Descripción de la Base de Datos  
La base de datos contenía cinco tablas principales:  

| Tabla      | Contenido                                 |  
|------------|------------------------------------------|  
| books      | Información sobre libros: título, fecha, páginas |  
| authors    | Autores/as                               |  
| publishers | Editoriales                              |  
| ratings    | Calificaciones numéricas de los usuarios|  
| reviews    | Reseñas textuales de los usuarios       |

Cada libro está relacionado con un autor y una editorial. Las calificaciones y reseñas están vinculadas a los libros mediante `book_id`.

### Tecnologías Utilizadas  
- SQL (PostgreSQL)  
- Jupyter Notebook  
- Python (Pandas solo para impresión de resultados)

### Consultas Realizadas y Hallazgos Clave  
1. **Libros publicados después del 1 de enero del 2000**  
   Resultado: Se identificó un volumen creciente de publicaciones tras el año 2000, apoyando un enfoque en títulos modernos.

2. **Calificaciones promedio y número de reseñas por libro**  
   Resultado: Algunos títulos altamente calificados no eran los más populares en número de reseñas, lo que sugiere oportunidades para destacar “joyas ocultas”.

3. **Editorial con más libros de más de 50 páginas**  
   Resultado: Se identificó una editorial líder en publicaciones extensas, útil para alianzas comerciales o recomendaciones dentro de la app.

4. **Autor con la mejor calificación promedio (mínimo 50 ratings)**  
   Resultado: Ranking confiable de autores con buena recepción crítica, ideal para destacar contenido de calidad.

5. **Reseñas promedio por usuarios con más de 50 calificaciones**  
   Resultado: Usuarios muy activos escriben más reseñas de texto que el promedio, por lo que podrían ser embajadores de la comunidad o creadores de contenido.

### Conclusiones Generales  
- La combinación de datos de reseñas, calificaciones y metadatos editoriales permite desarrollar estrategias efectivas para personalización de contenido.  
- Existen autores y libros con alto potencial de recomendación que aún no son ampliamente reconocidos.  
- Los usuarios más comprometidos generan un volumen significativo de contenido valioso (reseñas) y podrían ser clave para la fidelización.

### Valor para el Producto  
- Segmentación de contenido según editoriales líderes o autores de alto rendimiento.  
- Enfoque en usuarios activos para campañas de participación.  
- Creación de contenido basada en calidad percibida más que en volumen de calificaciones.

---

# SQL Case Study: Analysis of Reader Behavior During the Pandemic

## US English

**Role:** Data Analyst  
**Technologies:** SQL (PostgreSQL), Python (Pandas), Jupyter Notebook

### Project description  
During the COVID-19 pandemic, changes in social habits drove growth in book consumption and the development of new platforms for readers. In this project, I worked with a relational database from a startup in the publishing sector that is looking to launch a new digital product for readers. The goal was to identify valuable opportunities for this proposal using the available data.

### Project Objectives  
- Explore the database to understand reading and rating behavior.  
- Run SQL queries to extract key metrics on:  
  - Recent publications  
  - User engagement  
  - Author and publisher performance  
- Generate insights to inform product and strategy decisions.

### Database Description  
The database contained five main tables:  

| Table      | Content                                 |  
|------------|-----------------------------------------|  
| books      | Information about books: title, date, pages |  
| authors    | Authors                                 |  
| publishers | Publishers                             |  
| ratings    | Numerical ratings from users           |  
| reviews    | Textual reviews from users             |

Each book is related to an author and a publisher. Ratings and reviews are linked to books via `book_id`.

### Technologies Used  
- SQL (PostgreSQL)  
- Jupyter Notebook  
- Python (Pandas only for printing results)

### Queries Performed and Key Findings  
1. **Books published after January 1, 2000**  
   Result: Increasing volume of publications identified after 2000, supporting focus on modern titles.

2. **Average ratings and number of reviews per book**  
   Result: Some highly rated titles were not the most popular in terms of number of reviews, suggesting opportunities to highlight “hidden gems.”

3. **Publisher with the most books over 50 pages**  
   Result: Leading publisher of extensive publications identified, useful for commercial partnerships or editorial recommendations.

4. **Author with the best average rating (minimum 50 ratings)**  
   Result: Reliable ranking of authors with good critical reception, ideal for highlighting quality content.

5. **Average reviews by users with more than 50 ratings**  
   Result: Most active users write more text reviews than average, could be leveraged as community ambassadors or content creators.

### General Conclusions  
- Combining review data, ratings, and publisher metadata enables effective content personalization strategies.  
- High-potential authors and books not widely recognized yet.  
- Engaged users generate valuable content and are key for loyalty building.

### Value for the Product  
- Content segmentation based on leading publishers or high-performing authors.  
- Focus on active users for engagement campaigns.  
- Content creation based on perceived quality rather than volume of ratings.
