Este proyecto individual es de Ciencias de Datos con el cual se  desea implementar  una ingeniería de datos pasando por el ETL , EDA, API’s hasta desarrollar el deploy de un modelo de Machening Lerning.

Se parte de dos dataset movies.csv y credits.csv que se trata de películas y créditos  de esas películas.

¿Qué vamos a encontrar en este repositorio?

Archivo ETL_Peli.ipynb
Este archivo del repositorio contiene  la realización de extracción, transformación y carga de datos (ETL). El cual se llevó a cabo a través de  la limpieza de los dataset mencionados anteriormente y además esta limpieza dio origen a la creación de nuevos dataset. 

Archivo collextion.csv
Se realizó el tratamiento de la columna “belongs_to_collection” (cada fila de esa columna era un diccionario) perteneciente al dataset movies.csv  obteniendo así un nuevo dataset llamado Collection con cuatro columnas ‘id’, ‘name’,’ poster_path’, ‘backdrop_path’.

Archivo peliculas.csv
Luego de haber realizado la limpieza del dataset movies.csv se crea un nuevo dataset llamado películas.csv que contiene los datos limpios.

Archivo EDA_Peli_ipynb
En la realización de Análisis Exploratorio de Datos (EDA) se realizó el análisis de las variables categóricas a través del conteo y de un gráfico de seaborn.
Luego se procedió un análisis de las variables numéricas mediante pandas describe () que se utiliza para ver algunos detalles estadísticos básicos como percentil, media, estándar, etc. También se llevó a cabo histrogramas.
Se realizó gráfico de dispersión para relación de variables y también un mapa de calor.

Archivo main.py
Para la FastAPI se realizó un archivo main.py este  contiene las funciones y también la recomendación de películas.

Para poder llevar a cabo las funciones se crearon archivos que son los siguientes:

•	películas_idiomas.ipynb este archivo da origen al dataset películas_idiomas.csv necesario para poder realizar una función que al ingresar un idioma devuelva la cantidad de películas producidas en ese idioma.

•	películas_duración.ipynb por el cual se crea el dataset duración_api.csv necesario para poder realizar una función que la ingresar la película devuelva la duración y el año.

•	película_franquicia.ipynb este archivo da origen al dataset películas_franquicia realizado para poder crear una función que al ingresar la fanquicia retorne cantidad de películas, ganancia total y promedio.

•	películas_pais.ipynb crea el datataset películas_pais.csv para poder realizar una función que ingresando un país retorne la cantidad de películas producidas en el mismo.

•	Productoras_exitosas.ipynb  por el cual se crea un dataset productoras_exitosas.csv para poder realizar una función que al ingresar la productora retorne el revunue total y la cantidad de películas que realizo.

•	Director.ipynb por el cual se crea un dataset director.csv para poder realizar una función que al ingresar el nombre del director devuelva el éxito mediante el retorno, el nombre de cada película, fecha de lanzamiento, retorno individual, costo y ganancia de la misma.





