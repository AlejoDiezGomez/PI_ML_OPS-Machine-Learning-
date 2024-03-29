# PROYECTO INDIVIDUAL 1 ML OPS
### [English Readme](englishreadme.md)
## Introducción : 
Este proyecto consiste en crear una API para Steam, construyendo un modelo de recomendacion basado en Machine Learning . Otorgando una interfaz intuitiva para el usuario donde podra consultar datos sobre generos , fechas , sentiment score ,etc. De manera puntual.
## Tecnologías utilizadas :
- FastAPI
- Matplotlib
- NLTK
- Numpy
- Pandas
- Python
- Render
- Scikit-Learn
- Seaborn
- Uvicorn
- Wordcloud
## Resolución :
### 1. [ETL :](ETL.ipynb)
Realice el proceso de ETL (extracción, transformación y carga ) con los archivos obtenidos de distintas fuentes para su posterior análisis y utilización dentro del modelo de ML.
### 2. [EDA :](EDA.ipynb)
Realice el proceso EDA  (Exploratory Data Analysis) en el DataSet obtenido en el etl con el objetivo de identificar relaciones , insights , tendencias y/o patrones , tal que , sirvan para la creacion y ejecucion del modelo de ML
### 3. Modelo de Machine Learning :
Este modelo de  Machine Learning entrega recomendaciones de juegos precisas y personalizadas para cada usuario  con la utilizacion de algoritmos y tecnicas como la similitud del coseno y scikit-lear .
#### Sistema de recomendacion user-item: 
- def recomendacion_usuario( id de usuario ): Ingresando el id de un usuario ('user_id'), deberíamos recibir una lista con 5 juegos recomendados para dicho usuario. 
Ejemplo de uso: 76561198030567998 , 76561198066011588 
#### Sistema de recomendación item-item:
   - def recomendacion_juego( id de producto ): Ingresando el id de producto ('id), deberíamos recibir una lista con 5 juegos recomendados similares al ingresado.
Ejemplo de uso : 70 , 1520
### 4. Deployment de la API
Creamos una API utilizando el módulo FastAPI de Python, creando 5 funciones para que puedan ser consultadas:
- def PlayTimeGenre( genero : str ): Debe devolver año con mas horas jugadas para dicho género. Ejemplo de input: casual , sports 
- def UserForGenre( genero : str ): Debe devolver el usuario que acumula más horas jugadas para el género dado y una lista de la acumulación de horas jugadas por año. Ejemplo de input: action , adventure 
- def UsersRecommend( año : int ): Devuelve el top 3 de juegos MÁS recomendados por usuarios para el año dado. (reviews.recommend = True y comentarios positivos/neutrales) Ejemplo de input: 2014 , 2009 
- def UsersWorstDeveloper( año : int ): Devuelve el top 3 de desarrolladoras con juegos MENOS recomendados por usuarios para el año dado: 2009 , 2012
- def sentiment_analysis( empresa desarrolladora : str ): Según la empresa desarrolladora, se devuelve un diccionario con el nombre de la desarrolladora como llave y una lista con la cantidad total de registros de reseñas de usuarios que se encuentren categorizados con un análisis de sentimiento como valor. Ejemplo de input: Valve

Luego realizamos el deployement de esta API utilizando Render.
## Enlaces : 
- [API](https://alejo-diez-gomez-pi-ml-ops.onrender.com/)
- [Video explicativo](https://www.youtube.com/watch?v=jCIwM6Hw-_U)
## Contacto : 
- [Portafolio Web](https://alejodiezgomez.github.io/)
- [Linkedin](https://www.linkedin.com/in/alejo-gabriel-diez-gomez-402b93254/)
- [alejo10gomezz@gmail.com]()

